---
id: "bridgehead_N1822423"
type: "bridgehead"
title: "Applying VAT Before or After Discounts"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Applying Sales Tax or VAT to Discount Items > Applying VAT Before or After Discounts"
parent: "section_N1817936"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html"
anchors: ["bridgehead_1504077343"]
sha256: "a0fa5b03178a12a218d8183a53bb489ebdbec8b6c9932eb89f1c0acb100bc987"
---

On a discount item in a OneWorld account with a U.S. base subsidiary, NetSuite always applies VAT after applying the discount for transactions in non-U.S. nexuses. The system does this even if you disable the Apply Before Sales Tax preference on the discount item record. Also Apply Before Sales Tax preference has no effect with per-line taxes on. If a discount is used on line level, Tax Code for it is determined based on its Tax Schedule, for example, the Apply Before Sales Tax preference is relevant when the discount is used on transaction level (Discount Item field).

Note that the U.K. edition and other non-OneWorld editions (except U.S.) don't have the Apply Before Sales Tax box. This is because countries that use VAT/GST always apply the discount before tax.

## Respect Discount Item Tax Preference {#bridgehead_1504077343}

Important:

The following section is intended for Brazil, China, and India

The Set Up Taxes page for Brazil, China, and India (either in a OneWorld or non-OneWorld account) has the Respect Discount Item Tax Preference option, but it isn't enabled by default. To define a discount item as not taxable, you must enable the Respect Discount Item Tax Preference option on the Set Up Taxes page for the nexus, and disable the Apply Before Sales Tax preference on the discount item record. This will ensure that NetSuite applies the tax before applying the discount. If you have a Brazil, China, or India nexus, you must review your Set Up Taxes page and your discount item records, and make sure you have set up the correct tax calculation preference.

**Example: Calculate tax before discounts are applied**

The following example shows the steps to define a discount item as **not taxable**, so that on a transaction for this discount item, NetSuite will calculate tax before applying the discount.

1.  On the Set Up Taxes page for Brazil, China, or India, check the **Respect Discount Item Tax Preference** box.
    
2.  On the Discount Item record, clear the **Apply Before Sales Tax** box on the Accounting subtab.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Applying Sales Tax or VAT to Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817936.html)
-   [Applying Sales Tax to Discount Items (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818019.html)
-   [Discount Methods (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818089.html)
-   [Discount Methods (VAT Nexuses)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1821386.html)
-   [Recording VAT on Prompt Payment Discounts on Sales Invoices for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225129843.html)
-   [Recording VAT on Prompt Payment Discounts on Purchases for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225131687.html)
-   [Taxing Transactions with a Contingent/Volume Discount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029417.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
