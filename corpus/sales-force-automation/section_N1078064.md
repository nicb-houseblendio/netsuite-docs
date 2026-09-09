---
id: "section_N1078064"
type: "section"
title: "Entering Financial Information for the Customer"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Customers > Creating a Customer Record > Entering Financial Information for the Customer"
parent: "section_161860867711"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1078064.html"
anchors: ["procedure_N1078086"]
sha256: "a6042482b98ceb68d160dff62fa0ad3bc665c953b4edc5b12283cfc73420c887"
---

The Financial subtab has information about that customer's account with your company, like credit card data, price level, taxation, and account balance.

The fields and subtabs available under the Financial subtab depend on the features you've enabled in your account and your user role permissions. Some common subtabs are included in this topic, but others are documented with the feature that adds them.

#### To add financial information: {#procedure_N1078086}

1.  Open the customer record for editing, and click the **Financial** subtab.
    
2.  Under Account Information, provide information in the following fields as needed and available:
    
    -   **Account** - If you assign accounts to customers, enter the customer's account number.
        
    -   **Default Receivables Account** - Select the general ledger account of the type Accounts Receivable that you want to use by default on sales transactions for the customer.
        
        If you want to use the account selected as the **Default Receivables Account** in the accounting preferences, select **Use System Preference**.
        
    -   **Start Date** - Start Date - Enter or select the date this customer first started with you.
        
        When you enter the first estimate or opportunity for this customer, the transaction date becomes the value in this field.
        
    -   **End Date** - Enter how many days before the end date you want to be reminded that this customer's contract or job service needs to be renewed.
        
    -   **Reminder Days** - If you entered an end date, enter how many days before the end date you want an email reminder that the contract will expire soon.
        
        The system-defined Customers to Renew reminder uses End Date and Reminder Days. For information about reminders, see [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html).
        
    -   **Price Level** - If you want to sell to the customer at a specific price level, select an option from the list.
        
        Price levels are part of the Multiple Prices feature. For information, see [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)
        
    -   **Currency** - Select the currency this customer uses. You can't change this value after you've saved transactions for the customer.
        
        If you use the Multiple Currencies feature, this field is called **Primary Currency**, and you can select other transaction currencies on the Currencies subtab. For more information, including information about currency formats, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).
        
    -   **Override Currency Format** - If you do not use the Multiple Currencies feature, check this box to change the currency format used on screen and on printed documents for the customer.
        
        When you check the **Override Currency Format** box, the following additional field appear:
        
        -   **Currency Symbol** - Enter a symbol for the currency. Add spaces if you want to separate the currency symbol from the amount.
            
        -   **Symbol Placement** - Select **Before Number** or **After Number** to show where currency symbol appears.
            
            If you use the Multi-Language feature, choose the **Print in Customer's Locale** option to to match the customer's currency settings when you print. For information about the Multi-Language feature, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).
            
    -   **Terms** - Select the default payment terms for this customer's account.
        
        For information about adding options to this list, see [Creating Terms of Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234186.html).
        
    -   **Credit Limit** and **Hold** - Enter a credit limit for this customer, and select a hold option.
        
        For details, see [Managing Customer Credit Limits and Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1080144.html).
        
    -   **Pref. CC Processor** - Select the credit card processing profile you want to use when this customer enters an order.
        
        For setup information, see [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html).
        
3.  Under Tax Information, provide information in the following fields as needed and available:
    
    -   **Tax Reg. Number** - Enter the customer's tax registration number.
        
    -   **Taxable** - Check this box if the customer pays sales tax. Clear this box if the customer isn't taxable.
        
    -   **Tax Item** - Select the tax code you want to apply to this customer's purchases. This tax code overrides the tax code determined by the tax code lookup. For more information, see [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html).
        
        When you select a value here, it applies to the customer's purchases, even if the **Taxable** box is clear. NetSuite determines that a customer is not taxable only if the **Taxable** box is clear and the **Tax Item** field is empty.
        
    -   **Resale Number** - If you do not collect sales tax because your customer resells your merchandise, enter their tax license number in this field.
        
        Make sure that you also clear the **Taxable** box.
        
4.  The Balance Information section has read-only fields about the customer's current accounts receivable balance. For information see [Customer Balances in Transaction Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400109.html#subsect_161610274695).
    
    You can enter the following information in this section only before you save a new customer record:
    
    -   **Opening Balance** - Enter the opening balance for this customer's account.
        
    -   **Opening Balance Date** - Enter or select the date of the balance entered in the **Opening Balance** field.
        
    -   **Opening Balance Account** - Select the general ledger account for this customer's opening balance.
        
5.  If you use the Shipping Label Integration feature and third party billing, enter the following additional information in the Balance Information section:
    
    -   **3rd Party Billing Account Number** - FedEx or United Parcel Service (UPS) account number
        
        NetSuite uses this account number if you select Consignee Billing on item fulfillments that use UPS or Bill Recipient on item fulfillments that use FedEx.
        
    -   **3rd Party Billing Country** - Country associated with the customer's UPS or FedEx account number
        
    -   **3rd Party Billing Carrier** - Shipping carrier associated with the 3rd party billing account number
        
    -   **3rd Party Billing Zip** - Zip or postal code associated with the customer's UPS or FedEx account number
        
6.  Provide information in the following subtabs as needed and available. Links to detailed instructions are included.
    
    -   **Currencies** - Multiple Currencies feature adds this subtab to the customer record. For information, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).
        
    -   **Credit Cards** - Credit Card Payments feature adds this subtab to the customer record. For information, see [Tracking Customer Credit Card Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084186.html).
        
    -   **Electronic Funds Transfer** - Electronic Funds Transfer feature adds this subtab to the customer record.
        
    -   **Payment Instruments** - Payment Instruments feature adds this subtab to the customer record. For information, see [Creating a Payment Instrument Manually on a Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1538492538.html#subsect_160692591643).
        
    -   **Group Pricing** - Multiple Pricing feature adds this subtab to the customer record. For information, see [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html).
        
    -   **Item Pricing** - Use this subtab to set a price level or absolute price for items, as follows:
        
        1.  In the **Item** column, select the item you want to price.
            
        2.  In the **Price Level** column, set one of the following:
            
            -   Select a price level for this customer.
                
                For details about using price levels, read [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html).
                
            -   Select **Custom** in the **Price Level** field to set an absolute price. In the **Unit Price** field, enter the price you want to always charge this customer for this item. Absolute prices you set here override all other prices and price levels.
                
                For details about absolute pricing, read [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1083860.html).
                
        3.  Click **Add**.
            
        4.  Repeat these steps for each item you want to price for this customer.
            
    -   **Time Tracking** - The Time Tracking feature adds this subtab to the customer record. This subtab shows employee time that's billable to the customer, lists time already recorded, and lets you create new time records. For more information, see [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html).
        
7.  When you've finished updating the record, click **Save**.
    

### Related Topics

-   [Creating a Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161860867711.html)
-   [Customer Record Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161887259374.html)
-   [Assigning Additional Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161895998055.html)
-   [Entering Sales Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1077516.html)
-   [Entering Marketing Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1077855.html)
-   [Setting Preferences on the Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1079031.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
