---
id: "section_N1935242"
type: "section"
title: "Setting Tax Rounding Methods - Japan"
branch: "japan-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Japan Help Topics > Japan Tax Topics > Setting Tax Rounding Methods - Japan"
parent: "chapter_N1934076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1935242.html"
anchors: []
sha256: "faa889458d10fba3cb6dc6c003badf7b2af6fdf189121c138314503121120df7"
---

You can select a tax rounding method at the company level, or set it for each customer or vendor individually.

On the Set Up Taxes page, if the **Allow override rounding setting per Entity box** isn't checked, tax amounts will follow the tax rounding method and precision defined for the country nexus, no matter what tax rounding method and precision have been set for customers and vendors. If tax rounding preferences aren't defined on the entity record, the system uses the preferences defined for the country nexus.

You must enter the gross amount first, to get the correct tax calculation logic. Then, set the tax rounding method. The selected rounding method is applied to all amounts, the inputs and output. Because of the rounding method, the tax amount based on net amount will differ with that based on gross amount.

**Example of Rounding Methods**

The table shows the consumption tax amount corresponding the rounding method selected.

If an item is priced at ¥893, the consumption tax on the item is ¥44.65.

| Rounding Method | Consumption Tax Amount |
| --- | --- |
| Round Off | ¥45 |
| Round Down | ¥44 |
| Round Up | ¥45 |

### Related Topics

-   [Selecting Precision Settings - Japan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1937177.html)
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
