---
id: "section_N2400504"
type: "section"
title: "Entering a Purchase Order"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Purchasing and Receiving > Purchasing > Purchase Order Management > Entering a Purchase Order"
parent: "section_N2399585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400504.html"
anchors: ["procedure_N2400552", "procedure_N2400588", "procedure_N2400702", "procedure_N2400760", "procedure_N2400955", "bridgehead_N2400973", "procedure_N2400980", "procedure_N2402430", "procedure_N2402486", "procedure_N2402507"]
sha256: "8fb3b0b059c6c0dbafdb13f156e104847c5f379f17f5f1f5248eb91985be32d7"
---

Enter a purchase order to record a pending purchase and keep a record of items you need to stock or expect to receive. Then, you can track items you receive and items that remain outstanding.

You can create purchase orders individually or in bulk. For more information about creating bulk purchase orders, see [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html).

Note:

This is a non-posting transaction.

After entering a purchase order, you can optionally enter a vendor prepayment for the same vendor. For information about entering prepayments from a purchase order, see [Entering Vendor Prepayments From a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157311209466.html).

#### To enter an individual purchase order: {#procedure_N2400552}

1.  Go to _Transactions > Purchases/Vendors > Enter Purchase Orders_.
    
2.  Complete the form as described in the section below.
    
3.  When all information about the form is complete, click **Save**.
    

#### Primary Information {#procedure_N2400588}

1.  In the **Custom Form** field, choose the **Standard Purchase Order** form or select a custom form you have already created. Click **New** to customize a purchase order form now.
    
2.  In the **Vendor #** field, NetSuite inserts your account number for this vendor. This number is entered on the **Financial** subtab for this vendor's record at _Lists > Relationships > Vendors_.
    
3.  Select or enter the vendor's name.
    
    Important:
    
    If you use NetSuite OneWorld and the selected vendor is shared with multiple subsidiaries, you can assign any subsidiary to associate with this purchase order.
    
    After you select the **Subsidiary**, the fields on the **Items** subtab change to reflect the values associated with the selected subsidiary. In addition, in the Classification section, the **Class**, **Department**, **Location**, **Currency**, **Tax Nexus** and other fields also change to reflect the selected subsidiary. For more information about shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
4.  If you are entering a purchase request for an employee, select the employee's name.
    
    In OneWorld, you can select an employee from a subsidiary other than the vendor's subsidiary.
    
    Note:
    
    If your company uses approval routing and this employee has a supervisor, the supervisor must approve this request before it is a purchase order.
    
5.  If you have permission to approve this purchase order, check the **Supervisor Approval** box.
    
6.  In the **Receive By** field, enter the date by which you need to receive this order.
    
7.  Enter a date for this purchase order. The current date shows by default.
    
8.  Accept or enter the purchase order number.
    
9.  In the **Memo** field, enter a memo to identify this purchase order. When you use the Search Transactions feature, you can search for specific words and phrases in this field.
    
10.  The **Available Vendor Credit** field displays the remaining credit for this vendor before a payment is received. It is converted from vendor's primary currency into the transaction currency. The field value is available only in edit mode.
     
     This field is visible when you customize the purchase order. To display this field, you must first enable accounts payable preferences. Go to _Setup > Accounting > Preferences > Accounting Preferences_. In the Accounts Payable section, check the **Vendor Credit Limit Warnings** and **Vendor Credit Limit Includes Orders** boxes. Click **Save**. Then, from the **Customize** menu at the top right of the purchase order, click **Customize Form**. Click the **Screen Fields** subtab. Check the **Show** box next to **Available Vendor Credit**. Click **Save**.
     
     If the transaction exceeds the vendor's credit limit, a warning message appears indicating the exceeded credit amount. The message doesn't prevent you from saving the transaction. Click **OK** to save the transaction.
     

#### Classification {#procedure_N2400702}

1.  Select a department or class if you track them.
    
    For OneWorld accounts, you can select a department or class from the vendor's subsidiary or the employee's subsidiary.
    
    If the **Available Vendor Credit** field appears, changing the subsidiary changes the available credit limit value to reflect the currency of the selected subsidiary.
    
