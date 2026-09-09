---
id: "bridgehead_N2158349"
type: "bridgehead"
title: "Depreciation of Assets with Zero and Negative Costs"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Managing Assets > Asset Depreciation > Depreciation of Assets with Zero and Negative Costs"
parent: "section_N2158182"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2158349.html"
anchors: []
sha256: "22089a5f312c663745bf4268ee75751a8cd88af9ec58414cd804d15db0fd8b5e"
---

The SuiteApp can depreciate assets with zero and negative costs, provided the combination of the affected asset costs is any of the following:

| Original Cost | Current Cost | Residual Value |
| --- | --- | --- |
| Negative | Negative | Negative |
| Negative | Negative | Zero |
| Negative | Zero | Zero |

The minimum Residual Value you can enter is zero. By default, the system uses the absolute value of all negative asset costs. Therefore, depreciation for assets with negative values is calculated using the absolute values of the original and current costs up to zero or absolute Residual Value.

You can enter negative values in asset records if **Allow Negative Asset Cost** is enabled. For more information, see [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html).

Important:

For accounting methods, the system won't depreciate assets with negative costs if **Allow Negative Asset Cost** is turned off. No depreciation history records or journal entries are created. Even if **Allow Negative Asset Cost** is turned off, you may still import negative costs depending on your settings for CSV import. For more information, see [General Guidelines for Importing Fixed Asset Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163350867712.html).

### Related Topics

-   [Asset Depreciation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2158182.html)
-   [Depreciating Assets for the Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1201085716.html)
-   [Generating Depreciation Schedule Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1501564204.html)
-   [Depreciation of Compound Assets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4522209887.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
