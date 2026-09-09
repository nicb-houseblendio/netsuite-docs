---
id: "section_N1803739"
type: "section"
title: "Enabling Advanced Taxes"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Advanced Taxes > Enabling Advanced Taxes"
parent: "chapter_N1803438"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803739.html"
anchors: ["bridgehead_1544015782", "bridgehead_4552676987", "procedure_N1803880"]
sha256: "92778ea2e8c3a0ac1d3753ac5eb1cecfb387917b2a4cf5cf9d58945b4a4ddbc3"
---

Warning:

If you enable Advanced Taxes, you can't disable it in the future.

When you enable the Advanced Taxes feature, NetSuite makes the following changes in your NetSuite account:

-   NetSuite creates tax schedules for the existing tax codes and tax groups in your account. You can create tax schedules that define how NetSuite calculates and tracks taxes in each nexus at _Setup > Accounting > Taxes > Tax Schedules_.
    
-   You can create nexus records at _Setup > Accounting > Taxes > Nexuses > New_.
    

When you select a customer on a transaction form, the form changes to show the appropriate tax fields for the nexus in which the customer is located, based on the customer's shipping address.

Important:

If you have custom transaction forms that use SuiteScript, using the Advanced Taxes feature may affect your forms. You should test your transaction forms for errors when you enable this feature.

## Consistent Custom Field Labels Required {#bridgehead_1544015782}

The Advanced Taxes feature requires all custom field labels to match across all forms. Otherwise, a warning appears after you try enabling the feature.

If you enable Advanced Taxes, the non-matching labels are replaced with default system values. To customize the labels, go to _Setup > Accounting > Taxes > Setup Taxes_, and then click the **Field Naming** subtab.

**For U.S. edition (not OneWorld):**

-   Without Advanced Taxes, you can add other U.S. states only.
    
-   With Advanced Taxes enabled, you can add U.S. states and Canadian provinces.
    

**For Canada edition (not OneWorld):**

-   Without Advanced Taxes, you can add other Canadian provinces only.
    
-   With Advanced Taxes enabled, you can add Canadian provinces and U.S. states.
    

**For OneWorld accounts** (any edition), the Advanced Taxes feature is enabled by default, and you can add different country nexuses.

## Enabling Advanced Taxes When Tax Inclusive Pricing is Enabled {#bridgehead_4552676987}

When you enable Advanced Taxes in an account that has items with tax inclusive pricing, those item prices will be treated as tax exclusive prices. If you choose to enable Advanced Taxes, be sure to disable tax inclusive pricing, and update the prices for those items using the mass update feature.

#### To enable Advanced Taxes: {#procedure_N1803880}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Tax** subtab.
    
3.  In the Tax & Compliance section, check the **Advanced Taxes** box.
    
4.  Click **Save**.
    

### Related Topics

-   [Creating Tax Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804264.html)
-   [Nexuses and Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804037.html)
-   [Creating Tax Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804737.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)
-   [General International Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1813074.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