2.  If you track locations, choose a location for this order.
    
    For OneWorld accounts, you can select a location from the vendor's subsidiary or the employee's subsidiary.
    
3.  If you use the Multiple Currencies feature, select the currency you want to use for this purchase order. This currency will be used for the entire purchasing process (including item receipt, the vendor bill, and payment) and can't be changed. For more information, see [Vendors and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1400742.html).
    
    If this purchase order was created from a purchase request, the currency from the purchase request is used and can't be changed.
    
    The vendor's primary currency is selected by default.
    
    If the **Available Vendor Credit** field appears, changing the currency changes the credit limit value to reflect the selected currency.
    

#### Items {#procedure_N2400760}

1.  If you use multiple currencies, the current exchange rate for this vendor's currency appears in the **Exchange Rate** field.
    
    You can change the exchange rate for this transaction only, or you can update the currency record with the exchange rate you enter here. For a description of how setting the exchange rate affects the transaction, see [Setting Exchange Rates Directly on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404249.html).
    
    The vendor's currency appears in the **Currency** field. All currency amounts on this transaction are shown in this currency.
    
2.  Click the **Items** subtab.
    
    Important:
    
    There is a specific relationship between the date, the exchange rate, the item, and the item rate.
    
    In particular, when you set a date, the exchange rate is automatically filled with the value of the exchange rate at that date. When you select an item, the item rate is automatically calculated based on the price of the item and the value of the exchange rate. If you manually change the value of the exchange rate or the item rate, the relationship between the two breaks. Whenever the date is changed, the rate won't respond to the change and remains the same.
    
    If you manually changed one of these two values, the item rate can still change when the date is updated. This can occur if the item rate matches exactly with the one calculated based on the item and exchange rate. In this case, the relationship remains intact, and the item rate is updated when the PO date changes.
    
    As note above, when the date and the exchange rate are already set, when you add item, the item rate is automatically calculated. If you don't save the record and then change the date again, the new exchange rate is applied but the rate will remain the same. To have the item rate automatically updated based on the new exchange rate, cancel the item and then re-add after you set the date.
    
3.  In the **Item** column, select an item.
    
    1.  To add several items to this transaction, click **Add Multiple**.
        
        The Choose Item window opens and shows a list of items you can add.
        
    2.  Filter the list by item type or name.
        
    3.  In the left pane click an item to add it to the right pane.
        
    4.  Enter an item **Quantity**.
        
    5.  Click **Done**.
        
        Items and quantities shown in the right pane are added to the transaction.
        
4.  In the **Quantity** column, enter the quantity for this item.
    
5.  In the **Serial Number** field, enter the serial number of the item.
    
    Separate each serial number with a space, comma or by pressing **Enter** after each one.
    
    You must enter a serial number for each serialized item. For example, if you enter a quantity of **2**, then you must enter two serial numbers.
    
6.  Accept the amount in the **Rate** column or enter a new rate for this item.
    
    The total amount for this item is calculated and appears in the **Amount** column.
    
    If you use NetSuite OneWorld and the vendor is shared with multiple subsidiaries, note the following. The price for the item adjusts to reflect the costs associated with the selected subsidiary.
    
7.  Set any options for this item.
    
8.  If this item is for a particular customer, select that customer in the **Customer** column.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any customer associated with the selected subsidiary. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
9.  If you want the cost of this item billed back to the chosen customer, check the **Billable** box.
    
10.  Enter an **Expected Receipt Date** that is the day you anticipate the item will arrive in your warehouse. This date is used in calculations for Demand Planning and Advanced Inventory Management.
     
     This defaults to show the date of this purchase transaction.
     
11.  Click **Add**.
     
12.  Repeat these steps for each item you want to add.
     

#### Expenses

1.  If you allow expenses on purchase orders, click the **Expenses** subtab.
    
2.  In the **Account** column, select an account for this expense.
    
3.  In the **Amount** column, enter the expense amount.
    
