# Cloud-formation for  WordPress
-------------------
This repository contains AWS cloud formation template. This template could be used to bootstrap an ec2 instance with the LAMP stack serving a Wordpress blog.

##  Parameters Used

**DBRootPassword**Root password for MySQL database.

**DBName** The WordPress database name.
**DBPassword** The WordPress database admin account password.
**DBUser** The WordPress database administrator account username.
*InstanceType** WebServer EC2 instance type.
**KeyName** Name of an existing EC2 KeyPair to enable SSH access to the instance.
**SSHLocation** The CIDR range to which ssh port would be opened.
