---
id: "section_N2403862"
type: "section"
title: "Billing a Purchase Order With Advanced Receiving"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Billing a Purchase Order With Advanced Receiving"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html"
anchors: ["procedure_N2403904", "bridgehead_N2404097"]
sha256: "386967ba5270dd8a272484011a90436500c5a501ae5b21e32638f9175a2c950e"
---

Billing a purchase order indicates you have received an invoice from the vendor for items purchased and creates a bill in accounts payable. You can turn your purchase order into a bill without rekeying any data.

When a vendor bill includes many transaction lines, best practice is to split the vendor bill to improve processing performance.

If you use Advanced Receiving, you can receive an order and create a bill in separate steps. To enable advanced receiving, go to Setup > Enable Features. On the Purchase Transactions subtab, check the Advanced Receiving box, and click Save.

Note:

When you create a standalone bill or bill an existing purchase order, the transaction requires an active Accounts Payable account. For an active account, you must enable an existing Accounts Payable account, create a new Accounts Payable account, or contact your System Administrator.

#### To bill a purchase order with advanced receiving: {#procedure_N2403904}

1.  Go to _Transactions > Payables > Bill Purchase Orders_.
    
2.  On the Bill Purchase Orders page, in the **Vendor** field, select a vendor to filter the list of bills.
    
    You can select **All** to show all open bills, but you can create bills for only one vendor at a time.
    
    If you use NetSuite OneWorld and your vendors are shared with multiple secondary subsidiaries, a **Subsidiary** column appears. This column lists all of the unbilled purchase orders associated with the subsidiaries assigned to the selected vendor. You can bill any or all of these purchase orders that share the same subsidiary and currency. For more information about shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
3.  Click the **Select Order Number** field to scan in transaction bar codes.
    
    To scan in bar codes, you must select All in the Vendor field.
    
4.  In the **Use Bill-To Address From Vendor** field, do the following:
    
    -   Check this box to use the vendor's default billing address by default in the vendor field on the **Billing** subtab on the bill created.
        
    -   Clear this box to choose the following functions: If only one purchase order is submitted, the bill generated uses the purchase order address. If two or more purchase orders are submitted, the bill generated uses the default billing address. This is true even if the purchase orders submitted do not have addresses entered or have addresses that are not the vendor's default billing address. If a vendor has no default billing address, the Bill page defaults to no address, even if the purchase orders have billing addresses set.
        
5.  Check the box in the **Bill** column next to all purchase orders you want to bill.
    
    If you check more than one purchase order, items from all the purchase orders you check are grouped together on one bill.
    
6.  Click **Submit**.
    
    The bill appears and shows the purchase order items.
    
    -   If **Match Bill to Receipt** is set on the purchase order at vendor bill creation, you can select specific receipts in the **Receipts** column. Then, the values on the receipt determine the following:
        
        -   A bill is created for specific receipts that are selected.
            
        -   The bill is checked against receipt values for variances.
            
7.  If the information on the bill is correct, click **Save**.
    

Important:

When processing transactions, you must submit one page at a time. If you do not submit each page individually, information is not saved and can be lost when you switch between pages. To process multiple pages of information, always submit each page individually.

You can also bill purchase orders at the same time you receive the purchase order. Go to _Transactions > Purchases > Receive Order._. Select a vendor and then click **Receive** next to the purchase order. On the Item Receipt page, verify the information, and then click **Save and Bill**. A bill is created for each of the items received on that purchase order.

If you do not use Advanced Receiving, when you receive items on a purchase order, a bill is created for the items at the same time. To receive and bill a purchase order without Advanced Receiving, go to _Transactions > Purchases > Receive Order._.

To see bills you have created from purchase orders, go to _Transactions > Purchases/Vendors > Enter Bills > List_.

To see what has been received and billed for a purchase order, open the purchase order. Click **Receipts & Bills** at the top of the page.

## Closing Line Items on a Purchase Order {#bridgehead_N2404097}

On purchase orders, you are able to close line items manually when you do not intend to receive open items on the order. For more information, see [Closing Line Items on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415338.html).

### Additional Information

-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

### Related Topics

-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
    
-   [Entering a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html)
    
-   [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html)
    
-   [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html)
    
-   [Editing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html)
    
-   [Viewing the Status of a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html)
    
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
    
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)
    
-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
