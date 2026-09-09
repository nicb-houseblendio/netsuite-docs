---
id: "section_N1732506"
type: "section"
title: "Posting VSOE Revenue to the General Ledger"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Posting VSOE Revenue to the General Ledger"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html"
anchors: ["bridgehead_4071710047"]
sha256: "2c5f06bd686e83f72ddf322d9f66be8144087acee6e6efbb7b7589c16f3465f8"
---

When revenue is recognized for items not sold as a vendor-specific objective evidence (VSOE) bundle, the invoice price is the amount that posts to the assigned deferred revenue account for each line with a revenue recognition schedule. When revenue is recognized for a VSOE transaction, the VSOE allocation amount (not the sales amount) posts to the assigned deferred revenue account.

For example, you sell the following items:

-   Service Item A1
    
    -   Deferred revenue account = Deferred Revenue (Service)
        
    -   Invoice price = $300
        
-   Product Item B2
    
    -   Deferred revenue account = Deferred Revenue (Product)
        
    -   Invoice price = $600
        

When these items **aren't** sold as a VSOE bundle, the desired general ledger impact is as follows:

Accounts Receivable $900

Deferred Revenue (Service) $300

Deferred Revenue (Product) $600

On another transaction, the items **are** sold as a VSOE bundle. The VSOE allocation is as follows:

-   Service Item A1
    
    -   Deferred revenue account = Deferred Revenue (Service)
        
    -   Invoice price = $300
        
    -   VSOE allocation = $225
        
-   Product Item B2
    
    -   Deferred revenue account = Deferred Revenue (Product)
        
    -   Invoice price $600
        
    -   VSOE allocation = $675
        

When these items **are** sold as a VSOE bundle, the desired general ledger impact is as follows:

Accounts Receivable $900

Deferred Revenue (Service) $225

Deferred Revenue (Product) $675

To achieve the desired general ledger impact and properly recognize VSOE amounts, NetSuite posts to the ledger as follows:

1.  The sales amount posts to the deferred revenue account.
    
2.  The sales amount is reversed out of the deferred revenue account.
    
3.  The VSOE allocation amount posts to the deferred revenue account.
    

Applying these steps to the previous examples, the VSOE sale would post to the general ledger as follows:

## Accounts Receivable $900 {#bridgehead_4071710047}

-   Deferred Revenue (Service) $300
    
-   Deferred Revenue (Product) $600
    
-   Deferred Revenue (Service) $300 \[VSOE reversal\]
    
-   Deferred Revenue (Product) $600 \[VSOE reversal\]
    
-   Deferred Revenue (Service) $225 \[VSOE allocation\]
    
-   Deferred Revenue (Product) $675\[VSOE allocation\]
    

Note:

When you view the General Ledger Impact page for a VSOE transaction, you may see lines that show these reversal postings.

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
