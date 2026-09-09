---
id: "section_N564245"
type: "section"
title: "Memorized Transactions"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Transactions > Memorized Transactions"
parent: "chapter_N545359"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564245.html"
anchors: []
sha256: "43c4784449388670090fee1418612add0b84aa1bbb175a27224e80966c7f3129"
---

Note:

To work with memorized transactions, you need a View level of the Memorized Transactions permission.

A memorized transaction is a transaction you set up to recur in NetSuite, such as recurring journal entries. Memorized transactions eliminate data entry and serve as useful reminders. A memorized transaction consists of two parts:

-   The **Memorized Transaction Template** defines the transaction to be created.
    
-   The **Memorized Transaction Definition** sets the parameters for when to create the transaction, whether they're recurring, and how many transactions to create.
    

When you memorize a transaction, you set up the transaction to recur over time. You choose whether the transaction automatically posts or if you're reminded to post it. Set the frequency the transaction should occur and set posting options. You can specify that the transaction should recur forever or a set number of times.

When you edit or delete a memorized transaction, the change is tracked on the system notes of the memorized transaction.

The following are limitations for posting memorized transactions in locked and closed periods:

-   A user must have the Override Period Restrictions permission to enable the Allow Posting in Locked Period option for a memorized transaction. When this option is enabled, memorized transactions can post in locked periods even if users initiating these transactions don't have the Override Period Restrictions permission.
    
-   Transactions can never be posted in closed periods. If the posting date for a memorized transaction is in a period that has been closed, it's posted to the next open period.
    

In NetSuite, you can memorize the following transactions:

-   Checks
    
-   Deposits
    
-   Credit Cards
    
-   Purchase Orders
    
-   Bills
    
-   Sales Orders
    
-   Invoices
    
-   Estimates
    
-   Cash Sales
    
-   Journal Entries
    
-   Statement Charges
    
-   Work Orders
    
-   Purchase Requisitions
    
-   Transfer Orders
    
-   Opportunities
    
-   Custom Transactions
    

The Reminders portlet includes a standard reminder for Memorized Transactions due. For more information, see [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html).

After you've memorized a transaction, you can view and manage transactions created by the memorized transaction by going to _Transactions > Management > Enter Memorized Transactions_. Click **Edit** next to the transaction. The Transactions subtab shows associated transactions.

The time when the system runs memorized transactions varies by location, but it's usually shortly after midnight each day. The system checks for memorized transactions every four hours, and processes them according to the start date. If the start date is the current day, the system processes the transaction immediately, and then at the usual time each day afterward. If the start date is in the future, the system processes the transaction at the usual time on that future date, and each day afterward. If the start date is in the past, the system processes a transaction for each past day every four hours until caught up to the current day, then processes a transaction at the usual time each day afterward.

By default, when NetSuite creates a memorized transaction automatically, it lists the last user who edited the memorized transaction definition as the user who created the transaction. This user is visible in the memorized transaction definition. To list the user as -System- for automatic memorized transactions, set the **Create Automatic Memorized Transactions as -System-** preference at _Setup > Company > Preferences > General Preferences (Administrator)_. Changes to this preference take effect when you create a new memorized transaction definition or you edit and save an existing one. For more information, see [Setting General Account Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243797.html).

Note:

When set, this preference doesn't support server-side scripting. If you want to use server-side scripting and SuiteFlow on transactions, disable the preference.

For specific instructions, see the following topics in this section:

-   [Memorizing a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N564637.html)
    
-   [Submitting Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N565877.html)
    
-   [Editing Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566256.html)
    
-   [Customizing the Memorized Transactions List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564424.html)
    
-   [Viewing the Status of Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N564455.html)
    
-   [Deleting Memorized Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N566525.html)
    

### Related Topics

-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Creating Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N546079.html)
-   [Entering Transaction Line Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N550610.html)
-   [Entering Relationships on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586861907.html)
-   [Entering Communication Information to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4586862223.html)
-   [Tips for Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551712.html)
-   [Finding Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N560124.html)
-   [Voiding, Deleting, or Closing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N563543.html)
-   [Preferred Transaction Delivery on Customer and Vendor Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N558109.html)
-   [Transaction Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569351.html)
-   [Transaction Detail Workbook Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156465780853.html)
-   [Limits for Display of Transaction Lists and Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N569641.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
