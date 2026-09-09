---
id: "section_N558109"
type: "section"
title: "Preferred Transaction Delivery on Customer and Vendor Records"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Preferred Transaction Delivery on Customer and Vendor Records"
parent: "chapter_N545359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N558109.html"
anchors: ["procedure_N558173"]
sha256: "6456754421a3e9251c8d08dcffc2a665dfdb87dda15f175d63ca6b500e357997"
---

Because each customer and vendor can have an individual preference for how to receive transactions, you can set a preferred transaction delivery method on their records as the default way to deliver transactions to them.

NetSuite automatically generates transaction email whenever the following records are saved:

| Blanket Purchase Order | Cash Refund | Cash Sale | Credit Memo |
| --- | --- | --- | --- |
| Estimate | Invoice | Opportunity | Purchase Contract |
| Purchase Order | Request For Quote | Requisition | Return Authorization |
| Revenue Commitment | Revenue Commitment Reversal | Revenue Contract | Sales Order |
| Transfer Order | Vendor Request For Quote | Work Order |  |

On each customer and vendor record, define the entity's preferred way to receive transactions: by regular mail (printing), by email, by fax, or by a combination of the three. Then, the preferred delivery method is marked by default in the following situations:

-   on transactions when you select that customer or vendor
    
-   on transactions created from that customer or vendor record
    
-   on transactions that are copied or converted from a transaction that uses these settings
    
    For example:
    
    -   If you click Make Copy on an invoice, then the delivery preferences default from the customer record on the new copy of the invoice.
        
    -   If you click Bill on a sales order, then the delivery preferences default from the customer record on the bill that is created.
        

#### To define the preferred transaction delivery method on entity records: {#procedure_N558173}

1.  Open the entity record.
    
    -   For Customers: Go to _Lists > Relationships > Customers > New_. Click **Edit** next to the customer whose record you want to update.
        
    -   For Vendors: Go to _Lists > Relationships > Vendors > New_. Click **Edit** next to the vendor whose record you want to update.
        
2.  Click the **Preferences** subtab.
    
3.  Next to **Send Transactions Via**, check the appropriate boxes:
    
    -   **Email** - Check this box to check the **To Be Emailed** box by default on transactions when this entity is selected.
        
    -   **Print** - Check this box to check the **To Be Printed** box by default on transactions when this entity is selected.
        
    -   **Fax** - Check this box to check the **To Be Faxed** box by default on transactions when this entity is selected.
        
4.  Click **Save**.
    

After you save these settings on their record, these boxes are checked by default.

Note:

These settings override any customized settings on transaction forms you use.

For more information about printing and emailing transactions, see [Printing Checks and Other Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566722.html) and [Emailing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N513303.html).

You can also set values these fields using the Mass Update function. For information, see [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

### Related Topics

-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Entering Transaction Line Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html)
-   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
-   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
-   [Tips for Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551712.html)
-   [Finding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560124.html)
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)
-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Transaction Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569351.html)
-   [Transaction Detail Workbook Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156465780853.html)
-   [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
