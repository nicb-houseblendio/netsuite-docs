---
id: "section_N2060150"
type: "section"
title: "Granting Access to VAT/GST Reporting"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > Creating or Customizing Roles to Use the International Tax Reports > Granting Access to VAT/GST Reporting"
parent: "section_N2054151"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2060150.html"
anchors: ["procedure_N2060158"]
sha256: "b94f298d67fbcc42714af8393528aebe824a0536b13c0046d6cf927e4ae75378"
---

The following table lists the script deployments you need to add to your roles to grant access to VAT/GST reports.

| Purpose | Script Deployment Name (Suitelet) | Deployment ID |
| --- | --- | --- |
| To filter subsidiaries | Tax Report Subsidiary Filter | customdeploy\_vat\_filter |
| To access the country-specific tax forms | Tax Reporting Main | customdeploy\_vat\_ui |
| To export VAT reports | Tax Reporting Main | customdeploy\_vat\_export |
| To print VAT reports | Tax Reporting Main | customdeploy\_vat\_printing |
| To submit the UK VAT 100 report online | 3127 GB Online Filing | customdeploy\_3127\_submit\_online |
| To digitally submit and retrieve the UK VAT100 through MTD | Online Filing Runner Suitelet Online Filing Suitelet Authorization Suitelet | customdeploy\_online\_filing\_runner\_su customdeploy\_online\_filing\_su customdeploy\_authorization\_su |
| To submit the United Kingdom VAT100 in a CSV file | Online Filing Import Suitelet | customdeploy\_online\_filing\_import\_su |

#### To grant access to script deployments for international VAT/GST reporting: {#procedure_N2060158}

1.  Go to Customization > Scripting > Script Deployments.
    
2.  Locate the required script deployment based on the table on this page and click **Edit**.
    
    1.  On the **Audience** tab of each script deployment, select the roles that you want to give access to.
        
        Important:
        
        Only give access to roles. Don't select subsidiaries, departments, employees, groups, or partners.
        
    2.  Click **Save**.
        
        **Script Deployment Type: Suitelet**
        

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
