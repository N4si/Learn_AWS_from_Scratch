# Launch an EC2 Instance

Learn how to launch and connect to an EC2 instance. This step-by-step guide covers the essential steps to get your instance up and running.

## Steps to Launch an Instance

1. **Sign in to AWS Management Console**
   - Navigate to the [EC2 Dashboard](https://console.aws.amazon.com/ec2/).

2. **Launch Instance**
   - Click "Launch Instance" to start the instance creation wizard.

3. **Choose AMI**
   - Select an Amazon Machine Image (AMI). Options include:
     - **Amazon Linux 2**
     - **Ubuntu Server**
     - **Microsoft Windows Server**

4. **Choose Instance Type**
   - Select the instance type based on your requirements (e.g., `t3.micro` for low-cost testing).

5. **Configure Instance**
   - Set up network settings, IAM roles, and other configurations.

6. **Add Storage**
   - Attach Elastic Block Store (EBS) volumes. Default volume size and type can be modified.

7. **Add Tags**
   - Apply tags to organize and identify instances (e.g., Name: `MyWebServer`).

8. **Configure Security Group**
   - Define inbound and outbound rules. For example, allow HTTP (port 80) and SSH (port 22).

9. **Review and Launch**
   - Review your settings and click "Launch". Select an existing key pair or create a new one.

## Connecting to Your Instance

- **Linux**: Use SSH:
  ```bash
  ssh -i "your-key.pem" ec2-user@your-instance-public-dns


**Windows**: Use Remote Desktop (RDP). Download the RDP file and use the password generated during instance launch.


### Example Use Case
Development: Developers use EC2 instances to test new applications before deploying them to production.


### Certification Tips
Practice launching and configuring instances: Key for the AWS Certified Solutions Architect and AWS Certified DevOps Engineer exams.


### Resources
[Connecting to Your Instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connect-to-linux-instance.html)
