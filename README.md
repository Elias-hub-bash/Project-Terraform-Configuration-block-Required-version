Terraform Configuration Block

Terraform relies on plugins called "providers" to interact with remote systems and expand functionality. 
Terraform configurations must declare which providers they require so that Terraform can install and use them. 
This is performed within a Terraform configuration block.

     1: Check Terraform version
     2: Require specific versions of Terraform



Run the following command to check the Terraform version:

terraform -version

You should see:

Terraform v1.0.8


Create a file titled terraform.tf to define a minimum version of Terraform to be used.

terraform.tf

 terraform {
   required_version = ">= 1.0.0"
 }

terraform int

Terraform v1.0.8

This informs Terraform that it must be at least of version 1.0.0 to run the code. If Terraform is an earlier version it will throw an error.

Update the required_version line to "=1.0.0" and run terraform init.
