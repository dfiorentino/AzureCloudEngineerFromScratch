# Azure Active Directory

<p align=center>
<img src="../assets/aad.png" alt="ARM" title="ARM"> </p>

Azure Active Directory (AAD or Azure AD) is a cloud-based identity and access management service.

# Key Concepts for Azure AD

- <strong>Identity:</strong> An object that can get authenticated.

- <strong>Account:</strong> An identity that has data associated with it. You can't have an account without an identity.

- <strong>Azure AD Account:</strong> An identity created through Azure AD or another Microsoft cloud service, such as Microsoft 365. Identities are stored in Azure AD and accessible to your organization's cloud service subscriptions. This account is also sometimes called a Work or school account.

# User and Groups Accounts

**Users**

Azure AD handle three types of users:

- <strong>Cloud Identity:</strong> user accounts that only exist in Azure AD.

- <strong>Directory-syncronized Identities:</strong> these users exist in an OnPrem Active Directory and are syncronized through Azure AD Connect.

- <strong>Guest users:</strong> these users exist outside Azure. Accounts created using an invite from Azure AD and a external domain like outlook.com or gmail.com.

**Groups**

Azure AD handle two different types of groups:

- <strong>Security Groups:</strong> Security groups are used to manage member and computer access to shared resources for a group of users

- <strong>Microsoft 365 Groups:</strong> Microsoft 365 groups provide collaboration opportunities by giving members access to a shared mailbox, calendar, files, SharePoint site, and more

**Group Membership**

There are three ways that you can use to assign access rights:

- <strong>Assigned:</strong> allow only add speficic users to be member of this particular group.
- <strong>Dynamic User:</strong> allow to use a dynamic rules to automatically add or remove members, in this cases users only.
- <strong>Dynamic Device:</strong> allow to use a dynamic rules to automatically add or remove members, in this cases devices only.

# Administrative Units

Administrative units allow an organization to grant admin permissions that are restricted to a department, region, or any other segment of the organization that you define. An administrative unit can contain only users and groups

# Guest Accounts

# Role-Based Account Control