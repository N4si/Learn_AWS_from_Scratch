# AWS IAM Policies

## Overview
IAM policies are JSON documents that specify permissions. They determine what actions are allowed or denied for specific resources.

## Key Points
- **Managed Policies**: AWS or customer-created policies that can be attached to multiple entities.
- **Inline Policies**: Policies directly attached to a single user, group, or role.

## Practical Examples

### AWS CLI

- **Create an Inline Policy**:
    ```json
    {
      "Version": "2012-10-17",
      "Statement": [
        {
          "Effect": "Allow",
          "Action": "s3:ListBucket",
          "Resource": "arn:aws:s3:::example_bucket"
        }
      ]
    }
    ```
    ```bash
    aws iam put-user-policy --user-name Alice --policy-name ListS3Policy --policy-document file://policy.json
    ```

- **Attach a Managed Policy**:
    ```bash
    aws iam attach-user-policy --user-name Alice --policy-arn arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess
    ```

### AWS Management Console

- **Create an Inline Policy**:
    1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/).
    2. Open the IAM console at [IAM Dashboard](https://console.aws.amazon.com/iam/home).
    3. In the navigation pane, click **Users**, then select the user.
    4. Click the **Permissions** tab and then **Add inline policy**.
    5. Enter the policy JSON or use the visual editor, then click **Review policy**.
    6. Enter a **Policy name** and click **Create policy**.

- **Attach a Managed Policy**:
    1. In the IAM console, go to **Users**, then select the user.
    2. Click the **Permissions** tab and then **Add permissions**.
    3. Choose **Attach policies directly**.
    4. Search for and select the policy (e.g., **AmazonS3ReadOnlyAccess**).
    5. Click **Next: Review**, then **Add permissions**.

**Next:** [AWS IAM Best Practices](06-best-practices.md)