---
id: "section_N2415572"
type: "section"
title: "Exchange Rates on Item Receipts"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Receiving Orders > Exchange Rates on Item Receipts"
parent: "chapter_N2410585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html"
anchors: ["procedure_N2415584"]
sha256: "65a5fa90fdabfc91be5d0f5d831f1e5b54508e24593b837f2149d470af041b1b"
---

You can set a preference for how NetSuite defaults to handle exchange rates on item receipts. Choose between using the rate shown on the purchase order or using the rate that is current when the order is received.

#### To set the exchange rate preference: {#procedure_N2415584}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Order Management** subtab.
    
3.  Select one of the following in the **Default Receiving Exchange Rate** field:
    
    -   **Use Purchase Order Exchange Rate** - The exchange rate value on the order line is the purchase order exchange rate.
        
    -   **Use Exchange Rate at the Time of the Receipt** - The exchange rate value on the order line is the receipt date exchange rate.
        
    
    Then, based on your setting, the correct rate defaults to show in the **Exchange Rate** field on receipts.
    
4.  Click **Save**.
    

For example, you enter a purchase order for 10 widgets dated 7-1-2009. The exchange rate on the purchase order is 1. When you receive the order, the current exchange rate is 1.5.

-   If you selected **Use Purchase Order Exchange Rate**, the default value of the exchange rate on the order line is 1.
    
-   If you selected **Use Exchange Rate at the Time of the Receipt**, the default value of the exchange rate on the order line is 1.5.
    

After a rate defaults to show on a transaction form, you can still enter a different rate if needed. When you view an item receipt, the base amount is displayed on the receipt.

To view item receipts, go to _Transactions > Purchases > Receive Orders > List_.

### Related Topics

-   [Receipt Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411122.html)
-   [Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411320.html)
-   [Partially Receiving a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411754.html)
-   [Receiving a Purchase Order Before Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415076.html)
-   [Receiving a Purchase Orders With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html)
-   [Creating a Bill From an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162020541497.html)
-   [Bulk Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2414814.html)
-   [Closing Line Items on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415338.html)
-   [Deleting an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163705803638.html)
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162626600304.html)
-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
