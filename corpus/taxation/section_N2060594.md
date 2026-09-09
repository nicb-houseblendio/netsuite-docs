---
id: "section_N2060594"
type: "section"
title: "Granting Access to Sales and Purchase Reports Grouped by Tax Code"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports > Granting Access to Sales and Purchase Reports Grouped by Tax Code"
parent: "section_N2054151"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060594.html"
anchors: ["procedure_N2060618"]
sha256: "910b4124cb5cd13102fa4bb43b4808cf05ebbb696d26e3c1f763d715bb870dc7"
---

The following table lists the script deployments you need to add to your roles to grant access to sales and purchase reports by tax code.

Important:

For any custom role you create in NetSuite OneWorld, make sure you give the role access to all the sales and purchase reports provided by the International Tax Reports SuiteApp. The reports are filtered by subsidiary, so when you go to the Reports menu in NetSuite, you'll only see reports for the subsidiaries you have access to. For information about these reports, see [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html).

| Purpose | Script Deployment Name (Suitelet) | Deployment ID |
| --- | --- | --- |
| To dispatch the VAT saved reports | VAT Saved Report Dispatcher | customdeploy\_4110\_report\_dispatcher |
| To generate the Purchases By Tax Code (Details) | Report Dispatcher Filter | customdeploy\_4110\_vat\_purchase\_detail |
| To generate the Purchases By Tax Code (Summary) | Report Dispatcher Filter | customdeploy\_4110\_vat\_purchase\_summary |
| To generate the Sales By Tax Code (Details) | Report Dispatcher Filter | customdeploy\_4110\_vat\_sales\_detail |
| To generate the Sales By Tax Code (Summary) | Report Dispatcher Filter | customdeploy\_4110\_vat\_sales\_summary |

#### To grant access to script deployments for sales and purchase reports by tax code: {#procedure_N2060618}

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
