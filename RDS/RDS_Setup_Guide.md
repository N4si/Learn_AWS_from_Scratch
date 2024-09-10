# Amazon RDS Setup Guide 🛠️

## Step 1: Provision an RDS Instance

1. *Launch RDS: In the **RDS dashboard, click **Create Database*.
2. *Choose Engine*: Select the database engine based on your use case. For web apps, MySQL and PostgreSQL are common choices.
3. *Configure DB Settings*:
   - Instance Class: Choose compute capacity (e.g., db.t3.micro for small workloads, db.m5.large for production).
   - Storage: Select *General Purpose SSD* or *Provisioned IOPS* based on performance needs.
   - Multi-AZ: Enable for high availability in production environments.
   - VPC: Select an appropriate *VPC* and configure *subnets* and *security groups*.

4. *Backup and Monitoring*:
   - Enable *automatic backups* and set retention periods.
   - Enable *Enhanced Monitoring* and integrate with *CloudWatch* for performance insights.

5. *Security*:
   - Use *IAM roles* for DB access management.
   - Enable *Encryption at Rest* using AWS *KMS* (Key Management Service).
   - Apply *SSL/TLS* for data in transit.

## Step 2: Connecting to the RDS Instance
- After the instance is created, retrieve the *RDS endpoint* from the AWS console.
- Use a database client like MySQL Workbench or pgAdmin to connect:
```bash
mysql -h <RDS_ENDPOINT> -P 3306 -u <USERNAME> -p

Automate Provisioning with Terraform
Here’s an example of how to create an RDS instance using Terraform:
resource "aws_db_instance" "default" {
  allocated_storage    = 20
  engine               = "mysql"
  instance_class       = "db.t3.micro"
  name                 = "mydb"
  username             = "admin"
  password             = "password"
  parameter_group_name = "default.mysql8.0"
  skip_final_snapshot  = true
}