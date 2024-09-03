# AWS IAM Best Practices

## Overview
Following best practices ensures that your IAM setup is secure, manageable, and scalable.

## Key Practices

1. **Use Least Privilege**: Grant only the permissions necessary for users to perform their tasks.
2. **Use Groups**: Manage permissions via groups rather than assigning policies directly to users.
3. **Enable MFA**: Use Multi-Factor Authentication (MFA) for an additional layer of security.
4. **Regularly Review Permissions**: Periodically review and adjust permissions to ensure they align with current needs.
5. **Rotate Credentials**: Regularly rotate access keys and passwords.
6. **Use Roles for AWS Services**: Assign roles to AWS services rather than using access keys for better security.

## Practical Examples

- **Implementing Least Privilege**: Create a policy that grants only the required actions (e.g., read-only access).
- **Configuring MFA**:
    1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/).
    2. Open the IAM console at [IAM Dashboard](https://console.aws.amazon.com/iam/home).
    3. In the navigation pane, click **Users**, then select the user.
    4. Click the **Security credentials** tab.
    5. In the **Multi-Factor Authentication (MFA)** section, click **Manage**.
    6. Follow the instructions to configure MFA.

**Next:** [AWS IAM Troubleshooting](07-troubleshooting.md)