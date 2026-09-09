---
id: "section_N550610"
type: "section"
title: "Entering Transaction Line Items"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Entering Transaction Line Items"
parent: "chapter_N545359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html"
anchors: ["subsect_162003757652", "procedure_N550652", "subsect_162003760258", "procedure_N550696"]
sha256: "3f8cc1201f1e1c16ee93ec7e88aa44ebc56e88fb9d7702ee944ade4a81f3f2fe"
---

Most transactions require you to enter one or more line items to account for the transaction total. Line items you enter determine the changes that post in NetSuite when you process the transaction. For example, when you enter line items on an invoice and post it, the inventory total decreases and the accounts receivable total increases, reflecting account changes for that transaction.

Note:

The limit for transactions submitted through the user interface is 500 lines. For transactions submitted through CSV import, REST and SOAP web services, the limit is 5,000 lines per transaction. After you submit transactions exceeding the 500 lines limit through the CSV import or SOAP web services, you must do all additional changes and edits through the CSV import or SOAP web services.

For journal entries, these limits are 1,000 lines for the user interface, REST web services and for synchronous SOAP web services, and 10,000 lines for CSV import and asynchronous SOAP web services.

You should limit yourself to 200 lines or less on a purchase order unless they're to be received by WebServices.

Note:

Processed lines for some transaction types contribute to the Monthly Transaction Lines metric that counts toward maximum limits for your NetSuite service tier. For more information, see [Transaction Types Included in Monthly Transaction Lines Metric](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160311737279.html).

The method for entering line items depends on the type of transaction you're creating. Line-item information is entered by either selecting and entering data and adding as a line item, or by selecting lines with check boxes.

## Entering Line Items by Entering Data {#subsect_162003757652}

In the following procedure, you see how to select and enter data and add them as a line item.

#### To enter line items by entering data: {#procedure_N550652}

1.  Add the line-item information to the form.
    
2.  Click **Add** to add the information as a line item.
    
    The transaction total is updated in the header as you add each line item, and a new, empty line is added.
    
3.  Add more line items as necessary.
    
4.  Click **Save**.
    

## Entering Line Items by Selecting Lines From a List {#subsect_162003760258}

In the following procedure, you see lines of data, each with a box on the left. Many pages have data-entry fields on the line.

#### To enter line items by selecting them from a list: {#procedure_N550696}

1.  Check the box next to the line you want.
    
2.  If there are data fields, enter values into them.
    
3.  Repeat Steps 1 and 2 until you've chosen all your line items.
    
    The transaction total is updated in the header as you check each line item.
    
4.  Click **Save**.
    

To change a line item, click on the line in the list. When the line-item data appears in the center of the page, make your changes and then click Edit.

To remove a line item, click on the line in the list and then click Remove.

If you use the U.S. Version of NetSuite, you can charge taxes on a line item basis. For more information, see [Setting U.S. Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2038835.html).

### Related Topics

-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
-   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
-   [Tips for Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551712.html)
-   [Finding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560124.html)
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)
-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Preferred Transaction Delivery on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N558109.html)
-   [Transaction Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569351.html)
-   [Transaction Detail Workbook Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156465780853.html)
-   [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
