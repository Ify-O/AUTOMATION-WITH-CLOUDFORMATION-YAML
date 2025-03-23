# AUTOMATION WITH CLOUDFORMATION
 
Creating a CloudFormation Stack using YAML

#Attributes
The Parameters section has includes: 
MyVpcCidr
PublicSubnetCidr
AmazonLinuxAMIID 
These parameters are referenced in the Resources section.

The Resources section contains most of the lines in this template. It creates the following resources:
S3 Bucket
VPC
EC2 instance named Web Server.
WaitCondition and WaitHandle resources that wait for the userdata script (which is specified in the EC2 instance details) to complete.
Internet Gateway
Security Group resource named WebServerSG.
Public Route Table
Public Subnet

The Outputs section writes out the name of the VPCDefaultSecurityGroup, S3 bucket and the public IP address of the EC2 instance that were created.
