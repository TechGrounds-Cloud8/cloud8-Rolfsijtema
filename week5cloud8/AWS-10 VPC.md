# [Virtual Private Cloud (VPC)]


## Key terminology

**Default VPC**
When you create a AWS Account you always get a Default VPC
Whit this VPC you can create: 
- subnets
- internet gateways (igw)
- NAT gateways
- VPN: Virtual Private Network Connections
- Add up to 5 no-default VPC's per region. (These 5 are a soft limit: means you can ask this limit to be raised)

Many services within AWS need a VPC for example:
- EC2 Elastic Compute
- RDS Relational Database Service
- ECS Elastic Container Service

**CIDR** 
CIDR: Classless Inter-Domain Routing 

When creating a VPC you need to choose a CIDR BLOCK

In contrast to classful routing, which categorizes addresses into one of three blocks, CIDR allows for blocks of IP addresses to be allocated to Internet service providers. The blocks are then split up and assigned to the provider's customers

CIDR, which stands for Classless Inter-Domain Routing, is an IP addressing scheme that improves the allocation of IP addresses. It replaces the old system based on classes A, B, and C. This scheme also helped greatly extend the life of IPv4 as well as slow the growth of routing tables.
The CIDR number is typically preceded by a slash “/” and follows the IP address. For example, an IP address of 131.10. 55.70 with a subnet mask of 255.0. 0.0 (which has 8 network bits) would be represented as 131.10.


## Exercise


### Sources
[List your sources you used for solving the exercise]

### Overcome challanges
[Give a short description of your challanges you encountered, and how you solved them.]

### Results
[Describe here the result of the exercise. An image can speak more than a thousand words, include one when this wisdom applies.]