4.  If this expense is for a particular customer, select that customer in the **Customer** column.
    
5.  If you want this expense billed back to the chosen customer, check the **Billable** box.
    
6.  Click **Add**.
    
7.  Repeat these steps for each expense you want to add.
    

#### Billing {#procedure_N2400955}

1.  In the **Vendor Select** field, choose the billing address for this vendor.
    
    -   Select **New** in the list. You can also click the **+** icon to create a new address for this purchase order and saved with the vendor record.
        
    -   Select **Custom** in the list to create a new address for this purchase order only and not saved with the vendor record.
        

## Shipping {#bridgehead_N2400973}

Note:

The Shipping subtab only appears on a standard or custom drop ship purchase order form.

#### Shipping Information {#procedure_N2400980}

1.  In the **Ship Date** field, enter the date you expect the items to be shipped.
    
2.  Select your **Shipping Method** for this transaction. For more information about shipping methods, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
    
3.  In the **Additional Tracking Number** field, enter the shipment tracking number from the shipping company.
    
    If you use the exact format used by UPS or FedEx, the tracking number appears on the transaction as a link to the respective website. You can click the link to check the status of the shipment.
    

#### Shipping Address {#procedure_N2402430}

1.  If a customer is not selected in the **Ship To** list, your company shipping address autofills the **Ship To** text field. You can change this address as needed.
    
    Note:
    
    Take note of the following:
    
    -   The selection of a shipping address varies slightly depending on whether the shipment is going to your company or to a customer.
        
    -   If you use NetSuite OneWorld and select Location, the Ship To address will autofill with the address specified on the Location record. If the Location field is left blank, the Ship To address will use the Shipping Address as specified on the Company information page.
        
    
    -   To change the shipping address saved with your company record, go to Setup > Company > Company Information. Click the **Edit** link next to the **Shipping Address** field.
        
    -   To enter a shipping address for your company for this purchase order, select **Custom** from the **Ship To Select** list. Then, complete the fields in the address popup window.
        
2.  When you select a customer in the **Ship To** list, the customer's default shipping address autofills the **Ship To** text field. You can change this address as needed.
    
    -   Select another address that is associated with the customer from the **Ship To Select** field.
        
    -   Select **New** in the **Ship To Select** field. You can also click the **+** icon to add an address for this purchase order and saved with the customer record.
        
    -   Select **Custom** in the **Ship To Select** field to add an address for this purchase order only and not saved with the customer record.
        
    -   Click the **Edit** icon to make changes to the address selected in the **Ship To Select** field. These changes are saved with the customer record.
        

#### Relationships {#procedure_N2402486}

1.  Under Contacts, the primary contact for the customer is selected automatically. To edit information for this contact, click the contact's name.
    
2.  You can also add contacts to this order by entering the contact's information and clicking **Add**.
    

#### Communication {#procedure_N2402507}

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
    

You can check the To Be Emailed and To Be Faxed boxes on purchase orders prior to supervisor approval. If a purchase order is submitted with either box checked but still needs approval, the email or fax is not sent. The boxes remain checked. At the time of approval, the email or fax is sent and the To Be Emailed and To Be Faxed boxes are cleared.

After a purchase order is recorded you can track the items as they are received.

To view a list of purchase orders, go to _Transactions > Purchases > List._, and then click View next to the order.

When you view a purchase order, in the Print button list, click Print Labels to print a label for each item on the order.

You can use the Editing feature with the To Be Emailed and To Be Faxed boxes. The purchase order must be approved and the boxes clear. If the boxes are checked using the Editing feature, the purchase order is emailed.

### Related Topics

-   [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html)
-   [Setting Purchasing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2400174.html)
-   [Bulk Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2402825.html)
-   [Ordering Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403352.html)
-   [Billing a Purchase Order With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2403862.html)
-   [Editing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2404305.html)
-   [Closing a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163179592993.html)
-   [Viewing the Status of a Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2408514.html)
-   [Printing a Tax ID or Resale Number on Purchase Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4746558953.html)
-   [Purchase Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2407704.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
