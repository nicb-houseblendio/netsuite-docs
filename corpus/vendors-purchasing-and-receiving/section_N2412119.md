---
id: "section_N2412119"
type: "section"
title: "Receiving a Purchase Orders With Advanced Receiving"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Receiving Orders > Receiving a Purchase Orders With Advanced Receiving"
parent: "chapter_N2410585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html"
anchors: ["procedure_N2412194", "procedure_N2414390", "procedure_N2414411", "bridgehead_1493684781", "bridgehead_1493684735", "bridgehead_N2414561", "bridgehead_N2414633", "bridgehead_N2414654"]
sha256: "386156b1d102b17f2d961d0dd83d10ed81ae1c349f088af637ed0819a635633a"
---

After items you ordered have arrived, process the purchase order by receiving the items and creating a bill for them.

-   **Receiving** a purchase order indicates you have received the items you ordered and added them to your inventory.
    
-   **Billing** a purchase order indicates you expect payment for the items and creates a bill in accounts payable.
    

When receiving a purchase order, you can receive an entire purchase order or only some items on the order. If you receive only part of the order, you can receive the remainder later. You need to receive and bill each purchase order for all items you receive.

If you use the Advanced Receiving feature, you can receive and bill purchase orders as separate transactions. This enables you to receive entire orders or parts of an order, even if you do not bill the order when you receive it. To enable Advanced Receiving, go to _Setup > Company > Enable Features_. Check the Advanced Receiving box and then click Save.

#### To receive a purchase order with advanced receiving: {#procedure_N2412194}

1.  Go to _Transactions > Purchases > Receive Order_.
    
2.  Complete the steps described in the sections below.
    
3.  When you have filled in all information, do one of the following:
    
    -   Click **Save**.
        
    -   Click **Save and Bill** to also create a vendor bill for the items you mark received.
        

#### To select an order:

1.  The Receive Order queue displays the following information about each order pending receipt:
    
    -   **Transaction Type** - the kind of transaction
        
    -   **Mark Shipped** - identifies drop shipment orders
        
    -   **Date** - the purchase order transaction date
        
        You can click the date to open the purchase order form
        
    -   **PO #** - the purchase order number
        
    -   **Vendor Name** - name of the vendor
        
    -   **Ship To** - the contact for the item being shipped
        
    -   **Memo** - the memo entered on the purchase order
        
    -   **Order Total** - total purchase amount for the order
        
    -   **Currency** - the currency used on the purchase order
        
2.  Select a vendor in the **Vendor** field to filter the list. Select **All** to show orders for all vendors.
    
3.  In the **Process** column, click **Receive** next to the purchase order.
    

#### To complete the item receipt:

1.  On the Item Receipt page, accept or enter a number you can later use to reference this partial receipt in the **Reference #** field.
    
2.  Verify information in the following fields:
    
    -   **Vendor** - the vendor filling the purchase order
        
    -   **Created From** - the purchase order number of the order you are receiving
        
3.  Verify or enter the date on which the order was received.
    
4.  Select a posting period.
    
5.  Optionally enter a memo. Text you enter in this field can be searched for later.
    

#### Items Subtab

1.  On the **Items** subtab, check the box in the **Receive** column next to items you are receiving.
    
2.  Select a location to receive the items into inventory.
    
3.  The on-hand quantity autofills when you select a location.
    
4.  The **Remaining Quantity** field shows the number not yet received.
    
5.  In the **Quantity** column, enter the amount of each item you received in this shipment.
    
6.  In the **Serial Number** field, enter the serial numbers of the items you receive.
    
    Note:
    
    The quantity of serial numbers entered must match the quantity of serialized items on each transaction line. For example, if you are receiving three serialized items, you must enter three serial numbers.
    

#### Expenses Subtab

1.  Click the **Expenses** subtab.
    
2.  Check the box in the **Mark Received** column next to expenses you want to receive.
    

#### Landed Cost Subtab

1.  Click the **Landed Cost** subtab to enter landed cost for this transaction.
    
    For more information, see [Entering Landed Cost on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2418831.html).
    

