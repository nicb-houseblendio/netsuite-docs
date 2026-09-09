---
id: "bridgehead_N2839850"
type: "bridgehead"
title: "Note about Custom Transaction Line Field Sourcing"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Setting Sourcing Criteria > Note about Custom Transaction Line Field Sourcing"
parent: "section_N2839623"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2839850.html"
anchors: []
sha256: "27c342612b99d30a05db9aa7efd8799fdcd789b3a39f4b9700b1b9bfb8d29c61"
---

Before Version 2012.2, you could source a custom transaction line field's values from a body field by selecting <Record\_Name> (Line) in the Source List list on the Sourcing & Filtering subtab of the Transaction Line Field page. Now, to source a field's values from a body field, you need to select <Record\_Name> in the list. If you select <Record\_Name> (Line), sourcing is from a field in the sublist and if the field doesn't exist, values for the sourced custom transaction line field are blank.

For example, let's say you have a custom field on the Items sublist of Sales Order records. Because the sublist doesn't have a Customer field, selecting Customer (Line) for the new custom field will result in blank values. But if you select Customer, the new custom field's values are sourced from the Customer body field on Sales Orders.

![Transaction Column Field page with custom field applied to the Items sublist on Sale Order records.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustFieldSourcing.png)

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
-   [Setting Sourcing and Filtering Criteria for a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1024121621.html)
-   [Custom Fields Sourcing Videos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1024122002.html)
-   [Troubleshooting Common Sourcing Issues](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0709095341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
