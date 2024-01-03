# AWS-Website
Title: Hotsing a Website in AWS using Terraform and Git

# Steps to clone 
```
git clone https://github.com/atulkamble/AWS-Website.git
```

# Services and Tools:
- EC2
- github
- VPC
- S3
- IAM
- terraform
- AWS CLI

# Architecture


# Environment and Installation | Configuration | Tools
* CREATE EMPLOYEE ACCOUNT | PROVIDE ACCESS *
- Naviagte to IAM
- Create a user | atulkamble
- Add this user 'Administrator Group'
- Align Policy | FullAccessAdmin
- Create Console Sign in | Credentials Access file to be generated | Note it down.
- Sign in to AWS-CLI credentials.
```
aws configure
```
- Enter Default Region
- Enter Access Keys
- Secret Access key
- Output Format: json

# Developement

# Testing

# Script
- Navigate and Clone Project Folder
- Install git 
- Install Github Desktop
- Install VSCode
- Install Terraform | Configure System Variables | terraform -version
- Try Powershell | Update Powershell

// Set Credentials in git system
git config --global user.name "Full Name"
git config --global user.email "email id"

// Creating and Cloning Repository
```
mkdir Project
cd Project
git clone https://github.com/atulkamble/AWS-Website.git
cd AWS-Website
```

// Open Project in a VS Code
```
code .
```

// Update Code and Push Code to Github Repository
```
git status
git add README.md
git commit -m "Updated README File"
git push
```
// Saving terraform code in Code Folder
```
mkdir Code
cd Code
```

// Creating main file in terraform
```
New-Item main.tf
OR
touch main.tf
```
// Paste [AWS-Provider Details from following link](https://registry.terraform.io/providers/hashicorp/aws/latest)

// Opeining in VSCode
```
code main.tf
```
// Webserver on EC2 using Terraform

Note Down 
- Default VPC ID: vpc-0d1614828f3a43cbb
- Default Subnet ID: subnet-05a2cec43d3000109
- Security Group ID: sg-04eae7284fe9624cf
- AMI ID: ami-0a0f1259dd1c90938

Create a file >> main.tf >> Paste main.tf Code in it

// Create directory 

Paste keypair ```default-ec2.pem``` in directory ```aws/aws_keys``` within terraform directory


// Paste Following Code in variables.tf

```
variable "aws_key_pair" {
  default = "aws/aws_keys/default-ec2.pem"
}
```

// Terraform Commands
```
terraform init
terraform fmt
terrfaorm validate
terraform plan
terraform apply
yes
terraform destroy
```
