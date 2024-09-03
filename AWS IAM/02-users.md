# AWS IAM Users

## Overview
IAM users represent individuals or services that need access to AWS resources. Each user has unique credentials.

## Key Points
- **Credentials**: Users have passwords and access keys.
- **Permissions**: Permissions are usually managed via groups.

## Practical Examples

### AWS CLI

- **Create a User**:
    ```bash
    aws iam create-user --user-name Alice
    ```

- **Assign a Policy to a User**:
    ```bash
    aws iam attach-user-policy --user-name Alice --policy-arn arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess
    ```

### AWS Management Console

- **Create a User**:
    1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/).
    2. Open the IAM console at [IAM Dashboard](https://console.aws.amazon.com/iam/home).
    3. In the navigation pane, click **Users**.
    4. Click **Add user**.
    5. Enter a **User name**, select **Access type** (e.g., **Programmatic access** and/or **AWS Management Console access**).
    6. Click **Next: Permissions**.
    7. Set permissions as needed and click **Next: Tags**.
    8. (Optional) Add tags and click **Next: Review**.
    9. Click **Create user**.

- **Assign a Policy to a User**:
    1. In the IAM console, go to **Users**.
    2. Select the user you want to modify.
    3. Click the **Permissions** tab.
    4. Click **Add permissions**.
    5. Choose **Attach policies directly**.
    6. Search for and select the policy (e.g., **AmazonS3ReadOnlyAccess**).
    7. Click **Next: Review**, then **Add permissions**.

**Next:** [AWS IAM Groups](03-groups.md)
