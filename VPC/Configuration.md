# Configuring a VPC 🛠️

## Step-by-Step Guide

### 1. Create a VPC
- Navigate to the VPC Dashboard in the AWS Management Console.
- Click on "Create VPC."
- Define the IP address range (CIDR block), e.g., 10.0.0.0/16.

### 2. Create Subnets
- Choose "Subnets" from the VPC Dashboard.
- Click "Create Subnet" and specify the VPC, Availability Zone, and CIDR block for the subnet.

### 3. Configure Route Tables
- Go to "Route Tables" and select "Create Route Table."
- Associate it with your VPC and define routes as needed.

### 4. Attach an Internet Gateway
- Go to "Internet Gateways" and click "Create Internet Gateway."
- Attach it to your VPC.

### 5. Set Up a NAT Gateway (for Private Subnets)
- Navigate to "NAT Gateways" and click "Create NAT Gateway."
- Choose a subnet and allocate an Elastic IP.

### 6. Configure Security Groups and Network ACLs
- Create security groups with appropriate inbound and outbound rules.
- Define Network ACLs to control traffic at the subnet level.