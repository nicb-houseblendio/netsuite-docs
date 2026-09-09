---
id: "section_N1865357"
type: "section"
title: "Chile Tax Setup"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Chile Tax Topics > Chile Tax Setup"
parent: "chapter_N1865199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1865357.html"
anchors: ["bridgehead_N1865378", "bridgehead_N1865521"]
sha256: "856be71407ed2bcb0ff7a39a2391e5350c981414fe845d48f48083265490b4ee"
---

Following are the settings required to enable NetSuite to correctly generate the Chile tax reports provided by the International Tax Reports SuiteApp.

## Chile Tax Control Accounts {#bridgehead_N1865378}

Tax control accounts are automatically created upon creation of a Chile nexus. Go to Setup > Accounting > Taxes > Tax Control Accounts and make sure that you have the following tax control accounts:

| Tax Control Account Name | Tax Account Type |
| --- | --- |
| VAT on Sales CL | Sale |
| VAT on Purchases CL | Purchase |
| VAT Liability CL | Sale |

## Chile Tax Types {#bridgehead_N1865521}

Tax types are automatically created upon creation of a Chile nexus. Go to Setup > Accounting > Tax Types and make sure that you have the following tax type:

| Tax Type | Liability/Sales Tax Account Type | Asset/Purchase Tax Account Type |
| --- | --- | --- |
| IVA\_CL | VAT on Sales CL | VAT on Purchases CL |

For information about required tax codes for Chile, see [Chile Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1865743.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Chile Tax Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1865357.html)
-   [Chile VAT Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1867667.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
