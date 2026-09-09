---
id: "section_N2061855"
type: "section"
title: "Granting Access to EU Sales Lists"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports > Granting Access to EU Sales Lists"
parent: "section_N2054151"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2061855.html"
anchors: ["procedure_N2061879"]
sha256: "fa78a498c00a966633f8d6b6a25921032b85815b4b666db60961ca655823e7e1"
---

Important:

Before granting access to EU Sales Lists, you must first grant access to scripts for VAT/GST Reporting. See [Granting Access to VAT/GST Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html).

The following table lists the script deployments you need to add to your roles to grant access to generate and export EU sales list reports.

| Purpose | Script | Deployment ID |
| --- | --- | --- |
| To access the EU Sales List Report page | EU Sales List Report | customdeploy\_new\_ec\_sales\_listdisp |
| To display the ESL audit trail details | ESL Audit Trail Details - UE | customdeploy\_eslauditlock\_error\_ue2 |
| To display the ESL audit trail summary | UK ESL Audit Trail Restrict Edit - UE | customdeploy\_eslauditlock\_error\_ue |

#### To grant access to EU Sales List reports: {#procedure_N2061879}

1.  Go to Customization > Scripting > Script Deployments.
    
2.  Locate the required script based on the table on this page and click **Edit**.
    
    1.  On the **Audience** tab of each script deployment, select the roles that you want to give access to.
        
        Important:
        
        Only roles should be given access. Don't select subsidiaries, departments, employees, groups, or partners.
        
    2.  Click **Save**.
        

**Script Deployment Type: User Event**

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
