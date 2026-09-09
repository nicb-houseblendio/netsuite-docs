---
id: "section_N1307628"
type: "section"
title: "Receiving a Customer Return"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Return Management > Receiving a Customer Return"
parent: "section_N1302852"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html"
anchors: ["bridgehead_N1307716", "procedure_N1307737"]
sha256: "a95615c9613661d40bec785cf6629a7c3e863739793f2218fd4e5354c9d185b1"
---

When a shipment from a customer arrives at your business, process the return by matching the shipment to the corresponding return authorization number. Then, enter an item receipt for any items in that shipment against the open authorized return.

When you use the Advanced Receiving feature, you can mark authorized returned items as received when they arrive. When you receive an authorized returned order, you can indicate what was received and process the return based on those quantities.

By entering a receipt against the RMA, the following information is updated:

-   Items on return authorizations are recorded as received.
    
-   Inventory records are updated for the new stock levels.
    
-   Inventory asset accounts are updated with the values of returned items.
    
-   Status of the return is updated.
    

Then, your records show the most current information.

If you have not enabled the Refund in Advance of Return preference, you need to know when items are received to issue credits that are due to customers. For more information about this preference, read [Preferences for Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html).

## Exchange Rates on Returns {#bridgehead_N1307716}

You can set a preference for how currency exchange rates are handled on returns you process. This helps if exchange rates change between the time an authorization is entered and when it is received. For details, read [Exchange Rates on Item Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html).

#### To receive an authorized customer return: {#procedure_N1307737}

1.  Go to _Transactions > Customers > Receive Returned Order (Administrator)_.
    
2.  Select a customer from the dropdown list.
    
3.  In the **Receive** column, check the box next to the return you received from the customer.
    
4.  Click **Submit**.
    
5.  On the Item Receipt page:
    
    -   Verify information in the following fields:
        
        -   **Customer** - the customer who returned the order
            
        -   **Receipt of** - the return authorization number of the return you are receiving
            
    -   Verify or enter information in the following fields:
        
        -   **Date** - the date on which the return was received
            
        -   **Posting Period** - Select the period you want to post this transaction to. If a period is closed, you can't post to that period.
            
        -   **Ref. No.** - a number you can later use to reference this partial shipment
            
            Note:
            
            On the **Transactions** subtab, check the **Allow Override** box next to **Item Receipt** and click **Save**.
            
        -   **Memo** - Enter an optional reference memo for this receipt. Later, you can search for this receipt by text entered in the memo.
            
6.  On the **Items** subtab, check the box in the **Receive** column next to items you are receiving.
    
7.  In the **Quantity** column, enter the amount of each item you received in this shipment.
    
8.  In the **Restock** column, do one of the following:
    
    -   Check the **Restock** box to return this item to your inventory. Your inventory reflects the increased count of the returned item and the value of your inventory is also increased.
        
    -   Clear the **Restock** box to write the item off as an expense. Your inventory does not reflect the increased count of the returned item and the value of your inventory is not increased. Items that you write off are logged as an expense and the income you lose by not selling the item is posted as a loss.
        
    
    Note:
    
    You can set preferences for default handling of returned items you receive. For more information, read [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html).
    
9.  If you use the Multi-Location Inventory feature, you must select a location for each returned item.
    
10.  On the **Expenses** subtab, check the box in the **Mark Received** column next to expenses you want to receive.
     
11.  When you have finished, choose one of two options to post the information to your NetSuite account:
     
     -   Click **Save** to save the information and return to the Transactions page.
         
     -   Click **Save & Refund** to save the information and go to the cash refund for this return.
         
     
     You credit customers only for what you received.
     

Now, the items are marked as received from the customer.

Note:

You can also receive items on a return authorization record. Go to _Transactions > Customers > Issue Return Authorizations > List (Administrator)_ and click view next to the return authorization with the Pending Receipt status. Click **Receive** to mark the items as received. NetSuite creates an item receipt record for the returned items.

![Return Authorization page with Receive button highlighted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/CustomerReturns/ReturnAuthorizationPendingReceipt.png)

To see what has already been received and processed for a return authorization, open the return authorization record and click the Related Records subtab. Item receipts and refunds (such as credit memos and cash refunds) are listed on the Receipts & Refunds tab. Click the record link to view the related record. See [Customer Credits and Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310987.html) for more information.

### Related Topics:

-   [Customer Return Management Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303478.html)
-   [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html)
-   [Return Authorization (RMA) Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html)
-   [Preferences for Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html)
-   [Entering a Standalone Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305354.html)
-   [Entering a Linked Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306234.html)
-   [Approving a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306797.html)
-   [Printing a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307142.html)
-   [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html)
-   [Closing Line Items on a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1309679.html)
-   [Customer Return Authorization Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310133.html)
-   [Reporting on Customer Returns Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310580.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
