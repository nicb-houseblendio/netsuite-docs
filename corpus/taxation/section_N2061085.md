---
id: "section_N2061085"
type: "section"
title: "Granting Access to the Manage Tax Reporting Page"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports > Granting Access to the Manage Tax Reporting Page"
parent: "section_N2054151"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061085.html"
anchors: ["procedure_N2061093"]
sha256: "7f56877914a87ceae35ba273a30c7ddcd2fddef52a557685efcff65c0129f37f"
---

The following table lists the script deployments you need to add to your roles to grant access to the Manage Tax Reporting page.

| Deployment ID |
| --- |
| customdeploy\_tax\_return\_setup |
| customdeploy\_tax\_return\_inactivate\_notc |
| customdeploy\_tax\_return\_add\_default\_notc |

#### To grant access to script deployments for the Manage Tax Reporting page: {#procedure_N2061093}

1.  Go to Customization > Scripting > Script Deployments.
    
2.  Locate the required script deployment based on the table on this page and click **Edit**.
    
    1.  On the **Audience** tab of each script deployment, select the roles that you want to give access to.
        
        Important:
        
        Only give access to roles. Don't select subsidiaries, departments, employees, groups, or partners.
        
    2.  Click **Save**.
        

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
