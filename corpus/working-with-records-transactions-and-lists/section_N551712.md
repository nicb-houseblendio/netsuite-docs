---
id: "section_N551712"
type: "section"
title: "Tips for Working with Transactions"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Tips for Working with Transactions"
parent: "chapter_N545359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551712.html"
anchors: ["bridgehead_158088948106", "bridgehead_158088949400", "bridgehead_158088950779", "bridgehead_158088952609", "bridgehead_158088953978", "bridgehead_158088954777", "bridgehead_158088955661", "bridgehead_158088959006", "bridgehead_158088960786"]
sha256: "47e373f05aa52755ab7e4d05dc63b3b705f9c5334676d6ea2f8fb64e9bc8a209"
---

Refer to the following sessions for tips when working with transactions:

-   [Customize](#bridgehead_158088948106)
    
-   [Use Options](#bridgehead_158088949400)
    
-   [Print, Fax, Email, and Copy](#bridgehead_158088950779)
    
-   [Memorize](#bridgehead_158088952609)
    
-   [Maintain](#bridgehead_158088953978)
    
-   [Close](#bridgehead_158088954777)
    
-   [View the General Ledger](#bridgehead_158088955661)
    
-   [Use Shortcuts & Keyboard shortcuts](#bridgehead_158088959006)
    
-   [Get help](#bridgehead_158088960786)
    

## Customize {#bridgehead_158088948106}

-   Most transaction forms can be customized by using the **Customize** menu at the top of the page. The appropriate permission is required to customize the form. If you don't see the **Customize** menu, your current role doesn't include the permission.
    
-   Click **List** to open a list of all transactions of a specific type. From these lists, you can view and edit transactions, print and export your lists, and go to transactions' registers. Your customization of the viewing and sorting of the list will retain for the future views. You can change the list sorting by clicking another column heading.
    
-   Amount fields in transactions and records support computation. For more information, see [Amount Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N547812.html#section_N553441).
    

## Use Options {#bridgehead_158088949400}

-   Some fields on transaction forms display a double arrow button that you can click for the **List**, **Search**, and **New** options:
    
    -   Click **List** to display a popup list of stored records from which to choose.
        
    -   Click **Search** to search for a record.
        
    -   Click **New** to open a window and create a new record for that field.
        
-   On transactions and records that have buttons with a dropdown list, you can select a different button option. Use the Tab key to go to the dropdown button. Then use the Down Arrow key to expand the dropdown list. Click Enter to select the desired action. To collapse the dropdown list, use the Up Arrow key.
    
    For more information, see [Popup and Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474536.html) and [Buttons and Menus in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180852421.html).
    

-   Click **Add Multiple** in the **Items** subtab to open the Choose Item window. This window displays a list of items you can add. You can filter the list by item type or search for all or part of a name. When you click an item in the left pane, it's added to the right pane, where you can enter a quantity for the item. When you click **Done**, items and quantities shown in the right pane are added to the transaction.
    

## Print, Fax, Email, and Copy {#bridgehead_158088950779}

-   When you post a transaction, you can print, fax, or email a copy of the form:
    
    -   Check the **To Be Printed** box to save the form in a queue for printing later.
        
    -   Check the **To Be E-mailed** box and enter or verify an email address to email the form.
        
    -   Check the **To Be Faxed** box and enter or verify a fax number to fax the form.
        
    
    Administrators configure the fax and print setup at _Setup > Company > Preferences > Printing & Fax (Administrator)_. For more information, see [Setting Printing and Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253916.html).
    
    Administrators configure the e-mail setup at _Setup > Company > Email > Email Preferences (Administrator)_. For more information, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html).
    
-   When you view a transaction, you can make a copy of the transaction:
    
    -   From the **Actions** list, select **Make Copy** to replicate all the information from the original transaction and link it to the original transaction.
        
        For example, if you create an invoice from a sales order, the value in the **Created From** field is copied to the new transaction. The new transaction is also displayed in the history of the original transaction.
        
    -   From the **Actions** list, select **Make Standalone Copy** to make a copy of the original transaction that includes inventory costing but isn't associated with the original.
        
        For example, click **Make Standalone Copy** on a transactionw that uses advanced shipping to create a cash sale or invoice that has the same items as the original and includes the cost of good sold (COGS) account impact in addition to revenue. Because a standalone copy isn't linked to the original, it doesn't retain the value in the **Created From** field. The new transaction isn't part of the history of the original transaction and is considered a brand new transaction.
        

## Memorize {#bridgehead_158088952609}

Memorize a transaction to recall and use it again later. To memorize a transaction, go to the transaction type you want to memorize. Add the appropriate information to the form. From the **Actions** list, select **Memorize**. The Memorized Transaction page opens showing the information you entered. For more information, see [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html).

## Maintain {#bridgehead_158088953978}

-   To maintain performance, the limit for transactions submitted through the user interface is 500 lines. For transactions submitted through CSV import or SOAP web services, the limit is 5,000 lines per transaction.
    
-   For journal entries, the limit is 1,000 lines for the user interface and for synchronous SOAP web services, and 10,000 lines for CSV import and asynchronous SOAP web services.
    

For more information, see [Entering Transaction Line Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html).

## Close {#bridgehead_158088954777}

-   Close a line item on a transaction if you don't expect to fulfill or receive the item. To close a line item on a transaction, click **Edit** on the transaction. Click the line you want to close and then check the **Closed** box. Click **Done** and then click **Save**.
    
-   Close an entire transaction so that it no longer has an open status. When you view sales orders, purchase orders, and return authorizations, click **Close** to check the **Closed** box for all lines on the transaction. Then when you click **Save**, the transaction is no longer open.
    

## View the General Ledger {#bridgehead_158088955661}

To view the general ledger results of posting transactions, from the **Actions** list, select **GL Impact**. The details of the general ledger impact of lines on the originating transaction are displayed.

## Use Shortcuts & Keyboard shortcuts {#bridgehead_158088959006}

-   Use the **Shortcuts** menu to place a shortcut link on your home page to frequently-used transactions. For more information, see [Navigation Menu](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4323290738.html).
    
-   Transactions support many of the same keyboard shortcuts as other records. When using tabbed display, you can switch between subtabs by using keyboard shortcuts. Each subtab has a single letter underlined in the title. Press and hold the **Alt** key on your keyboard and then press the corresponding letter to switch to that subtab. The first field on the subtab is automatically selected. For information, see [Keyboard Shortcuts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474926.html).
    

## Get help {#bridgehead_158088960786}

-   Click the **Help** link at the top of the page to get help specific to the transaction you're working with.
    
-   Click the **field name** to display a popup window with field level help.
    

Important:

When processing transactions in bulk, you must submit one page at a time. If you don't process each page individually, information isn't retained and can be lost when you click a different page.

### Related Topics

-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Entering Transaction Line Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html)
-   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
-   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
-   [Finding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560124.html)
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)
-   [Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html)
-   [Preferred Transaction Delivery on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N558109.html)
-   [Transaction Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569351.html)
-   [Transaction Detail Workbook Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156465780853.html)
-   [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
