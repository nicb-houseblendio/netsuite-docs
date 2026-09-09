---
id: "section_N2248474"
type: "section"
title: "Discount Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Discount Items"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html"
anchors: ["bridgehead_N2248491", "bridgehead_N2248506", "bridgehead_N2248522", "bridgehead_N2248553", "procedure_N2248583"]
sha256: "36bcfbf4b4b322ab4eb5de914b27f391bab1151b9e497887080153ca38c0c463"
---

You can create discount items to use on sales transactions. When these items are added, discounts are applied to the items being sold. Using discount items lets you track discount amounts without affecting inventory valuation. For more information, see [Create or Verify Discount Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1497969716.html).

Note:

NetSuite converts flat-rate discounts to the equivalent percentage values on related transactions created from the sales order. Examples of transactions that may be created from the sales order include return authorizations, invoices, and cash sales.

You can add discount items as line items, or you can select a discount item in the body of sales transaction.

If you want discount items available to customers online, you must associate them with an item coupon, promotion code for use on your website. For more information, see [Creating Item Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185383.html)

Note:

When using a discount item, be sure that the transaction item and the applied discount item have the same associated tax code. If the transaction item uses a tax code that is different than the tax code for the discount item, errors in tax calculations may occur.

## Line-Item Discounts {#bridgehead_N2248491}

When a discount item is applied on a sale, it reduces the line-item amount that precedes the discount item by a percentage or flat rate. A discount item added in-line is never applied to all items on the transaction.

To apply a discount to all items on the transaction, choose a discount in the header. For more information, see [Transaction Discounts](#bridgehead_N2248506).

## Transaction Discounts {#bridgehead_N2248506}

A discount item can also be used to reduce the total amount of a transaction.

To apply a discount item to a transaction's total, select the discount item you want to apply in the Discount field. NetSuite autofills the item's rate and the transaction's discounted total.

Note:

When the SuitePromotions feature is enabled, discount items applied at the transaction level will only be applied to the transaction subtotal. This means, for example, tax and shipping costs will not be discounted.

## Non-Posting Discount Items {#bridgehead_N2248522}

You can also create discount items that don't post to a general ledger account. When a discount item without an account specified is added to a transaction, it doesn't post as an individual transaction line. Instead, the item it is applied to posts the net amount of the discount.

For example, when you create a sales transaction and add the non-posting discount after a line-item, the discount is applied to the previous line-item only. The net amount of the transaction is then correct and the appropriate revenue posts.

This net amount is used for commissions calculation and to post deferred revenue accurately when you use the Revenue Recognition feature.

Note:

If you use the classic Revenue Recognition features, always use non-posting discount items with items on sales transactions that have an associated revenue recognition template. This ensures that the net amount of the invoice is amortized and the discount posts to your ledger properly.

## Discount Items and Promotion Codes {#bridgehead_N2248553}

You can also associate a discount item with a promotion code. Then, you assign promotion codes to customer records. When you enter a transaction for a customer with a promotion code, the appropriate discount autofills on the transaction form.

To create promotion codes, go to _Lists > Marketing > Promotion Codes > New_.

## Amount, Amount (Net of discount), and Amount (Gross before discount) {#procedure_N2248583}

On transactions and reports, NetSuite uses the terms Amount, Amount (Net of discount) and Amount (Gross before discount). The definition for the Amount column differs based on the following:

-   whether an applied discount is a posting discount
    
-   which transaction line you are observing.
    

The terms are defined as follows:

-   If a posting discount is applied, then:
    
    -   Amount (Net of discount) = transaction amount including discount
        
    -   Amount (Gross before discount) = transaction amount excluding discount
        
    -   Amount = Amount (Gross before discount)
        
-   If a non-posting discount is applied, then:
    
    -   Amount (Net of discount) = transaction amount including discount
        
    -   Amount (Gross before discount) = transaction amount excluding discount
        
    -   Amount = Amount (Net of discount)
        

For example, invoice #1181 has a $100 non-posting discount. The Amount (Net) is $100 and the Amount (Gross) is $200 for the revenue line. Invoice #1182 has a $100 posting discount. The Amount (Net) is $100 and the Amount (Gross) is $200. Although the amounts are the same, the Amount column differs. For invoice #1181, the amount is $100 and for #1182, the amount is $200.

### Related Topics

-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
-   [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)
-   [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html)
-   [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)
-   [Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247990.html)
-   [Service Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248153.html)
-   [Download Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248348.html)
-   [Subtotal Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248793.html)
-   [Description Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248894.html)
-   [Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248975.html)
-   [Expense Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4042372470.html)
-   [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html)
-   [Other Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249208.html)
-   [Payment Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249363.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
