# 🛠️ S3 Bucket Task: DevOps & Cloud Engineer

This task focuses on using Amazon S3 in a DevOps/Cloud Engineering workflow. You'll automate S3 bucket management, integrate security, and implement best practices for handling data storage at scale.

## Task Overview

You will:
1. Create and configure an S3 bucket using the AWS CLI.
2. Implement bucket policies and IAM roles for secure access control.
3. Enable versioning and configure lifecycle policies.
4. Automate uploads with the AWS CLI.
5. Enable server-side encryption.
6. Set up event notifications for integration with Lambda.

---

### 🛠️ Step 1: Create an S3 Bucket

Create an S3 bucket using the AWS CLI. Buckets need unique names and a specified region.

```bash
aws s3api create-bucket \
    --bucket <bucket-name> \
    --region <region> \
    --create-bucket-configuration LocationConstraint=<region>
