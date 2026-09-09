---
id: "section_N2158182"
type: "section"
title: "Asset Depreciation"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Managing Assets > Asset Depreciation"
parent: "chapter_N2157855"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2158182.html"
anchors: []
sha256: "bc00060ab25fb626f7122d2e0acd6d11e80737bf0cd2a584360397c0742151ce"
---

Note:

In the latest Fixed Assets Management version, custom journals don't work with Multi-book accounting.

Use Asset Depreciation to run first time depreciation or to depreciate assets after you revise their method or period.

You can run depreciation periodically for a single or several asset types. This procedure is run to depreciate assets for the next period. The SuiteApp decides which assets require depreciation by checking the depreciation start date, last depreciation period, and depreciation rules. When it posts the depreciation values, the system creates a batch of GL journal entries.

An asset depreciates for each period (set on the depreciation method) up to the date entered on the Depreciate Assets page.

For example, if an asset depreciates monthly and the last depreciation is in January,a depreciation run in June processes depreciation for February through June.

Note:

Depreciation stops when the last depreciation period is reached for both the accounting and alternate/tax methods assigned to the asset.

Important:

If you enabled the accounting preferences **Make Departments Mandatory**, **Make Classes Mandatory**, and **Make Locations Mandatory**, but the asset's department, class, or location is not set, the system won't process the depreciation. No depreciation history records or journal entries will be created.

### Related Topics

-   [Managing Assets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2157855.html)
-   [Depreciating Assets for the Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1201085716.html)
-   [Generating Depreciation Schedule Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1501564204.html)
-   [Depreciation of Compound Assets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4522209887.html)
-   [Depreciation of Assets with Zero and Negative Costs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2158349.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
