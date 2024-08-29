# Introduction to EC2

Amazon EC2 (Elastic Compute Cloud) provides scalable virtual servers in the cloud. This section introduces you to EC2, its instance types, pricing models, and key concepts.

## Key Concepts

- **Instance Types**: Different types of instances tailored for various use cases:
  - **General Purpose**: `t3.micro`, `t3.medium` – Balanced compute, memory, and networking resources.
  - **Compute Optimized**: `c5.large`, `c5.xlarge` – High performance for compute-intensive tasks.
  - **Memory Optimized**: `r5.large`, `r5.xlarge` – Designed for memory-intensive applications.

- **Pricing Models**: 
  - **On-Demand Instances**: Pay for compute capacity by the hour or second. No long-term contracts.
  - **Reserved Instances**: Commit to a one- or three-year term for a significant discount.
  - **Spot Instances**: Purchase unused capacity at reduced rates by bidding.
  Watch this video on Pricing Models: 

- **Regions and Availability Zones**: Deploy instances in multiple geographic locations to improve fault tolerance and redundancy.

## Example Use Case

- **Startup**: A startup may use on-demand instances to scale up during peak times and save costs during off-peak periods.

## Certification Tips

- **Understand instance types and pricing**: Essential for AWS Certified Solutions Architect and AWS Certified DevOps Engineer exams.

## Resources

- [EC2 Pricing](https://aws.amazon.com/ec2/pricing/)
- [EC2 Instance Types](https://aws.amazon.com/ec2/instance-types/)
- [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)
