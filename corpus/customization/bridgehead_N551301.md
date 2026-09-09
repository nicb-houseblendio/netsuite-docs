---
id: "bridgehead_N551301"
type: "bridgehead"
title: "Filtering and Sorting Bills by Custom On Hold Field Example"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Customizing a Transaction Sublist > Filtering and Sorting Bills by Custom On Hold Field Example"
parent: "section_N551202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N551301.html"
anchors: []
sha256: "58578b144f2e05aa084e7e69a37420f05c87fee9ab4ddebd19b02ead2d1fad69"
---

The example in this topic shows how you can filter and sort transaction sublists using a custom On Hold field for bills. For an overview and general instructions on customizing transaction sublists, see [Customizing a Transaction Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551202.html).

You may want to delay paying bills until certain criteria are met. To identify these bills on the Bill Payments page, you can add a custom **On Hold** field to the bill record. Add this as filter criteria to the Bill Payments page and then sort by the wanted setting to view bills that you must pay versus bills that should wait.

To set up this scenario, create a custom Transaction Body field of the Type Check Box and apply it to purchase records.

![Sample Transaction Body Field page with Type and Purchase settings highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/SortByBillType.png)

After bills are entered, go to the Bill Payments page, click Customize View and then select On Hold on the Additional Filters subtab.

![Sort by bill type example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/SortByBillType2.png)

Add the On Hold field to the Results subtab and save.

![Sample Results subtab highlighting the On Hold field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/SortByBillType3.png)

You can now filter results to display only records that aren't On Hold.

![Sort by bill type example with On Hold filter highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/SortByBillType4.png)

### Related Topics

-   [Customizing a Transaction Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551202.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
