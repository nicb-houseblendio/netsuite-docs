---
id: "bridgehead_N1821386"
type: "bridgehead"
title: "Discount Methods (VAT Nexuses)"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Applying Sales Tax or VAT to Discount Items > Discount Methods (VAT Nexuses)"
parent: "section_N1817936"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1821386.html"
anchors: ["bridgehead_N1821477", "bridgehead_N1822347", "bridgehead_N1822387"]
sha256: "50dbf1bcf9a8677670908340385d19079bae2215f0f30772f9421a107c881d5c"
---

To apply VAT to discount items, you should understand the types of discount methods available in NetSuite and how they will affect your tax calculation.

The following discount methods are available:

-   [Method 1: Applying a Discount to all Items from the Discount Field (U.K. and International Editions)](#bridgehead_N1821477)
    
-   [Method 2: Applying a Discount to a Line Item (U.K. and International Editions)](#bridgehead_N1822347)
    
-   [Method 3: Applying Discount to a Group of Line Items with Subtotal (U.K. and International Editions)](#bridgehead_N1822387)
    

Note:

For countries that have VAT, the discount is **always** be applied before tax and never after. Applying a discount after tax results in incorrect VAT being reported to the tax authorities. The UK edition and International edition non-OneWorld accounts therefore don't have the Apply Before Tax option for discount items. Only Brazil, China, and India nexuses have the option to apply discounts after tax. See [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html).

## Method 1: Applying a Discount to all Items from the Discount Field (U.K. and International Editions) {#bridgehead_N1821477}

You can apply a specific discount percentage or dollar amount by selecting an option from the Discount dropdown list on the Item subtab for the sales order or invoice. The choices available in the Discount dropdown list are based on discount items that have already been created in your account.

When you choose a discount method from the dropdown list, the % or amount of the discount is populated in the **Rate** field and is applied to all items on the sales order or invoice. It is critical to remember that when using this method, the percentage or fixed amount you enter for the discount is always applied to the group of items before tax is applied. In addition, U.K. users should always enter net amounts in the **Discount** field to get the end desired result. If you want to use different tax codes for different line items in the sales order or invoice, you should use [Method 2: Applying a Discount to a Line Item (U.K. and International Editions)](#bridgehead_N1822347).

The following examples show correct tax calculations for discounts applied to all items. The only difference is that Example 1 is based on a percentage (10%) discount, and Example 2 is based on a fixed amount (-112.50) for the discount.

**Example 1: Percentage Discount Applied to all Items (UK and International Editions)**

![Example of applying a discount using the Discount dropdown list](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountPercentUKI18N.png)

**Example of Fixed Amount Discount Applied to All Items (U.K. and International Editions)**

![Example of fixed amount discount applied to all items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountAmountUKI18N.png)

**Calculating Discount Before Tax Versus After Tax (U.K. and International Editions)**

In both examples, you might have expected the price, tax, and overall discount to be greater. This could occur if you incorrectly assume that the discount will be applied after tax.

Table 1 shows the correct calculation of a discount and its ensuing tax as it is applied before tax by NetSuite. Notice that the total amount applied as a discount (132.19) is greater than the original discount amount (112.50) because tax is applied to the amount of the items after the discount is applied.

| Table 1: Correct Calculation of Discount Across All Items |
| --- |
|  | **Net Price** | **Tax** | **Total** |
| **Item 1** | 1000 | 175 | 1175 |
| **Item 2** | 125 | 21.88 | 146.88 |
|  | 1125 | 196.88 | 1321.88 |
| **Discount Field** | 112.50 | 19.69 | 132.19 |
| **Totals** | 1012.50 | 177.19 | 1189.69 |

Table 2 shows **incorrect** application and calculation of discount and tax. The numbers are incorrect because the discount amount has been applied after tax when it should have been applied before tax.

| Table 2: Incorrect Calculation of Discount Across All Items |
| --- |
|  | **Net Price** | **Tax** | **Total** |
| **Item 1** | 1000 | 175 | 1175 |
| **Item 2** | 125 | 21.88 | 146.88 |
|  | 1125 | 196.88 | 1321.88 |
| **Discount Field** | 95.75 | 16.75 | 112.50 |
| **Totals** | 1029.25 | 180.13 | 1209.38 |

## Method 2: Applying a Discount to a Line Item (U.K. and International Editions) {#bridgehead_N1822347}

You can apply a discount amount or percentage for a specific line item on a sales order or invoice. You can accomplish this by adding a discount item directly below the line item that you want the discount to apply to.

When you choose the line item discount method, the discount is applied only to the previous line item on the sales order or invoice. No other line items are affected. If you assign a VAT code to the discount item, the amount of VAT charged to the customer is reduced. You must select and match the discount item's VAT code to the VAT codes for the products or services on the sales order or invoice.

The following screenshot shows a fixed discount applied to the previous line item. The calculations shown are correct but required manual selection of the correct discount and tax rate.

![Example of applying a discount using a discount item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountLineItemsUKI18N.png)

## Method 3: Applying Discount to a Group of Line Items with Subtotal (U.K. and International Editions) {#bridgehead_N1822387}

You can apply a percentage discount to a group of line items on a transaction. You can accomplish this by first creating a subtotal item that contains a set of items. After creating the subtotal item, you then add a discount item as a line item directly below the subtotal item.

If you use this discount method, the discount is applied to all of the items in the subtotal.

Note:

For countries that have VAT, the discount must be applied before tax. Applying a discount after tax results in incorrect VAT being reported to the tax authorities. The UK edition and International edition non-OneWorld accounts therefore don't have the Apply Before Tax option for discount items. Only Brazil, China, and India nexuses have the option to apply discounts after tax. See [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html).

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Applying Sales Tax or VAT to Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817936.html)
-   [Applying Sales Tax to Discount Items (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818019.html)
-   [Discount Methods (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818089.html)
-   [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html)
-   [Recording VAT on Prompt Payment Discounts on Sales Invoices for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225129843.html)
-   [Recording VAT on Prompt Payment Discounts on Purchases for United Kingdom](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4225131687.html)
-   [Taxing Transactions with a Contingent/Volume Discount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2029417.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
