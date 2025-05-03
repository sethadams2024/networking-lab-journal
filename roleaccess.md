# Role-Based Access Control (RBAC) Documentation

## Table of Contents
- Introduction
- Folder Setup
- Permissions Breakdown
- IT-Only Folder
- User Folders
- Setting Permissions
- Testing Access
- Simulating Active Directory Environment

## Introduction

This document outlines the process of setting up access control on a local PC to simulate role-based access and restricted user permissions. The goal is to understand how to manage user access and apply permissions in a typical corporate environment.

In this setup:
- **ITadmin** (administrator) has full access to all folders.
- **Corporate users** have access to their own designated folders and are restricted from accessing other users' folders.

## Folder Setup

The folder structure on the machine is as follows:

C:\CorpShared


IT ONLY # Accessible only by ITadmin

AND

DeptA # Department folder, contains user-specific subfolders

    Corp_user1 # Accessible only by corp_user1 and ITadmin
    
    Corp_user2 # Accessible only by corp_user2 and ITadmin
    
    Corp_user3 # Accessible only by corp_user3 and ITadmin



### Folder Breakdown:
- **IT ONLY Folder**: A folder exclusively for the ITadmin to store system-related tools and data.
- **DeptA Folder**: A department-specific folder that contains subfolders for each user. These subfolders are **private** to each user but accessible by ITadmin.

## Permissions Breakdown

Permissions were configured using **NTFS** permissions, giving different access levels to various users.


1. **IT ONLY Folder**:
   - **Users**: Only **ITadmin** has full access (read/write/modify).

2. **DeptA Folder**:
   - **User1's Folder**: Accessible only by **User1** and **ITadmin**.
   - **User2's Folder**: Accessible only by **User2** and **ITadmin**.
   - **User3's Folder**: Accessible only by **User3** and **ITadmin**.

## IT-Only Folder

The `IT ONLY` folder is designated for administrative use only, and its access is strictly limited to the **ITadmin** account. This folder is used to store system tools, logs, or scripts that should not be accessed by standard users. This is an important practice for maintaining security and ensuring sensitive system data is protected.

### Access Configuration:
- **ITadmin**: Full Control (read, write, modify, delete)
- **Other Users**: No access

## User Folders

Each department or user (in this case, `DeptA`) has its own folder, and inside each department folder, there are subfolders for individual users. Each subfolder is only accessible to the specific user and **ITadmin**, ensuring that users can’t access each other's files.

### User Folder Permissions:
- **Corp_user1's Folder**: Only **Corp_user1** and **ITadmin** can access.
- **Corp_user2's Folder**: Only **Corp_user2** and **ITadmin** can access.
- **Corp_user3's Folder**: Only **Corp_user3** and **ITadmin** can access.

## Setting Permissions

To set up these permissions, follow the process:

1. **Create the Folders**:
   - Right-click in **C:\CorpShared**, select **New > Folder**, and name the folders according to the structure above.
  
2. **Modify Permissions for Each Folder**:
   - Right-click on the folder (e.g., `DeptA`), go to **Properties > Security**.
   - Click on **Edit**, then **Add** users (`ITadmin`, `Corp_user1`, etc.).
   - Set permissions based on role:
     - **Full Control** for ITadmin.
     - **Read/Write** for the respective user (e.g., `User1`).
     - Remove permissions for all other users (e.g., User2 doesn’t have access to User1’s folder).
   - Click **Apply** and **OK** to save changes.

3. **Break Inheritance**:
   - If needed, disable inheritance on subfolders and set explicit permissions for each user to prevent the propagation of general folder permissions.
  
## Testing Access

Once the permissions are set, it's important to test access to ensure everything is functioning as expected.

1. **Log in as ITadmin** and confirm full access to all folders.
2. **Log in as Corp_user1** and confirm access to `Corp_user1`'s folder, but not `Corp_user2` or `Corp_user3`'s folders.
3. **Log in as Corp_user2** and repeat the access tests.

### Expected Results:
- **ITadmin**: Full access to all folders.
- **Corp_user1**: Access to `Corp_user1`'s folder and `General` folder, no access to other user folders.
- **Corp_user2**: Access to `Corp_user2`'s folder and `General` folder, no access to other user folders.
- **Corp_user3**: Access to `Corp_user3`'s folder and `General` folder, no access to other user folders.

## Problems Encountered and Solutions

### **Access Denied Despite Correct Permissions**
   **Problem**: After setting permissions for certain folders, users were unable to access them, even though it appeared that permissions were correctly configured.

   **Cause**: The issue was likely due to **permission inheritance** settings or conflicts between **Allow** and **Deny** permissions.

   **Solution**:
   - **Disable Inheritance**: When dealing with subfolders, sometimes inheritance needs to be disabled so that explicit permissions are set. To disable inheritance, go to **Properties > Security > Advanced**, then click **Disable inheritance**.
   - **Ensure No Deny Permissions**: Double-check that there are no **Deny** entries in the permissions, as they take precedence over **Allow** permissions.
   - **Apply Permissions Recursively**: Make sure that the permissions are propagated correctly to all subfolders and files by selecting **Apply to this folder, subfolders, and files**.













## Simulating Active Directory Environment

While this setup is done on a **local PC**, it mimics the kind of role-based access you would implement in a corporate **Active Directory** environment. In a real-world scenario, these folder permissions would be managed through **Active Directory groups** and **Group Policy Objects (GPOs)**.

- **AD Groups**: Users would be assigned to groups like **DepartmentA**, **IT**, etc.
- **GPOs**: Policies would apply group-wide settings, such as limiting access to control panel, enforcing password policies, or setting up automatic network drive mappings.

---

## Conclusion

This exercise has helped simulate a common **role-based access control (RBAC)** system, where users have permissions based on their roles and need-to-know access. The key takeaway is how important it is to break inheritance and explicitly set permissions in scenarios where different roles require different levels of access. In a real-world corporate environment, this would be managed through Active Directory and Group Policies.
