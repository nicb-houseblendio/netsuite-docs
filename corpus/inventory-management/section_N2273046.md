---
id: "section_N2273046"
type: "section"
title: "Enabling Bin Management Features"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Enabling Bin Management Features"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html"
anchors: ["subsect_0419103326", "subsect_0419103450"]
sha256: "37184979fe68ba11e7bf306501e92bf63269cdeeeb132a54ec2f2c439cbe49f3"
---

You can enable features for basic or advanced bin management, depending on your inventory requirements.

## Prerequisites {#subsect_0419103326}

Before you can enable features for Bin Management, make sure that you enable the Inventory feature. To use Advanced Bin/Inventory Management to track bins for lot or serialized items, make sure that you enable the Lot Tracking or Serialized Inventory features, respectively.

Warning:

If you use SuiteScript in conjunction with the basic Bin Management feature, note the following. These scripts will no longer function after you enable the Advanced Bin / Numbered Inventory Management feature. To learn more, see [Creating an Inventory Detail Subrecord Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675625458.html#subsect_1517632031).

## Upgrading to Advanced Bin Management {#subsect_0419103450}

After you enable Advanced Bin Management, any item that is lot or serial numbered and uses bins is not placed in a bin. These items must be manually reassigned to a designated bin using a bin putaway worksheet. To learn more, see [Updating Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2277819.html).

Warning:

If you also use both the Lot Tracking and Serialized Inventory features, perform a bin management upgrade immediately after you enable the Advanced Bin / Numbered Inventory Management feature.

You should update related SOAP web services code when you enable Advanced Bin/Numbered Inventory Management. To learn more, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

#### To enable Bin Management features:

1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
    
2.  Click the **Items & Inventory** subtab.
    
3.  Before you can enable Bin Management, make sure that you check the **Inventory** box.
    
4.  To enable basic or advanced Bin Management, check the **Bin Management** box.
    
5.  To enable advanced Bin Management, check the **Advanced Bin/Numbered Inventory Management** box.
    
    If you have existing lot or serialized items prior to upgrading to Advanced Bin/Numbered Inventory Management, see [Upgrading to Advanced Bin Management](#subsect_0419103450).
    
6.  Click **Save**.
    

### Related Topics

-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html)
-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)
-   [Disabling Use Bins Settings and Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0512092419.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
