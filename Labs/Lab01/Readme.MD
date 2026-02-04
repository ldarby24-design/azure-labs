# Lab 01 — Manage Microsoft Entra ID Identities

## Lab Overview

**Module:** Administer Identity  
**Estimated Time:** 30 minutes  
**Completion Date:** [Your Date Here]  
**Region Used:** East US  
**Status:** ✅ Completed

---

## Objectives

This lab focused on creating and managing user accounts and groups in Microsoft Entra ID (formerly Azure Active Directory). The goal was to understand the basic building blocks of Azure identity management.

**What I Learned:**
- How to create internal user accounts in Entra ID
- How to invite external guest users to the organization
- How to create and configure security groups
- The difference between assigned and dynamic group membership
- How tenants work in Microsoft Entra ID

---

## Lab Scenario

The organization is building a new lab environment for pre-production testing. Engineers are being hired to manage this environment, and I was tasked with:
1. Provisioning user accounts (internal and guest users)
2. Creating security groups to organize these users
3. Configuring group membership to minimize administrative overhead

---

## Tasks Completed

### ✅ Task 1: Create and Configure User Accounts

**What I Did:**
1. Signed into the Azure Portal (https://portal.azure.com)
2. Navigated to Microsoft Entra ID via the search bar
3. Explored the Entra ID Overview blade and reviewed tenant information
4. Created an internal user account (`az104-user1`)
5. Configured user properties including job title, department, and location
6. Invited an external guest user using my personal email
7. Configured the same properties for the guest user

**Key Settings Used:**

| Setting | Value |
|---------|-------|
| Internal User | az104-user1 |
| Display Name | az104-user1 |
| Job Title | IT Lab Administrator |
| Department | IT |
| Usage Location | United States |
| Guest User Email | [My personal email] |
| Guest Display Name | [My name] |

**Challenges Encountered:**
- [Note any issues you faced, e.g., "Had to refresh the page multiple times before the guest user appeared"]
- [Add your specific experiences]

**Screenshots Taken:**
- ✅ `01_entra_id_overview.png` — Entra ID Overview page with tenant information
- ✅ `02_user1_created.png` — Users list showing az104-user1
- ✅ `03_both_users_created.png` — Users list showing both internal and guest users

---

### ✅ Task 2: Create Groups and Add Members

**What I Did:**
1. Navigated to the Groups blade in Entra ID
2. Reviewed group settings (Expiration and Naming policy options)
3. Created a new Security group named "IT Lab Administrators"
4. Set myself as the group owner
5. Added both az104-user1 and the guest user as group members
6. Verified the group was created successfully
7. Confirmed members and owners were properly assigned

**Key Settings Used:**

| Setting | Value |
|---------|-------|
| Group Type | Security |
| Group Name | IT Lab Administrators |
| Group Description | Administrators that manage the IT lab |
| Membership Type | Assigned |
| Owners | [My account] |
| Members | az104-user1, [Guest user] |

**Why These Settings Matter:**
- **Security groups** control access to Azure resources
- **Assigned membership** means manual management (vs Dynamic which auto-adds based on rules)
- **Owners** can manage group membership and settings
- **Members** inherit permissions assigned to the group

**Screenshots Taken:**
- ✅ `04_group_members.png` — IT Lab Administrators group showing Members tab
- ✅ `05_group_owners.png` — IT Lab Administrators group showing Owners tab

---

### ✅ Demo Walkthrough: Additional Exploration

**What I Did:**
1. Reviewed license and domain information on the Entra ID Overview page
2. Explored user account management options (Reset password, Delete user, Sign-ins)
3. Reviewed group configuration options (Expiration, Naming policy)
4. Confirmed the group membership type and verified all members

**Screenshots Taken:**
- ✅ `06_demo_tenant_info.png` — Tenant information section
- ✅ `07_demo_user_profile.png` — az104-user1 profile with action buttons
- ✅ `08_demo_group_detail.png` — IT Lab Administrators group detail page

---

## Key Concepts Learned

### 1. **Tenants**
A tenant is a specific instance of Microsoft Entra ID that represents an organization. It contains all the accounts, groups, and applications for that organization.

**Real-world example:** Each company has its own tenant. When you sign into Office 365 or Azure with your work account, you're accessing your company's tenant.

### 2. **User Account Types**

| Type | Description | Use Case |
|------|-------------|----------|
| **Internal User** | Created within the organization's Entra ID | Employees, full-time contractors |
| **Guest User** | Invited from outside the organization | Partners, vendors, consultants |

**Key Difference:** Guest users have more restricted permissions and appear with `#EXT#` in their username.

### 3. **Groups**

**Security Groups** — Used to manage access to Azure resources
- Can contain users and devices
- Used for assigning permissions (RBAC)
- Can be nested (groups within groups)

**Microsoft 365 Groups** — Used for collaboration
- Includes shared mailbox, calendar, files
- Used for Teams, SharePoint, Planner

### 4. **Membership Types**

| Type | How It Works | When to Use |
|------|--------------|-------------|
| **Assigned** | Manually add/remove members | Small teams, specific roles |
| **Dynamic** | Auto-add based on user properties (requires Premium P1/P2) | Large organizations, rule-based membership |

**Example Dynamic Rule:** All users with JobTitle = "IT Lab Administrator" are automatically added to the group.

---

## Screenshots Summary

All screenshots are stored in the `screenshots/` folder:

| # | Filename | Description | Completed |
|---|----------|-------------|-----------|
| 1 | `01_entra_id_overview.png` | Entra ID Overview page | ✅ |
| 2 | `02_user1_created.png` | Internal user created | ✅ |
| 3 | `03_both_users_created.png` | Both users visible | ✅ |
| 4 | `04_group_members.png` | Group members list | ✅ |
| 5 | `05_group_owners.png` | Group owners list | ✅ |
| 6 | `06_demo_tenant_info.png` | Tenant information | ✅ |
| 7 | `07_demo_user_profile.png` | User profile with actions | ✅ |
| 8 | `08_demo_group_detail.png` | Group detail page | ✅ |

---

## Real-World Applications

**Scenario 1: New Employee Onboarding**
When a new IT administrator joins:
1. Create their user account in Entra ID
2. Add them to the "IT Lab Administrators" group
3. They automatically inherit all permissions assigned to that group
4. No need to manually assign individual permissions

**Scenario 2: Contractor Access**
When working with an external contractor:
1. Invite them as a guest user
2. Add them to specific project groups
3. They get limited access based on group membership
4. Easy to revoke access by removing them from groups

**Scenario 3: Department Reorganization**
If the IT department restructures:
1. Create new groups for each team
2. Use dynamic membership based on department property
3. Users automatically move to correct groups when their department changes
4. Minimizes manual administrative work

---

## Best Practices Observed

✅ **Naming Conventions**
- Used descriptive names for users (`az104-user1` follows lab convention)
- Used clear group names that indicate purpose (`IT Lab Administrators`)

✅ **Least Privilege**
- Created a specific group instead of giving users direct access
- Assigned only necessary permissions to the group

✅ **Documentation**
- Added descriptions to groups explaining their purpose
- Documented job titles and departments for all users

✅ **Organization**
- Kept related users in the same group
- Used consistent properties (job title, department, location)

---

## Common Issues & Solutions

### Issue 1: User not appearing after creation
**Problem:** Created a user but they didn't show up in the list  
**Solution:** Had to refresh the page (F5) - Azure portal doesn't always auto-refresh  
**Lesson:** Always manually refresh after creating resources

### Issue 2: Guest user invitation not received
**Problem:** Guest user email didn't arrive immediately  
**Solution:** Waited 5 minutes, checked spam folder  
**Lesson:** Guest invitations can take a few minutes to process

### Issue 3: Cannot change membership type to Dynamic
**Problem:** Dynamic membership option was grayed out  
**Solution:** This requires Azure AD Premium P1 or P2 license  
**Lesson:** Some features require premium licensing - check requirements first

---

## Commands Reference

While this lab used the Azure Portal, here are equivalent PowerShell/CLI commands for future reference:

### PowerShell
```powershell
# Connect to Azure AD
Connect-AzureAD

# Create a new user
New-AzureADUser -DisplayName "az104-user1" -UserPrincipalName "az104-user1@yourtenant.onmicrosoft.com" -AccountEnabled $true -MailNickName "az104-user1"

# Create a new group
New-AzureADGroup -DisplayName "IT Lab Administrators" -MailEnabled $false -SecurityEnabled $true -MailNickName "ITLabAdmins"

# Add user to group
Add-AzureADGroupMember -ObjectId <GroupObjectId> -RefObjectId <UserObjectId>
```

### Azure CLI
```bash
# Create a new user
az ad user create --display-name "az104-user1" --user-principal-name "az104-user1@yourtenant.onmicrosoft.com"

# Create a new group
az ad group create --display-name "IT Lab Administrators" --mail-nickname "ITLabAdmins"

# Add user to group
az ad group member add --group "IT Lab Administrators" --member-id <user-object-id>
```

---

## Related Resources

### Microsoft Learn Modules
- [Understand Microsoft Entra ID](https://learn.microsoft.com/training/modules/understand-azure-active-directory/)
- [Create Azure users and groups](https://learn.microsoft.com/training/modules/create-users-and-groups-in-azure-active-directory/)
- [Allow users to reset their password](https://learn.microsoft.com/training/modules/allow-users-reset-their-password/)

### Official Documentation
- [What is Microsoft Entra ID?](https://learn.microsoft.com/entra/fundamentals/whatis)
- [Add or delete users](https://learn.microsoft.com/entra/fundamentals/add-users)
- [Create a basic group and add members](https://learn.microsoft.com/entra/fundamentals/groups-view-azure-portal)

### Demo Reference
- See `Demos/Demo01/` for quick walkthrough version

---

## Next Steps

Now that I've completed Lab 01, I'm ready to:

- [ ] **Lab 02a** — Manage Subscriptions and RBAC (assign roles to the groups I created)
- [ ] **Lab 02b** — Manage Governance via Azure Policy (apply policies to resources)
- [ ] Review Dynamic Group membership in Microsoft Learn
- [ ] Practice creating users and groups via PowerShell/CLI
- [ ] Explore Entra ID Premium features (if available)

---

## Personal Notes

**What went well:**
- [Add your reflections on what was easy or intuitive]
- [Example: "Creating users was straightforward, portal UI is very clear"]

**What was challenging:**
- [Add what you struggled with]
- [Example: "Understanding the difference between Security and Microsoft 365 groups"]

**Time taken:**
- **Estimated:** 30 minutes
- **Actual:** [Your actual time]

**Would I do differently next time:**
- [Add lessons learned]
- [Example: "Take screenshots as I go instead of at the end"]

---

## Certification Alignment

This lab covers AZ-104 exam objectives:

**Manage Azure identities and governance (20-25%)**
- ✅ Manage Microsoft Entra users and groups
  - Create users and groups
  - Manage user and group properties
  - Manage licenses in Microsoft Entra ID
  - Configure self-service password reset

---

## Lab Files

```
Lab01/
├── README.md                           # This file
├── Lab01_Azure_Entra_ID_Guide.docx    # Detailed step-by-step guide
└── screenshots/
    ├── 01_entra_id_overview.png
    ├── 02_user1_created.png
    ├── 03_both_users_created.png
    ├── 04_group_members.png
    ├── 05_group_owners.png
    ├── 06_demo_tenant_info.png
    ├── 07_demo_user_profile.png
    └── 08_demo_group_detail.png
```

---

**Lab Completed:** ✅  
**Screenshots Uploaded:** ✅  
**Documentation Complete:** ✅  
**Ready for Review:** ✅
