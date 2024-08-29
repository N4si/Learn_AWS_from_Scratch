# Elastic IPs

Elastic IPs are static IP addresses designed for dynamic cloud computing. They provide persistent IP addresses for your EC2 instances, even if they are stopped or restarted.

## Key Points

- **Allocation**: Allocate an Elastic IP from the AWS Management Console or CLI.
- **Association**: Attach the Elastic IP to your EC2 instance.
- **Release**: Release the Elastic IP when no longer needed to avoid extra charges.

## Benefits

- **Static IP**: Maintain a consistent IP address even if the instance is stopped or restarted.
- **Failover**: Quickly remap the IP address to another instance in case of failure or maintenance.

## Example Use Case

- **High Availability**: Use Elastic IPs to ensure that your application's IP address remains constant, even if you need to replace the underlying instance.

## Certification Tips

- **Understand Elastic IP management and cost implications**: Useful for AWS Certified Solutions Architect and AWS Certified DevOps Engineer exams.

## Resources

- [Elastic IP Addresses](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/elastic-ip-addresses-eip.html)
- [Elastic IP Best Practices](https://aws.amazon.com/blogs/aws/elastic-ip-addresses-a-new-best-practice/)
