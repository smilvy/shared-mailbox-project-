
# Shared Mailbox Management in Microsoft 365 Using Microsoft 365 Admin Console

## Project Overview
This guide provides a step-by-step approach to managing shared mailboxes in Microsoft 365 using the Microsoft 365 Admin Console. It covers creating shared mailboxes, assigning permissions to users for access, and configuring retention policies and Litigation Hold to support compliance. This approach is designed for IT administrators who prefer a console-based setup within the Microsoft 365 environment without using PowerShell.

## Objectives
1. **Create a Shared Mailbox**: Use the Microsoft 365 Admin Console to set up shared mailboxes accessible by multiple users.
2. **Assign Permissions**: Grant users appropriate access rights to shared mailboxes, including Full Access, Send As, or Send on Behalf permissions.
3. **Configure Retention Policies**: Define and apply data retention policies to manage data lifecycle.
4. **Enable Litigation Hold**: Enable Litigation Hold on shared mailboxes to preserve emails for legal and compliance purposes.

## Prerequisites
- **Microsoft 365 License**: Ensure that shared mailboxes are covered under the appropriate license.
- **Admin Access**: Access to the Microsoft 365 Admin Console and Exchange Admin Center.
- **Microsoft 365 Compliance Center**: Access for managing retention policies and Litigation Hold settings.

## Step-by-Step Setup Guide

### Step 1: Create a Shared Mailbox
1. **Log in to the Microsoft 365 Admin Center** at [admin.microsoft.com](https://admin.microsoft.com).
2. In the left-hand navigation, go to **Teams & groups** > **Shared mailboxes**.
3. Click **+ Add a shared mailbox**.
4. Enter a **Display name** and **Email address** for the shared mailbox, then click **Save changes**.
5. Once created, the shared mailbox will appear in the list, and you can manage settings and permissions from here.

### Step 2: Assign Permissions to Users

1. In the **Shared mailboxes** section, select the shared mailbox you created.
2. Under **Members**, click **Edit** to add users who should have access to the mailbox.
3. Choose the users who will have **Full Access** permissions (view and manage all emails).
4. For **Send As** permissions (to send emails as the shared mailbox), select **Mailbox delegation** and click **Edit** under **Send As**.
5. Choose the users and groups you wish to allow **Send As** permissions and click **Save**.
6. For **Send on Behalf** permissions (to send emails on behalf of the shared mailbox), go to **Mailbox delegation** and select **Send on behalf**.

### Step 3: Configure Retention Policies
1. Navigate to the **Microsoft 365 Compliance Center** at [compliance.microsoft.com](https://compliance.microsoft.com).
2. In the Compliance Center, go to **Policies** > **Data lifecycle management** > **Retention policies**.
3. Click **+ Create retention policy** to start configuring a new retention policy.
4. Give the policy a **Name** and **Description**.
5. Select the option to **Retain items** or **Delete items** based on your organization’s compliance needs.
6. Under **Locations**, select **Exchange email** and specify the shared mailbox email address.
7. Review and apply the settings, then click **Submit** to save the policy.

### Step 4: Enable Litigation Hold

1. Go to the **Microsoft 365 Admin Center** and open the **Exchange Admin Center** (EAC).
2. In the EAC, navigate to **Recipients** > **Mailboxes**.
3. Locate the shared mailbox and click on it to open the **Properties** panel.
4. In the mailbox properties, select **Others** under Mailbox features.
5. Find **Litigation Hold** and enable it by clicking **Enable**.
6. Enter the **Litigation Hold Duration** (in days) if you have a specific retention period, or leave it blank to hold data indefinitely.
7. Click **Save** to apply Litigation Hold to the mailbox.

### Step 5: Verify Configuration

1. **Shared Mailbox Access**: Verify that users can view and access the shared mailbox in Outlook or Outlook on the Web.
2. **Permissions**: Confirm that assigned permissions are functioning by testing **Full Access**, **Send As**, and **Send on Behalf** features.
3. **Retention Policy**: Check that the retention policy is applied to the shared mailbox by reviewing the settings in the **Compliance Center**.
4. **Litigation Hold**: Confirm Litigation Hold status by returning to the **Exchange Admin Center** > **Recipients** > **Mailboxes** > **Others**.

## Usage Guidelines

- **Accessing the Shared Mailbox**: Users with Full Access permissions can add the shared mailbox to their Outlook profile by going to **File** > **Account Settings** > **Account Settings** > **Change** > **More Settings** > **Advanced** > **Add**.
- **Retention Policy Application**: Ensure that the shared mailbox data is compliant with company retention policies.
- **Litigation Hold Precautions**: Inform users that Litigation Hold preserves all email data and cannot be bypassed; it’s critical for eDiscovery and compliance audits.

## Key Benefits

- **Seamless Collaboration**: Shared mailboxes provide a centralized platform for team communication.
- **Controlled Access**: Role-based permissions ensure that only authorized users can access and manage shared mailboxes.
- **Data Compliance**: Retention policies and Litigation Hold enable data protection and ensure compliance with legal requirements.

## Troubleshooting

- **User Permission Issues**: Verify permissions in the **Shared Mailboxes** section in the Admin Center and adjust as necessary.
- **Retention Policies Not Applying**: Confirm that the policy is enabled and assigned to the correct mailbox in the Compliance Center.
- **Litigation Hold Not Working**: Ensure that Litigation Hold is enabled and consult the Exchange Admin Center settings for verification.

## Additional Resources

- [Microsoft 365 Admin Center](https://admin.microsoft.com)
- [Exchange Admin Center Documentation](https://docs.microsoft.com/exchange/exchange-admin-center)
- [Microsoft 365 Compliance Center Documentation](https://docs.microsoft.com/microsoft-365/compliance/)

---

This README provides an overview of managing shared mailboxes in Microsoft 365 using the Admin Console, focusing on setup, permissions, retention, and compliance. For further customization,consult Onyechere Esther @aesther083@gmail.com
