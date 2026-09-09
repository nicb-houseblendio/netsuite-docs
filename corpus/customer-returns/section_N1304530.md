---
id: "section_N1304530"
type: "section"
title: "Return Authorization (RMA) Forms"
branch: "customer-returns"
category: "order-management"
breadcrumb: "Order Management > Customer Returns > Customer Return Management > Return Authorization (RMA) Forms"
parent: "section_N1302852"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1304530.html"
anchors: ["bridgehead_4585520010"]
sha256: "2a6bd533fa84de8ff81657760b94509fc2ccc2497f2f520d3f66ba1d5972325d"
---

A return authorization form, also known as a return materials authorization (RMA), is a record of expected customer returns.

The return authorization holds information about the items you expect a customer to return, such as the item number or vendor item number and the quantity being returned. The authorization also tracks the price of items being returned and the amount to be credited or refunded to the customer.

Note:

This is a non-posting transaction.

Important:

The form you choose when you enter an authorization guides whether the return is processed as a refund or a credit, along with other account settings.

## Credit or Refund? {#bridgehead_4585520010}

Whether the return process results in a credit or a refund is dependent on three things:

-   Which return authorization form is selected in the Custom Form field on the authorization.
    
    Standard forms available include the following:
    
    -   **Standard Return Authorization - Credit** - A return using this form generates a credit memo for the returned item.
        
        The credit memo can later either be applied to an account balance or refunded to the customer.
        
    -   **Standard Return Authorization - Cash** - A return using this form generates a refund for the returned item.
        
        A cash form return authorization **cannot** later be processed as a credit memo.
        
-   Your setting for the [Refund in Advance of Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html#bridgehead_N1305083) preference.
    
-   Whether the **Advanced Receiving** feature is enabled.
    
    -   If you have enabled the Advanced Receiving feature, you must credit a return before you can refund a return.
        
        -   First, a credit is created from the return authorization in the authorized amount.
            
        -   Next, from the credit, a refund is created, also in the authorized amount.
            
        
        For more information, read [Receiving a Purchase Orders With Advanced Receiving](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2412119.html).
        
    -   If you do not use the Advanced Receiving feature, you can create a refund directly from an authorization without creating a credit memo first.
        
    
    Whether Advanced Receiving is enabled or not, you can always enter standalone credit memos that record credit on a customer account that can be applied toward their account balance. For more information about this type of customer credit memo, read [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html).
    

As you enter information to process the return, the return authorization keeps track of the status of return while accounting and inventory records are updated. This way, you can monitor accurate data to know which steps are completed and what to expect next.

For example, when the warehouse manager gets the item from the customer and marks the return authorization received, the accounting department sees the return authorization in their queue to be credited.

Note:

For help with filling out any of the required fields, click on the field name.

To begin the customer return process, issue the authorization. NetSuite offers two ways to issue a return authorization.

-   [Entering a Standalone Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305354.html).
    
    This creates a return authorization that isn't linked to a sale.
    
-   [Entering a Linked Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306234.html).
    
    This creates a return authorization from a cash sale or invoice including the items from the original sale that's linked to the original sale.
    

### Related Topics:

-   [Customer Return Management Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303478.html)
-   [Customer Returns Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1303799.html)
-   [Preferences for Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html)
-   [Entering a Standalone Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305354.html)
-   [Entering a Linked Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306234.html)
-   [Approving a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1306797.html)
-   [Printing a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307142.html)
-   [Processing Return Authorizations and Credit Transactions with a Different Location in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0708104225.html)
-   [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html)
-   [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html)
-   [Closing Line Items on a Customer Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1309679.html)
-   [Customer Return Authorization Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310133.html)
-   [Reporting on Customer Returns Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310580.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