#### Relationships {#procedure_N2414390}

1.  Under **Contacts**, the primary contact for the customer is selected automatically. To edit information for this contact, click the contact's name.
    
2.  You can also add contacts to this order by entering the contact's information and clicking **Add**.
    

#### Communication {#procedure_N2414411}

1.  On the **Messages** subtab, complete the following as necessary:
    
    -   Check the **To Be Printed** box if you want to save the purchase order in a queue for printing later.
        
    -   Check the **To Be Emailed** box and enter or verify an email address if you want to email the purchase order.
        
        Note:
        
        If you use Approval Routing, you can only email purchase orders that have been approved by a supervisor.
        
    -   Check the **To Be Faxed** box and enter or verify a fax number if you want to fax the purchase order.
        
        If you prefer, you can click **Print** when you have finished entering all the information to immediately save and print the purchase order.
        
    -   Enter a vendor message to appear on your purchase order.
        
2.  Use the **Events**, **Tasks**, and **Phone Calls** subtabs to attach activities to this transaction. For more information, see [Attaching Events, Tasks, and Calls to Records and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084924.html).
    
3.  On the **Files** subtab, you can select and attach files from the File Cabinet related to this transaction. Select **New** to upload a new file to File Cabinet.
    
4.  On the **User Notes** subtab, you can enter a title and note for any comments you want to add to this transaction. Click **Add** after each note.
    

## Partially Received vs. Fully Received {#bridgehead_1493684781}

If you **did not receive** all items on this purchase order, your inventory is updated with the items received. The order then has the status Partially Received. To receive the rest of this order when the items arrive, repeat the steps above.

If you **did receive** all items on the purchase order, your inventory is updated with the items received. The order then has the status Pending Billing. Bill the purchase order by going to _Transactions > Payables > Bill Purchase Orders_.

To see what has already been received and billed for a purchase order, click the Related Records subtab on the purchase order. Then click Receipts & Bills.

## Receiving Serial or Lot Numbered Inventory {#bridgehead_1493684735}

After you receive **serialized or lot-numbered inventory** from vendors, you can enter a memo or custom information about the item.

#### To enter a memo or custom information about an item:

1.  Go to _Transactions > Purchases > Receive Order_.
    
2.  Click **View** next to the order.
    
3.  Click the Open icon next to the Serial or Lot number.
    
4.  In the popup window, you can enter a memo and values in any custom fields for each inventory number.
    

## Receiving Overages {#bridgehead_N2414561}

Sometimes when you are receiving an order, the amount you are processing is more than the quantity shown on the receipt. This additional amount is called an overage, and NetSuite enables you to process overages using the Allow Overage on Item Receipts preference.

Advanced Receiving provides a setting to allow the receipt of more items than the original quantity entered on purchase orders.

#### To receive more items than entered on a purchase order:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **Order Management** subtab.
    
3.  Check the **Allow Overage on Item Receipts** box.
    
4.  Click **Save**.
    

With the preference set, you can enter a quantity larger than the quantity remaining for an item when processing an item receipt.

## Vendor Bill Variances {#bridgehead_N2414633}

With Advanced Receiving, purchase order items you receive can be matched to the corresponding vendor bill. Then, you can check for variances in quantities and rates. For more information, see [Posting Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html).

## Closing Line Items {#bridgehead_N2414654}

On purchase orders, you are able to close line items manually when you do not intend to receive open items on the order. For more information, see [Closing Line Items on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415338.html).

### Related Topics

-   [Receipt Workflow Charts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411122.html)
-   [Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411320.html)
-   [Partially Receiving a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2411754.html)
-   [Receiving a Purchase Order Before Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415076.html)
-   [Creating a Bill From an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162020541497.html)
-   [Bulk Receiving Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2414814.html)
-   [Closing Line Items on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415338.html)
-   [Deleting an Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163705803638.html)
-   [Exchange Rates on Item Receipts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415572.html)
-   [Printing Labels From Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162626600304.html)
-   [Receiving Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2410585.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
