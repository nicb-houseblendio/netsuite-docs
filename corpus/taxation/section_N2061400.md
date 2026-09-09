---
id: "section_N2061400"
type: "section"
title: "Granting Access to Intrastat Reports"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports > Granting Access to Intrastat Reports"
parent: "section_N2054151"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061400.html"
anchors: ["procedure_N2061433", "procedure_160812803899", "procedure_160812800667", "procedure_N2061624"]
sha256: "3e9d6711521c779f236d8549f93086a1b5c2efdf45bfdac7e7af06bb62ccf957"
---

Important:

Before you give access to Intrastat Reports to a role, ensure that:

-   The role has access to both the subsidiary and its immediate parent subsidiary
    
-   You've already given the role access to scripts for VAT/GST Reporting
    

For more information, see [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html) and [Granting Access to VAT/GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html).

The following section shows the steps you need to complete to grant a role access to Intrastat reports.

#### To grant access to Item Fields for Intrastat reporting: {#procedure_N2061433}

1.  Go to Customization > Lists, Records, & Fields > Item Fields.
    
2.  Click **Commodity Code**.
    
3.  Click the **Access** subtab.
    
4.  Add the custom role.
    
5.  Click **Save**.
    
6.  Click **Nature of Transaction Codes**.
    
7.  Click the **Access** subtab.
    
8.  Add the custom role.
    
9.  Click **Save**.
    

#### To grant access to Transaction Body Fields for Intrastat reporting: {#procedure_160812803899}

1.  Go to Customization > Lists, Records, & Fields > Transaction Body Fields.
    
2.  Click **Delivery Terms**.
    
3.  Click the **Access** subtab.
    
4.  Add the custom role.
    
5.  Click **Save**.
    

#### To grant access to Transaction Column Fields for Intrastat reporting: {#procedure_160812800667}

1.  Go to Customization > Lists, Records, & Fields > Transaction Column Fields.
    
2.  Click **NoTC**.
    
3.  Click the **Access** subtab.
    
4.  Click **Save**.
    

#### To grant access to script deployments for Intrastat reporting: {#procedure_N2061624}

1.  Go to Customization > Scripting > Script Deployments.
    
2.  Click the **Edit** link of the following script deployment used for Intrastat reporting:
    
    -   customdeploy\_itr\_intrastat
        
3.  On the **Audience** tab of the script deployment, select the roles that you want to give access to.
    
    Important:
    
    Only give access to roles. Don't select subsidiaries, departments, employees, groups, or partners.
    
4.  Click **Save**.
    

### Related Topics

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Defining Script Audience](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999041.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [International Tax Reports Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054820.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Installing and Setting Up International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051712.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
