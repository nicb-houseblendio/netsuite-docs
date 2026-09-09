---
id: "section_N2371184"
type: "section"
title: "Vendor Bill Variances"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Variances"
parent: "chapter_N2370131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html"
anchors: ["bridgehead_N2372040", "subsect_160681500759", "procedure_N2372096", "subsect_160681512317", "procedure_N2372315", "bridgehead_N2372466", "bridgehead_N2372513", "subsect_87115456170", "bridgehead_N2372606"]
sha256: "65511ad4cbcae264e4f4bffa2e5bb2d21708c082c6995ff3119ea31f610cd9cf"
---

When you enter purchase orders, receipts, and vendor bills for items, each transaction can show a quantity, price, and exchange rate for the items. If there are any discrepancies between the quantity, price, or exchange rate, a remaining value may post to the Accrued Purchases account. If you use the Advanced Receiving feature, you can use the vendor bill variances process to generate journal postings to variance accounts, based on discrepancies.

For example, you enter a purchase order that shows the following:

| Purchase Order |  |  |
| --- | --- | --- |
| Price= $5 | Quantity= 100 | Exchange Rate = 0.50 |

Next, you receive the items into your warehouse. The item receipt shows the following:

| Receipt |  |  |
| --- | --- | --- |
| Price= $4.5 | Quantity= 98 | Exchange Rate = 0.52 |

Then, the vendor sends you a bill for the purchase. The bill shows the following:

| Vendor Bill |  |  |
| --- | --- | --- |
| Price= $6 | Quantity= 105 | Exchange Rate = 0.6 |

| Receipt |  |  |
| --- | --- | --- |
| DR | Inv Asset | 4.5\*98\*0.52 = $229.32 |
| CR | Accrued Purchases | $229.32 |

| Vendor Bill |  |  |
| --- | --- | --- |
| DR | Accrued Purchases | 6\*105\*0.60 = $378 |
| CR | Accounts Payable | $378.00 |

Because the amounts on the receipt and vendor bill do not match, the remaining amount needs to be reconciled ($378.00 - 229.32 = $148.68).

To resolve these discrepancies, you can reconcile these differences using the Post Vendor Bill Variances page to post variance journal entries.

When you track and resolve these variances over time, the accuracy of your record-keeping improves. You are also better able to work with your vendors to ensure that billed quantities and prices are consistent with the receipt quantities and prices.

The Post Vendor Bill Variances page posts journal entries with these types of variances:

-   **Bill Quantity Variance** - to resolve variances between quantities on bills and receipts
    
-   **Bill Price Variance** - to resolve variances between the unit cost of items on bills and receipts
    
-   **Bill Exchange Rate Variance** - to resolve variances between exchange rates on bills and receipts
    

Create variance journals at _Transactions > Payables > Post Vendor Bill Variances_. For more information, see [Posting Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html).

## Methods for Posting Variances {#bridgehead_N2372040}

Choose from two methods to create a variance post:

