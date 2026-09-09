---
id: "section_N1665126"
type: "section"
title: "Processing Payments"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Processing Payments"
parent: "chapter_N1585433"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665126.html"
anchors: []
sha256: "ddff9566cf93d9b6e1640612e5aaaeb5df5754f96f0eadf8b7bda166eb0741b3"
---

The Electronic Bank Payments SuiteApp enables you to generate payment files for vendor bills, employee expenses, customer refunds, and customer payments. It also supports term or early payment discounts and credit applications. The payment files contain instructions for facilitating fund transfers between bank accounts. You can send these payment files to your bank or your customer's bank for processing.

Note:

Specific permissions are required to process discounts and credit applications. For more information, see [Setting Up Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1586829.html).

Review the following limitations and guidelines when processing transactions through Electronic Bank Payments:

-   Electronic Bank Payments currently processes up to 5,000 open payment transactions for bills, invoices, or customer refunds at a time. If you have more than 5,000 payment transactions, you can process the first 5,000 transactions and then proceed with the remaining ones.
    
    For payment transactions using SEPA Direct Debit, Electronic Bank Payments can process up to 1,500 open payment transactions for invoices. For more information about the maximum transactions that can be processed per template, see [Creating a New Custom Payment File Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4002284424.html).
    
-   There is a limit of 10,000 open transactions that you can process per vendor, customer, partner, and employee. If this limit has been exceeded, only the first 10,000 open transactions are included for electronic bank payment. The payment file administration record is tagged with incomplete payments.
    
    For more information about transaction limits, see [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html).
    
    -   You can define a Transaction type saved search to retrieve all open transactions for an entity and determine if the limit has been exceeded. To create a saved search, go to Lists > Search > Saved Searches > New. See the following sample filtering criteria to retrieve all open bills for a specific vendor's account:
        
        -   **Type** filter setting is **Bill**
            
        -   **Name** filter setting is the vendor's name
            
        -   **Status** filter setting is **Bill:Open**
            
        -   **Main Line** filter setting is **Yes** or true
            
        -   **Account** filter setting is the vendor's account
            
        
        For more information about creating saved searches, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
        
    -   You can reduce the number of open vendor bills by placing a hold on those that are not yet due for payment. After you have generated the payment files, you can remove the hold on the bills.
        
-   Processing through electronic bank payment overrides other default payment methods that have been set on entity records, to prevent multiple payment processing.
    
-   When it takes too long to load transactions on a Payment Processing page, the following notice is displayed as a fail-safe to prevent time-out errors:
    
    **Notice**: Additional transactions match your criteria and will be available for display after this selection is processed.
    
    The notice is displayed on the **Select Transactions** subtab when the first set of transactions have been loaded to the list. You can process transactions that have not been loaded separately, after processing of the initial set has been completed.
    
-   Use the Electronic Bank Payments to generate files with payment instructions that you can send to your bank. The Electronic Bank Payments doesn't transmit payment files to the banks. Contact your bank for information about transmitting payment files using their EFT systems.
    
-   Electronic Bank Payments can only process one payment file at a time if multi-queue is not set. PFA is automatically set to one of the following status unless there is any unexpected error due to external factors.
    
    -   Failed
        
    -   Processed
        
    -   Processed with Errors
        
    -   Cancelled
        
-   Exclude invoice and credit memo transactions from electronic payments processing by checking the **Exclude from Electronic Bank Payments Processing** box. This box is available on Invoice, Credit Memo, and Sales Order records.
    

See the following topics on electronic bank payment processing:

-   [Processing Bills and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665255.html)
    
-   [Processing Customer Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1667516.html)
    
-   [Processing Payments from Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1668006.html)
    
-   [Using Instant Electronic Bank Payment File Creation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4754712845.html)
    

### Related Topics

-   [Setting Up Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3831186542.html)
-   [Setting Up Bank Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html)
-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Creating Payment Files from Transactions for Electronic Bank Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4689182781.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
