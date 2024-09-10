# VPC Components 🧩

## 1. Subnets 🕵️‍♂️
- *Public Subnets*: Accessible from the internet.
- *Private Subnets*: Not directly accessible from the internet.

## 2. Route Tables 🛤️
- *Main Route Table*: Default route table associated with your VPC.
- *Custom Route Tables*: Create custom route tables for more control.

## 3. Internet Gateway 🌍
- *Purpose*: Allows communication between instances in your VPC and the internet.

## 4. NAT Gateway 🔄
- *Purpose*: Enables outbound internet traffic for instances in private subnets.

## 5. VPC Peering 🔗
- *Purpose*: Connects two VPCs enabling them to communicate.

## 6. Security Groups 🔒
- *Purpose*: Acts as a virtual firewall to control traffic for your instances.

## 7. Network ACLs 🚧
- *Purpose*: Provides an additional layer of security at the subnet level.