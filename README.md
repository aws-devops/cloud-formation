# Cloud-formation for  WordPress

This repository contains AWS cloud formation template. This template could be used to bootstrap an ec2 instance with the LAMP stack serving a Wordpress blog.

##  Parameters Used

**DBRootPassword** Root password for MySQL database.

**DBName** The WordPress database name.

**DBPassword** The WordPress database admin account password.

**DBUser** The WordPress database administrator account username.

**InstanceType** WebServer EC2 instance type.

**KeyName** Name of an existing EC2 KeyPair to enable SSH access to the instance.

**SSHLocation** The CIDR range to which ssh port would be opened.

##  Usage

1. Clone this repository to your local workstation.
2. Log-in to your AWS Managemnt console and choose CloudFormation.
3. Select Create a stack and choose upload the template. You can upload ec2-vpc-wordpress.json file from the local repositoy.
4. Provide the required parameters and create the stack.
5. Check the wordpress blog by visiting to the link http://instance-ip-address/wordpress/
