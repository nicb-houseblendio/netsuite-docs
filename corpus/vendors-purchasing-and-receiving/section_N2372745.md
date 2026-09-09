---
id: "section_N2372745"
type: "section"
title: "Posting Vendor Bill Variances"
branch: "vendors-purchasing-and-receiving"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Vendors, Purchasing, and Receiving > Vendors > Vendor Bills > Vendor Bill Variances > Posting Vendor Bill Variances"
parent: "section_N2371184"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2372745.html"
anchors: ["procedure_N2372780", "bridgehead_N2372928", "bridgehead_N2372968"]
sha256: "29e4343e1680f6913fbe6b5350f975fb4e0870f96edd69854742dd4364c0495a"
---

After you have associated item records with variance accounts, you can create variance journal postings. For information about ways to create variance postings, see [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html). Then, after your transactions are set to create variance postings, you can create variance journal entries on the Post Vendor Bill Variances page.

Note:

These journal entries address variances only for inventory, non-inventory, other charge, and service items.

#### To post a variance journal entry: {#procedure_N2372780}

1.  Go to _Transactions > Payables > Post Vendor Bill Variances_.
    
    Note:
    
    Vendor bills in pending approval status appear on this page because the quantity buckets must be allocated so that NetSuite properly operates. This also helps you prevent over billing.
    
2.  On the Post Vendor Bill Variances page, verify or select the posting period for the journal entry you are creating.
    
3.  Verify or enter the date for the journal entry. The current date automatically fills this field.
    
4.  If you have a NetSuite OneWorld account, select a subsidiary from the list in the **Subsidiary** field.
    
    If your vendor records are shared with multiple subsidiaries, the item records that can be posted reflect the combination of selected vendor and subsidiary. For more information about globally shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
    
5.  In the **Transaction Type** field, make a selection to filter the list of transactions:
    
    -   Choose **Purchase Order** to show closed purchase order lines with a variance that do not have the **Match Bill To Receipt** box checked.
        
    -   Choose **Bill** to show only vendor bills linked to Purchase Orders that have the **Match Bill To Receipt** box checked.
        
6.  When you have selected **Bill** in the **Transaction Type** field, you can make a selection in the **Transaction Status** field:
    
    -   Choose **Open** to show all open vendor bills.
        
    -   Choose **Paid in Full** to show only vendor bills that are completely paid.
        
7.  In the **Vendor** field, select a vendor to filter the list to show only transactions associated with the selected vendor.
    
8.  Clear the **Include Bills Without Receipts** box to exclude bills from the list that have no item receipts entered against them. Check this box to include all bills regardless of receipts.
    
9.  Check the box in the **Select** column next to all transactions you want to create a variance journal entry for.
    
10.  Click **Create Journal Entries**. The Post Vendor Bill Variances Results page opens and shows the journals created by the entry. You can click the link to open the journal and see the lines posted.
     

For information about the journals created for variances, see [Vendor Bill Variance Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373098.html).

Important:

After the variances on the journal entry are created and posted, associated purchase orders, receipts, and vendor bills transactions can"t be changed.

The variance journal entries must be voided or deleted to allow changes to associated transactions. Also, the accounting period must be open for the entries being considered and the A/P must be unlocked.

## Vendor Bill Variances Status Page {#bridgehead_N2372928}

To view the status of vendor bill variance calculations you are performing, go to _Transactions > Payables > Post Vendor Bill Variances_. This page displays the date and time the variance journal was created. It also provides the processing percentage complete, and a link to the results of completed journals in the Status column.

## Vendor Bill Variances Results Page {#bridgehead_N2372968}

The Post Vendor Bill Variances Results page is displayed in the following two ways:

-   After you click Create Journal Entries on the Post Vendor Bill Variances page
    
-   When you click the Complete link in the Status column of the Post Vendor Bill Variances Status page
    

Post Vendor Bill Variances Results page displays the following information:

-   The transaction type that the journal was created from, which is a link to open the transaction
    
-   The item on the transaction that had a variance calculated
    
-   The number of the journal entry created, which is a link to open the journal
    
-   The total amount posted by the journal
    

To view individual lines posted by the journal, click the journal number to open the entry. For more information, see [Vendor Bill Variance Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373098.html).

### Related Topics

-   [Vendor Bill Variance Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373098.html)
-   [Mass Updates for Variance Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2373402.html)
-   [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
