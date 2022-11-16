# CloudFormationPrivateVPC
a Yaml file which built to be used with AWS cloudFormation to build a Virtual Private Cloud VPC

the code builds the following: 
VPC 
a public subnet 
two private subnets
a gateway and VPCgatewayattachment 
a NAT gateway with elastic IP 
Load Balancer with a listener and target group 
route tables with routes and route table assosiations 
2 private ec2-s with private security group
a public ec2 with public security group 
key for accessing ec2-s 

Notes: 
the UserData file in public ec2 has a public key generated to access from out side of the VPC to the ec2 since the generated key in by cloudformation secret.
