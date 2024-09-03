# AWS IAM Troubleshooting

## Common Issues and Solutions

### Issue 1: Access Denied Errors

- **Problem**: Users receive "Access Denied" errors.
- **Solution**: 
  1. Check the user's permissions and ensure they have the correct policies attached.
  2. Review the IAM policy and ensure it grants the required actions.

### Issue 2: Policies Not Taking Effect

- **Problem**: Policies seem to not apply correctly.
- **Solution**: 
  1. Verify that the policy is correctly attached to the user, group, or role.
  2. Use IAM Policy Simulator to test the policy and identify issues.

### Issue 3: Role Assumption Failures

- **Problem**: Roles cannot be assumed.
- **Solution**: 
  1. Check the trust policy of the role to ensure it allows the intended entities to assume the role.
  2. Verify the role's permissions and make sure they are correctly configured.

## Practical Examples

- **Using IAM Policy Simulator**:
    1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/).
    2. Open the IAM console at [IAM Dashboard](https://console.aws.amazon.com/iam/home).
    3. In the navigation pane, click **Policy Simulator**.
    4. Enter the policy details and simulate actions to test permissions.
