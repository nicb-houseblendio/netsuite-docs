---
id: "section_N2074456"
type: "section"
title: "Creating or Customizing Roles to Use Tax Audit Files"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Tax Audit Files > Creating or Customizing Roles to Use Tax Audit Files"
parent: "chapter_N2073244"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074456.html"
anchors: ["bridgehead_N2074480", "procedure_N2074488", "bridgehead_N2076856", "procedure_N2076864"]
sha256: "89d3ffd794bdf3b0b2a581cc3af5a4f45f725d7b1d0317e53db1788ed52cfc2e"
---

Important:

Tax Audit Files SuiteApp isn't compatible with the SuiteTax feature. If the SuiteTax feature is enabled in your NetSuite account, please don't install this SuiteApp.

The tax audit files require access to all transaction data from NetSuite. Only an administrator or someone with full permission over transaction records can use the tax audit file reporting features.

The Tax Audit Files Accountant and Tax Audit Files CFO custom roles are added automatically when you install the SuiteApp. With these roles, you can:

-   Have automatic access to the Tax Audit Files Suitelets and records
    
-   Assign roles to users
    
-   Create or customize any role to use the tax audit file reporting features
    

To create or customize a role for tax audit file reporting, you'll need to add permissions and give the roles access to the required script deployments.

## Adding Permissions to Custom Roles for Tax Audit Files {#bridgehead_N2074480}

#### To add permissions to a custom role: {#procedure_N2074488}

1.  Go to Setup > Users/Roles > Manage Roles.
    
2.  Click Customize or Edit to update a role.
    
3.  Click the **New Role** button to create a new role.
    
4.  Enter the following information for the role:
    
    1.  **Name**: Enter a new name for the role.
        
    2.  Select a Center Type (for new roles only).
        
5.  You set the following restrictions:
    
    1.  For OneWorld accounts - Restrict access to subsidiaries.
        
    2.  Employee restrictions - You can use the Employee Restrictions dropdown list to select from the following restriction types:
        
        -   None - no default
            
        -   None - default to own
            
        -   Own, subordinate, and unassigned
            
        -   Own and subordinates only
            
    3.  Click the **Restrictions** subtab to set department, class, and location restrictions.
        
6.  Set any other restrictions you want to apply to the role (Issue role, Web Services Only role, IP address).
    
7.  Click the **Permissions** subtab to set the following permissions for the role on Transactions, Reports, Lists, Setup, and Custom Records:
    
    | Subtab | Permission | Level | Comments |
    | --- | --- | --- | --- |
    | Transactions | Find Transaction | Full | Required |
    | Lists | Subsidiaries | View | This is only necessary if you're using a OneWorld account |
    | Lists | Tax Items | View | Required |
    | Setup | Manage Accounting Periods | Full | Required |
    | Setup | Manage Tax Reporting Periods | Full | Required |
    | Setup | Set Up Company | Full | Required |
    | Custom Records | Record: 4599 Custom Record | Full | Required |
    | Custom Records | Record: 4599 System Note | Full | Required |
    
8.  Click the **Forms** subtab to set default forms and restrictions for the role.
    
9.  Click the **Searches** subtab to set search defaults for the role.
    
10.  Click the **Dashboard** subtab to select a dashboard to for the role.
     
11.  Click **Save**.
     

## Granting Access to Scripts for Tax Audit Files {#bridgehead_N2076856}

#### To grant access to script deployments for Tax Audit Files: {#procedure_N2076864}

1.  Go to Customization > Scripting > Script Deployments.
    
2.  Click the Edit link of the following scripts:
    
    | Purpose | Script Deployment Name | Deployment ID | Execute As Role |
    | --- | --- | --- | --- |
    | To use Tax Audit Files features | Tax Audit Files Suitelet | customdeploy\_4599\_main\_s | Administrator |
    | To grant access to custom roles | Tax Audit Files Filter | customdeploy\_taf\_filter | Current Role |
    
3.  On the Audience tab, select the roles you want to give access to.
    
4.  Refer to the previous table to set the appropriate value for the **Execute As Role** field.
    
5.  Click **Save**.
    

### Related Topics

-   [Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2073244.html)
-   [Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2074100.html)
-   [Prerequisites for Installing the Tax Audit Files SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_98164624128.html)
-   [Setting Up Tax Audit Files to Use Multiple Queues or Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4361709092.html)
-   [Setting Up Threshold Configuration on Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1516603486.html)
-   [Setting Tax Audit Files Report Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158080650603.html)
-   [Using Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2077183.html)
-   [France Fichier d'Ecritures Comptables (FEC)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3929748561.html)
-   [Germany GoBD Data Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3838969498.html)
-   [Malaysia GST Audit File (GAF)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4228553324.html)
-   [Mexico DIOT File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1941830.html)
-   [Mexico Electronic Accounting File (Mexico Compliance SuiteApp)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4219758919.html)
-   [Philippines Tax Audit Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1967465.html)
-   [Portugal Standard Audit File for Tax Purposes (PT SAF-T)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1971159.html)
-   [Singapore Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1989169.html)
-   [United Arab Emirates Tax Audit File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539749458.html)
-   [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
