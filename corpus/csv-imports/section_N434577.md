---
id: "section_N434577"
type: "section"
title: "Using the Inventory Worksheet Import Assistant"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Simple Imports > Single Inventory Worksheet Import > Using the Inventory Worksheet Import Assistant"
parent: "section_N434282"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434577.html"
anchors: []
sha256: "a57d4467547b3bb3f37e4056918e731d7020393cdcd73c7288534788cd2510d8"
---

The Single Inventory Worksheet Import Assistant is available at _Transactions > Inventory > Adjust Inventory Worksheet > Import_, to users who have the required permission. See [Permission for Inventory Worksheet Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434282.html#bridgehead_N434423).

This Import Assistant includes the following steps:

1.  Upload the CSV file that contains your inventory worksheet data.
    
    -   The first page of the Assistant provides a link to a CSV template file. Click this link to download the template file and populate it with your data.
        
        Before you populate your CSV file data, review [Requirements for Inventory Worksheet CSV File Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N435556.html).
        
    -   After you have a CSV file with data in it, click the Select button in the Import Assistant, browse to your file, and click Next.
        
        ![Import Assistant Scan and Upload CSV File page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/InvWorkPage1_2014_2.png)
2.  Review mappings of CSV fields to NetSuite fields and start the import.
    
    ![Import Assistant View Mapping/Start Import page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/InvWorkPage2_2014_2.png)
    -   The Assistant automatically maps fields in your CSV file to NetSuite standard inventory worksheet fields. Header-level fields are listed under Inventory Worksheet; line-level fields are listed under the Inventory Worksheet Adjustments sublist.
        
    -   You can click Run to accept the default mappings and immediately start the import.
        
    -   You can make changes as necessary by dragging and dropping fields to add or subtract them from the import.
        
    -   You can click the edit icon for a field to open a popup where you can set a default value. This option is useful for header-level fields that need to be the same value for each imported line.
        
        For example, in the following screenshot, the CSV file doesn't include a Subsidiary field value, so a default value is set in the popup:
        

![Import Assistant Default Value or Reference Type window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/InvWorkDefault_RefType_2014_2.png)

When you click Run, the import job is processed.

-   If the import was successful, or if there are errors, the Job Status page appears.
    
-   Note that, unlike most other imports, an email notification isn't sent for single inventory worksheet imports.
    

For more information about adjusting inventory, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).

### Related Topics

-   [Single Inventory Worksheet Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N434282.html)
-   [Requirements for Inventory Worksheet CSV File Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N435556.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
