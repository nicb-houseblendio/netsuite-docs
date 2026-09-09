---
id: "bridgehead_N1818089"
type: "bridgehead"
title: "Discount Methods (U.S. and Canada)"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > General International Tax Topics > Applying Sales Tax or VAT to Discount Items > Discount Methods (U.S. and Canada)"
parent: "section_N1817936"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818089.html"
anchors: ["bridgehead_N1818165", "bridgehead_N1818212", "bridgehead_N1819921", "bridgehead_N1819957", "bridgehead_N1821302", "bridgehead_4567397511", "bridgehead_4762637163", "procedure_N1821334"]
sha256: "db084ead0598d98b384149cfe45b462544e8dd4dedf6dc117344c16f11d5e963"
---

The following discount methods are available:

-   [Method 1: Applying a Discount to all Items from the Discount Field (U.S. and Canada Editions)](#bridgehead_N1818165)
    
-   [Method 2: Applying a Discount to a Line Item (U.S. and Canada Editions)](#bridgehead_N1818212)
    
-   [Method 3: Applying a Discount to a Group of Line Items with a Subtotal (U.S. and Canada Editions)](#bridgehead_N1819921)
    

Read [Calculation Logic for Sales Tax on Discount Items](#bridgehead_N1819957) to understand the implications of choosing each of these methods.

## Method 1: Applying a Discount to all Items from the Discount Field (U.S. and Canada Editions) {#bridgehead_N1818165}

You can apply a specific discount percentage or dollar amount by selecting an option from the Discount dropdown list on the Item tab for the Sales Order or Invoice. The choices available in the Discount dropdown list are based on discount items that have already been created in your account.

When you choose a discount method from the dropdown list, the % or amount of the discount is populated in the Rate field and is applied to all items on the sales order or invoice.

![Example of applying a discount using the Discount dropdown list](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountItemsUSCAN.png)

## Method 2: Applying a Discount to a Line Item (U.S. and Canada Editions) {#bridgehead_N1818212}

You can apply a discount amount or percentage for a single line item on a sales order or invoice. You can accomplish this by adding a discount item directly below the line item that you want the discount to apply to.

If you choose this discount method, the discount is applied only to the previous line item on the sales order or invoice. No other line items are affected.

![Example of applying a discount to a line item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountLineItemsUSCAN.png)

## Method 3: Applying a Discount to a Group of Line Items with a Subtotal (U.S. and Canada Editions) {#bridgehead_N1819921}

You can apply a percentage discount to a group of line items on a transaction. You can accomplish this by first creating a subtotal item that contains a set of items. After creating the subtotal item, you then add a discount item as a line item directly below the subtotal item.

![Example of applying a discount to by creating a subtotal item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/DiscountSubtotalItemsUSCAN.png)

If you use this discount method, the discount is applied to all of the items in the subtotal.

## Calculation Logic for Sales Tax on Discount Items {#bridgehead_N1819957}

It is important to understand how using the different discount methods affect your tax calculation. In the screenshots, the items, tax, and value of the discount are the same, but the choice of discount method yielded different tax amounts.

Note:

The following examples are for a discount item with the Apply Before Sales Tax preference enabled.

The following scenarios represent calculations for Methods 1 and 2 with the same items, tax, and discount value. Scenario 1 uses Method 1, which applies a discount amount to all items. Scenario 2 uses Method 2, which applies a line item discount only to the line directly above the discount item. The tax owed ($15.33) for Scenario 1 is correct. However, the tax owed ($15.26) for Scenario 2 is incorrect. This is because Scenario 2 does not take into account the proportion of the discount that should be applied to nontaxable items across the invoice, which affects the amount of tax owed for the items.

**Scenario 1: Discount Rate Across All Items**

If you use Method 1 to apply a discount to all items on a transaction (using the Discount dropdown list as shown in the screenshot), the following calculations will apply:

| Discount to All Items using Discount Field |
| --- |
|  | **Net Price** | **Tax** | **Total** | **Notes** |
| **Taxable Items (96.6% of total)** | $285,00 | 
-   $17.10
-   (6% of $285.00)

 | $302.10 |  |
| **Non Taxable Items (3.4% of total)** | $10.00 | 0.00 |  |  |
| **Subtotal** | **$295.00** | **$17.10** | **$312.10** |  |
|  |  |  |  |  |
| **Taxable discount portion** | 

-   \-$29.56
-   **96.6% of discount amount ($30.60) applied for taxable items**

 | \-$1.77 tax to deduct from taxable portion of discount (6% of $29.56) | \-$31.33 | Applied to whole transaction. Tax is prorated based on taxable and nontaxable net totals |
| **Nontaxable discount portion** | 

-   \-$1.04
-   **3.4% of discount amount ($30.60) applied for nontaxable items**

 | 0.00 no tax to deduct | \-$1.04 |  |
| **Totals** | $264.40 | $15.33 | $279.33 | Important: In this case, the Discount Rate across all items takes nontaxable items into account and pro-rates the tax discount accordingly. |
|  |  |  |  |  |
| Taxable Discount 96.6% of $30.60 | \-$29.56 | $1.77 | \-$31.33 |  |
| Non-tax Discount | \-$1.04 | 0 |  |  |
| **Discount Totals** | \-$30.60 | \-$1.77 | \-$31.33 |  |

**Scenario 2: Line Item Discount for a Single Line item**

By default, if you use Method 2 to apply a discount on a single line item on a sales order or invoice (using a line item discount as shown in the screenshot), the following calculations will apply:

| Discount to All Items using Discount Field |
| --- |
|  | **Net Price** | **Tax** | **Total** | **Notes** |
| **Taxable Items** | $285.00 | $17.10 | $302.10 |  |
| **Non Taxable** | $10.00 | 0.00 | $10.00 |  |
| **Discount** | \-$30.60 | \-$1.84 | \-$32.44 | Tax calculated on previous line item where tax = T |
| **Total** | $264.40 | $15.26 | $279.66 | Important: In this case, the Discount applied to the single line item does not take nontaxable items into account so the tax calculation is under by .07 cents. |

## Applying a Discount After Sales Tax {#bridgehead_N1821302}

By default, when you create a discount item, the discount is applied after sales tax has been calculated and applied to the items.

## Applying a Discount Before Sales Tax {#bridgehead_4567397511}

If you want the discount to be applied before sales tax is calculated and applied to the item, you must enable the Apply Before Sales Tax option for the discount item.

## Respect Discount Item Tax Preference {#bridgehead_4762637163}

The **Respect Discount Item Tax Preference** box is available for certain countries only.

For information about the **Respect Discount Item Tax Preference** box for Brazil, China, and India, see [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html).

For information about the **Respect Discount Item Tax Preference** box for the U.S., see [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html).

#### To enable the Apply Before Sales Tax preference: {#procedure_N1821334}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click the discount item to modify.
    
3.  On the Discount Item record, click the **Accounting** subtab.
    
4.  Check the **Apply Before Sales Tax** box.
    
5.  Click **Save**.
    

### Related Topics

-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [Applying Sales Tax or VAT to Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1817936.html)
-   [Applying Sales Tax to Discount Items (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1818019.html)
-   [Discount Methods (VAT Nexuses)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1821386.html)
-   [Applying VAT Before or After Discounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1822423.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
