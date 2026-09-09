---
id: "section_N1937177"
type: "section"
title: "Selecting Precision Settings - Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Tax Topics > Selecting Precision Settings - Japan"
parent: "chapter_N1934076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937177.html"
anchors: []
sha256: "9b8fc54173747068479bb7aba156c2466f7f91219b6d44c674e1fab3dbfc24b8"
---

You can select the level of tax rounding precision at the company level, or set it for each customer or vendor individually.

On the Set Up Taxes page, if the **Allow override rounding setting per Entity box** isn't checked, tax amounts will follow the tax rounding method and precision defined for the country nexus, no matter what tax rounding method and precision have been set for customers and vendors. If tax rounding preferences aren't defined on the entity record, the system uses the preferences defined for the country nexus.

You must enter the gross amount first, to get the correct tax calculation logic. Then, set the tax rounding method. The selected rounding method is applied to all amounts, the inputs and output. Because of the rounding method, the tax amount based on net amount will differ with that based on gross amount.

**Example of Tax Rounding Precision Settings and Computation**

If,

Tax Rounding Precision = 1 and below;

Tax Rounding Method = Round Down; and

Tax Rate = 8%.

Then, with net amount as source: 95 \* 1.08 = 102.6 ; rounded down to 102.

The tax amount is calculated as 102 - 95 = 7.

And, with gross amount as source: 102 / 1.08 = 94.4444... ; rounded down to 94.

The tax amount is calculated as 102 - 94 = 8.

The table shows another example of consumption tax amount resulting from a selected rounding precision, if the selected rounding method is round down.

If an item is priced at ¥73,489, the consumption tax on the item is ¥3674.45.

| Rounding Precision | Consumption Tax Amount |
| --- | --- |
| 1 and Below | ¥3,674 |
| 10 and Below | ¥3,670 |
| 100 and Below | ¥3,600 |

### Related Topics

-   [Setting Tax Rounding Methods - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1935242.html)
-   [Setting Tax Rounding Preferences for a Customer or Vendor - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937473.html)
-   [Japan Consumption Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1934460.html)
-   [Setting Up Consumption Tax - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1934652.html)
-   [Japan Consumption Tax Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937672.html)
-   [Deductible Purchase Tax for Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937846.html)
-   [Japan Consumption Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1565781755.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1803438.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
