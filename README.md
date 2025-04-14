# Onboard a New User in Azure with Microsoft Entra ID

## Overview

This lab walks through onboarding a new employee in Microsoft Azure by creating a user account in Microsoft Entra ID (formerly Azure Active Directory), assigning licenses, and adding the user to appropriate Microsoft 365 and security groups. This ensures proper identity and access management from day one.

---

## Lab Requirements

- Microsoft Entra ID (Azure AD) admin access
- Microsoft 365 license available for assignment
- Access to Microsoft Entra Admin Center: https://entra.microsoft.com
- Access to Microsoft 365 Admin Center: https://admin.microsoft.com

---

## Who, What, When, Where, Why

- **Who**: Azure administrators or IT support engineers  
- **What**: Onboarding new users with Microsoft Entra ID and Microsoft 365  
- **When**: When a new employee joins the organization  
- **Where**: Microsoft Entra Admin Center and Microsoft 365 Admin Center  
- **Why**: To ensure users are securely onboarded with proper identity and access controls

---

## Steps

### Step 1: Create a New User in Microsoft Entra ID

**Definition**:  
Microsoft Entra ID is Microsoft's cloud-based identity and access management service. It is used to manage users, groups, and access to applications and resources.

1. Go to: https://entra.microsoft.com  
2. In the left pane, select **Users** > **All users**  
3. Click **+ New user**  

![image](https://github.com/user-attachments/assets/197093b3-f8d2-4797-abc6-646b0e305ac9)


4. Under Identity, choose **Create user**  
5. Enter the following:
   - **User name**: `jane.doe@yourdomain.com`
   - **Name**: `Jane Doe`
   - Leave the default auto-generated password or define a temporary one  
6. Click **Create**

![image](https://github.com/user-attachments/assets/b5f60cb9-6214-4ac9-ae8e-66bde74c288c)
![image](https://github.com/user-attachments/assets/2f3deac5-a671-430d-9b79-572c1782970f)

---

### Step 2: Assign a Microsoft 365 License

**Definition**:  
A Microsoft 365 license provides access to cloud productivity tools such as Outlook, Teams, SharePoint, and OneDrive.

1. Go to: https://admin.microsoft.com  
2. In the left pane, select **Users** > **Active users**  
3. Locate and select the new user (`Jane Doe`)  
4. In the user panel, click **Licenses and apps**  
5. Assign a Microsoft 365 license (e.g., Microsoft 365 Business Premium)  
6. Click **Save changes**

![image](https://github.com/user-attachments/assets/21973c10-51be-4e3f-8245-991aa8c42bc5)
![image](https://github.com/user-attachments/assets/e78f7f16-9075-41f8-a1f7-985bdf5ae4bb)
![image](https://github.com/user-attachments/assets/a8987258-8f53-4a16-8aa7-c39f2b9bb381)

---

### Step 3: Add the User to Microsoft 365 and Security Groups

**Definition**:  
Groups in Microsoft Entra ID allow administrators to manage permissions and access to resources collectively rather than individually.

1. Go to: https://entra.microsoft.com  
2. In the left pane, select **Groups** > **All groups**  
3. Select an existing group or click **+ New group** to create one  
   - Example: `All Employees`, `HR Department`  
4. Open the group and go to **Members**  

![image](https://github.com/user-attachments/assets/f3efaf59-1c43-4c81-804e-b72a0ab8f535)
![image](https://github.com/user-attachments/assets/a186515b-49b6-4a57-a66e-440f97e78844)


5. Click **+ Add members**  

![image](https://github.com/user-attachments/assets/1430d695-357a-4571-a7ea-7572acce7b1a)

6. Search for and select `Jane Doe`  

![image](https://github.com/user-attachments/assets/d79aca1c-f483-47dd-aa13-1753cb13f9c2)

8. Click **Select**

![image](https://github.com/user-attachments/assets/bcbd8060-83f4-42a4-9b25-b1f6e48fdc5d)
![image](https://github.com/user-attachments/assets/4bcbae01-c5b9-4ef3-bfb3-30bbaa0f99d5)

---

### Step 4: Verify User Sign-In and Access

**Definition**:  
User verification confirms that account setup, licensing, and access permissions have been applied correctly by simulating a real sign-in scenario.

1. Open an incognito/private browser window  
2. Navigate to https://portal.office.com  
3. Sign in using the new account: `jane.doe@yourdomain.com`  

![image](https://github.com/user-attachments/assets/f2a13f58-eebe-4f07-bfec-aa9f79297144)

4. Enter the temporary password and create a new password when prompted  

![image](https://github.com/user-attachments/assets/e38303ff-f041-4ee4-92d2-e8f126dc8b0f)
![image](https://github.com/user-attachments/assets/49677c6a-18ee-439a-b747-32c990a541ee)
![image](https://github.com/user-attachments/assets/59637690-b551-4d6e-93d5-3a410dda5439)

5. Verify access to licensed services (Outlook, Teams, OneDrive)  

![image](https://github.com/user-attachments/assets/9c5880fb-f544-437d-ab4d-216db58c6fb6)
![image](https://github.com/user-attachments/assets/60e3aa49-833a-45e5-94f5-977ce05238ad)

---

## Conclusion

Onboarding a user in Microsoft Entra ID ensures secure access to cloud-based resources and applications from day one. This lab demonstrated how to create a user, assign a license, and add them to the appropriate groups for access management. Proper onboarding practices streamline user access, reduce configuration errors, and strengthen organizational security posture.
