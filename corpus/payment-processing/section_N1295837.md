---
id: "section_N1295837"
type: "section"
title: "Returned Check/NSF Fees"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Customer Payments > Handling Returned/NSF Checks > Returned Check/NSF Fees"
parent: "section_N1295030"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295837.html"
anchors: ["procedure_N1295889", "procedure_N1295992"]
sha256: "9dd9e1d89f4e8e4118e6090c7e0184e62e3b7cf6ef361519d119b3c5d4471291"
---

If you would like to charge the customer a fee for the returned check, you can add an NSF (Insufficient Funds) charge to the unpaid invoice. This fee is charged **in addition** to the current outstanding amount, and the invoice ages appropriately.

To bill a customer for returned check fees, first create an item record for returned check/NSF fees. Then, bill the customer for the returned check/NSF fees.

1.  [Create an Item Record for Returned Check/NSF Fees](#procedure_N1295889).
    
2.  [Bill the Customer for the Returned Check/NSF Fee](#procedure_N1295992).
    

#### Create an Item Record for Returned Check/NSF Fees {#procedure_N1295889}

1.  Go to _Financial > Lists > Items_.
    
2.  Under Other Charge, click **For Sale**.
    
3.  In the **Item Name/Number** field, enter **Returned Check/NSF Fee**.
    
4.  Optionally enter a sales description to explain how this item is intended to be used.
    
5.  On the **Sales/Pricing** subtab, for **Base Price**, enter the amount you charge for returned checks in the **Amount** column.
    
6.  On the **Accounting** subtab, in the **Income Account** field, select the account to which income from this fee will post.
    
7.  Select a tax schedule for this item.
    
8.  Click **Save**.
    

For additional details on creating these items, read [Other Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249208.html).

## Bill the Customer for the Returned Check/NSF Fee {#procedure_N1295992}

Bill the customer for the returned check/NSF fee in one of two ways:

-   Add the returned check/NSF fee to the original invoice.
    
    1.  Go to _Billing > Sales > Create Invoices > List_.
        
    2.  Click Edit next to the invoice that you are adding the fee to.
        
    3.  On the Items subtab, click the Items subtab.
        
    4.  In the Item field, select the Returned Check/NSF item that you created.
        
    5.  Click Add.
        
    6.  Click Save.
        
-   Create a new invoice that includes only the item for returned check or NSF fee.
    
    1.  Go to _Billing > Sales > Create Invoices_.
        
    2.  Select the customer and complete any other necessary information.
        
    3.  On the Items subtab, click the Items subtab.
        
    4.  In the Item field, select the Returned Check/NSF item that you created.
        
    5.  Click Add.
        
    6.  Click Save.
        

Note:

If the bank charged you a fee for the returned check, enter this charge as an Other Charge when you reconcile your bank statement. For more information, read [Reconciling Bank Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1552329.html).

### Related Topics:

-   [Handling Returned/NSF Checks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295030.html)
-   [Correcting Account Balances for NSF Checks Using a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1295419.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
