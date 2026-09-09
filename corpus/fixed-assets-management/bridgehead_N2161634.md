---
id: "bridgehead_N2161634"
type: "bridgehead"
title: "Transferring Assets Across Asset Types"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Managing Assets > Asset Transfer > Transferring Assets Across Asset Types"
parent: "section_N2161434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2161634.html"
anchors: []
sha256: "1cf047227121317e114d941e0b308e3e3681027c6b5258db5ae13a12711cc6f9"
---

Changing the asset type also updates the general ledger asset, depreciation account assignments, and asset life. The last posted amounts for the current cost and cumulative depreciation are carried over from the old to the new accounts through sale and reversal transactions. The asset inherits the asset life of the new asset type.

The system tracks historical records of asset activities for both the accounting and alternate/tax methods.

Tax methods with accounting book values on the original asset type must exist on the default alternate depreciation list of the destination asset type. Otherwise, the transfer won't be processed. See the following example:

| **Original Asset Type** | **Accounting Book** | **Alternate Depreciation** |
| --- | --- | --- |
| Secondary Book | Depreciation Method 8 |
| Secondary Book | Depreciation Method 9 |
| Empty | Depreciation Method 9 |

| **Destination Asset Type** | **Accounting Book** | **Alternate Depreciation** |
| --- | --- | --- |
| Secondary Book | Depreciation Method 8 |
| Secondary Book | Depreciation Method 9 |

Note:

In the previous example, the original asset type's third alternate method (with no accounting book) also transfers to the destination asset type.

### Related Topics

-   [Asset Transfer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2161434.html)
-   [Transferring an Asset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1202041617.html)
-   [Transferring Multiple Assets through CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1202041510.html)
-   [Transferring Assets Across Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2161496.html)
-   [Transferring Assets Across Classes, Departments, or Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2161600.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