-   [Posting Variances Based on Vendor Bill Lines](#subsect_160681500759)
    
    In this case, the Match Bill to Receipt option is used.
    
-   [Posting Variances Based on Purchase Order Lines](#subsect_160681512317)
    
    In this case, the Match Bill to Receipt option is not used.
    

## Posting Variances Based on Vendor Bill Lines {#subsect_160681500759}

When you use the Match Bill to Receipt method, note the following. Each line on a purchase order can be marked to require matching those line items to the items on the corresponding vendor bill. Then, lines on associated receipts are compared to vendor bill lines to check for variances in the quantity, price, and exchange rate. Journal entries can be created to post the amounts to variance accounts.

The Match Bill to Receipt method is used if a purchase spans multiple accounting periods and there is a need to post the variances. Using this method, variances you post are based on vendor bill lines, not purchase orders.

To mark a purchase order line for matching, check the Match Bill to Receipt box on each line for items you want to be matched. You can also set the box to be checked by default using the setting on item records. Then, when the item is added to a purchase order, the line automatically shows the Match Bill to Receipt box as checked. For more information, see the Match Bill to Receipt section of [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html).

On vendor bills, you can select specific receipts in the Receipts column. Do this when you create the vendor bill if the corresponding purchase order lines have Match Bill to Receipt checked. Then, a bill is created for the receipts that are selected. Also, the bill is checked against receipt values for variances.

Using this method, all purchase orders with lines marked Match Bill to Receipt are considered for variance calculations.

Note:

For lines with drop-ship items, do not check the Match Bill to receipt box.

The following example describes using the Match Bill to Receipt method:

#### To post variances based on vendor bill lines: {#procedure_N2372096}

1.  First, purchase orders are entered and dated across several months time.
    
    The purchase orders can generate variance postings whether the transaction lines are open or closed.
    
    Make sure that for all applicable lines, the **Match Bill to Receipt** box is checked.
    
    Enter purchase orders at _Transactions > Purchases > Enter Purchase Orders_.
    
2.  Multiple receipts are entered against the purchase order.
    
    To receive purchase orders, go to _Transactions > Purchases > Receive Orders_.
    
3.  Vendor bills are entered for the items.
    
    Upon creating a vendor bill from a purchase order, all bill lines automatically show any outstanding item receipts. Note that you can override the association of the receipt and vendor bill.
    
    The vendor bill must be linked to any receipts.
    
    To bill purchase orders, go to _Transactions > Payables > Bill Purchase Orders_.
    
4.  Go to the Post Vendor Bill Variances page at _Transactions > Payables > Post Vendor Bill Variances_. Variances are generated based on the differences between the vendor bill and associated receipts.
    

## Posting Variances Based on Purchase Order Lines {#subsect_160681512317}

When items on an order are fully received and billed, variances can be generated for posting. These variances are based on purchase order lines without using the Match Bill to Receipt box.

After all the vendor bills and receipts for a purchase order are entered, you can create variance journals.

Note:

If the order is not fully received and billed, open transaction lines must be closed to generate variances to post.

The following example describes generating variances without using the Match Bill to Receipt method.

#### To post variances based on purchase order lines: {#procedure_N2372315}

1.  Enter a purchase order that sets the rate and amount for items.
    
    Purchase order lines must be fully received and billed for variances to be generated. If lines are not fully received and billed, they must be closed to generate variances.
    
    Enter purchase orders at _Transactions > Purchases > Enter Purchase Orders_.
    
2.  Enter receipts with the standard cost for the items on the purchase order.
    
    To receive purchase orders, go to _Transactions > Purchases > Receive Orders_.
    
3.  Enter the vendor bill.
    
    To bill purchase orders, go to _Transactions > Payables > Bill Purchase Orders_.
    
4.  To generate variance postings, go to _Transactions > Payables > Post Vendor Bill Variances_. The list of transactions shows orders with variances calculated.
    
    1.  In the **Transaction Type** field, select **Purchase Order**.
        
    2.  Check the **Select** box next to all transactions you want to create a journal entry for.
        
    3.  When you click **Create Journal Entries**, the journals are created.
        
        Note:
        
        Vendor Bill and Receipt Lines wherein variances are computed and posted are not editable.
        

## Setting Up Item Records for Variances {#bridgehead_N2372466}

To be able to analyze variances for items, set up item records for the following:

-   Select [Variance Accounts](#bridgehead_N2372513) to post variances to.
    
-   Choose a default setting for [Match Bill to Receipt](#subsect_87115456170).
    

## Variance Accounts {#bridgehead_N2372513}

On an item record, you must select variance accounts in the Exchange Rate Variances, Bill Quantity Variances, and Bill Price Variances fields. Then, when a variance occurs for that item, it posts to the variance account you selected.

If you prefer to see one single variance, select the same account in all three variance account fields.

## Match Bill to Receipt {#subsect_87115456170}

On an item record, check this box to make the Match Bill to Receipt box checked by default on transaction lines for this item. Then, purchase orders that include this item default to have this box checked and variances are generated based on vendor bill lines.

This preference is disabled by default. Even when enabled, this option can be changed on individual purchase order lines.

Clear this box if you do not want the Match Bill to Receipt box to be checked by default on transaction lines for this item. You can still check the box on individual transaction lines as necessary.

For information about setting up item records, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).

## Variance Status Column on Bills {#bridgehead_N2372606}

You can optionally add a column to your vendor bill form to show if a variance is expected for the line.

The Bill Variance Status column can show the following statuses:

-   **No Variances** - No variances are found.
    
-   **Journal Not Posted** - Variances are found, but journal entries are not yet created.
    
-   **Journal Posted** - Variances are found and journal entries have been created.
    

To add the Bill Variance Status column, select Customize Form in the Customize list on a vendor bill. On the custom form, click the Items subtab. Check the box in the Show column next to Bill Variance Status and save the form.

### Additional Information

-   [Posting Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html)
-   [Vendor Bill Variance Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373098.html)
-   [Mass Updates for Variance Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373402.html)

### Related Topics

-   [Entering a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161968486146.html)
-   [Bill Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164726334180.html)
-   [Differences Between Bills and Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370776.html)
-   [Receiving Inventory in Advance of a Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2370995.html)
-   [Canceling a Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2375066.html)
-   [Vendor Bill Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161070688350.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)
-   [Vendor Bill Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373552.html)
-   [Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2376194.html)
-   [3 Way Match Vendor Bill Approval Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4096219721.html)
-   [Vendor Bill Approvals in the Employee Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157528106765.html)
-   [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
