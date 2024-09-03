# AWS IAM Groups

## Overview
IAM groups allow you to manage permissions for multiple users collectively.

## Key Points
- **Permissions**: Users in a group inherit the group’s policies.
- **Organization**: Group users by roles (e.g., Developers, Admins).

## Practical Examples

### AWS CLI

- **Create a Group**:
    ```bash
    aws iam create-group --group-name Developers
    ```

- **Add User to Group**:
    ```bash
    aws iam add-user-to-group --user-name Alice --group-name Developers
    ```

### AWS Management Console

- **Create a Group**:
    1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/).
    2. Open the IAM console at [IAM Dashboard](https://console.aws.amazon.com/iam/home).
    3. In the navigation pane, click **Groups**.
    4. Click **Create New Group**.
    5. Enter a **Group name** and click **Next Step**.
    6. Attach policies to the group as needed and click **Next Step**.
    7. Review and click **Create Group**.

- **Add User to Group**:
    1. In the IAM console, go to **Groups**.
    2. Select the group you want to modify.
    3. Click the **Users** tab.
    4. Click **Add users to group**.
    5. Select the users to add and click **Add users**.

**Next:** [AWS IAM Roles](04-roles.md)
