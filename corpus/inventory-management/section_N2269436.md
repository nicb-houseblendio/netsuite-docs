---
id: "section_N2269436"
type: "section"
title: "Setting a Location on a Transaction"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Setting a Location on a Transaction"
parent: "chapter_N2250682"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2269436.html"
anchors: ["bridgehead_N2269527", "procedure_N2269566", "bridgehead_N2269625", "bridgehead_N2269862"]
sha256: "fc833da92daee416df2bc6faded4f9ce8ccf270603f3cf0367db3619230207f5"
---

You can associate locations on transactions in these ways:

-   Associate one location for the entire transaction.
    
    Read [Identifying Locations in the Transaction Header](#bridgehead_N2269527).
    
-   Associate one location for each transaction line-item.
    
    Read [Setting a Location for Individual Line Items](#bridgehead_N2269625).
    
-   Associate both a location in the header and on transaction lines.
    
    Read [Line-item Locations with Header Locations](#bridgehead_N2269862).
    

## Identifying Locations in the Transaction Header {#bridgehead_N2269527}

You can choose to identify a location in the header of a transaction. This sets all transaction lines to the location identified in the transaction header.

For example, you can select a location in the header of a sales order to record where the sale is made. You could also select a location in the header of a purchase order to identify where you expect to receive those items.

When you identify your transactions by location, you can manage your inventory based on the location from which items are ordered, received, and sold.

#### To identify a location on a transaction: {#procedure_N2269566}

1.  Click the **Transaction** tab.
    
2.  Click the name of the transaction you want to create.
    
3.  In the Classifications section, in the **Locations** field, select the appropriate location. For more information about how to create a location, read [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html).
    
4.  Complete the transaction as required.
    
5.  Click **Save**.
    

When you identify locations on transactions, you can run reports with information filtered by location. For more information about reporting by locations, read [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html).

## Setting a Location for Individual Line Items {#bridgehead_N2269625}

When you use the Locations or Multi-Location Inventory feature, you can set a preference to show a location for individual line items on transactions.

Note:

To show line-item locations on a transaction, you must customize the form. For more information, see [Customizing a Form for Line-item Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270130.html).

If you do not use line-item locations:

-   The location you choose in the transaction body applies to all line items on the transaction.
    
-   An adjustment account chosen in the transaction body is also associated with the location chosen in the body.
    

If you do use line-item locations:

-   A different location can be associated with each line item.
    
-   An adjustment account chosen in the transaction body is not associated with a location.
    

Line-item locations function differently when used with each feature. For more information, see the following topics:

-   [Per-Line Locations with the Locations Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162024160153.html#bridgehead_162024176514)
    
-   [Per-Line Locations with the Multi-Location Inventory Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162024160153.html#bridgehead_162024184449)
    

## Line-item Locations with Header Locations {#bridgehead_N2269862}

If you use per-line locations, you can customize transaction forms to identify a location at the header and line level at the same time.

Using the Locations feature and the Allow Per-Line Locations preference displays a Location field on each transaction line and in the form header. You can choose the location East Coast on one line and choose West Coast on another line. Then, you can choose the location United States in the transaction header.

This is useful if you identify legal entities or geographical segments by location and want to report separate balance sheets and income statements. Therefore, a sales order can post line items to the correct locations (East and West Coast). Then, the header location allows a correct income statement to be run for United States transaction totals.

Forms customized to show a location at the header and line level must have data in both fields. If either are left blank, both fields are cleared unless they are required. If you enabled the preference to make locations mandatory, the selection is mandatory at both the header and line level.

For more information about how to customize a form to identify a classification at both the header and line level, read [Customizing a Form for Line-item Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270130.html).

### Related Topics

-   [Inventory Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161970666917.html)
-   [Inventory Management Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2249539.html)
-   [Inventory Setup with Locations and Multi-Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2252794.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Purchasing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2251098.html#bridgehead_N2251155)
-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Warehouse Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2317586.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
