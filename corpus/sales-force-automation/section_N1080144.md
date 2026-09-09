---
id: "section_N1080144"
type: "section"
title: "Managing Customer Credit Limits and Holds"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Customers > Creating a Customer Record > Entering Financial Information for the Customer > Managing Customer Credit Limits and Holds"
parent: "section_N1078064"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1080144.html"
anchors: []
sha256: "cd5886e544b6bb0db42cedbf2873eb4caa1b2f650f0e149155e9a610feb9557a"
---

You can use credit limits and credit holds to manage how much credit you're giving your customers. If a customer is delinquent on payments or reaches a pre-set credit limit, NetSuite can restrict the entry of new sales transactions on credit. The customer's restricted on new orders until they pay the invoices due, or you manually release the hold.

The credit limit you set for a customer doesn't include any of the customer's subcustomers. The customer may reach its credit limit, but you can continue to create sales transactions for its subcustomers without restrictions. For more information see [Creating a Subcustomer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1085616.html).

To use credit limits and holds, you set credit limits on customer records. A credit limit defines the maximum amount the customer is allowed to accrue in outstanding receivables.

The Customer Credit Limit Handling accounting preference determines the grace period for overdue invoices and what happens when customers exceed their credit limit. For more information, see [Credit Limit Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4490498729.html).

When credit limits are enforced, a credit hold restricts entry of a new sales transaction under the following circumstances:

-   **Credit limit reached** - When the customer's preset credit limit is exceeded, the credit hold is applied automatically. The customer must settle one or more outstanding invoices to reduce the balance due and release the credit hold.
    
-   **Delinquent payments** - A payment is delinquent when a customer's Overdue Balance has exceeded the grace period in the Days Overdue for Warning/Hold accounting preference.
    
-   **Credit hold applied manually** - The **Hold** field on the customer record is set to **On**. NetSuite ignores the assigned credit limit. You're restricted from placing an order for the customer even if the credit limit hasn't been reached. You must release a manual credit hold to permit the customer to create orders.
    

#### To manage customer credit limits and holds:

1.  Go to _Lists > Relationships > Customers_.
    
2.  Click **Edit** next to the customer name.
    
3.  Click the **Financial** subtab.
    
4.  In the **Credit Limit** field, enter the customer's maximum amount of credit for the purchase of goods or services.
    
    If you use the Multiple Currencies feature, the credit limit you enter on the customer record uses the customer's primary currency. This is the total credit limit for all of the customer's transaction currencies. If you change a customer's primary currency, you'll need to re-enter the credit limit in that new currency. For more information, see [Assigning Currencies to Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html).
    
5.  In the **Hold** field, select a credit hold setting from the following options:
    
    -   **Auto** - Credit warnings and blocks are applied according to the customer's credit limit and the Credit Limit Handling accounting preference. For details, see [Credit Limit Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4490498729.html) and [Credit Limit Warnings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4490500811.html).
        
        This is the default option for new customer records.
        
    -   **On** - Puts the customer on hold and stops them from buying on credit regardless of the **Credit Limit** value and customer balance. This option is sometimes called a manual credit hold.
        
    -   **Off** - Disables credit limits and credit holds for the customer. NetSuite ignores the customer's **Credit Limit**, and the customer can purchase goods of any value on credit.
        
6.  Click **Save**.
    

### Related Topics

-   [Entering Financial Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1078064.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1083860.html)
-   [Tracking Customer Credit Card Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1084186.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
