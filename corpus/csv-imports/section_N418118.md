---
id: "section_N418118"
type: "section"
title: "Journal Entry Import and Intercompany Journal Entry Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Journal Entry Import and Intercompany Journal Entry Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html"
anchors: []
sha256: "102954280c5aecd91ee42f3212b6038fc4e5a6d668b9ed018cad0db43fff9664"
---

A journal entry records debits and credits to be posted to ledger accounts, adjusting the value of accounts. In NetSuite OneWorld, an intercompany journal entry records the impact of transactions between two subsidiaries. Intercompany journal entries identify both a 'from', or originating, subsidiary and a 'to', or receiving, subsidiary.

You can import multiple journal entries and, for NetSuite OneWorld, multiple intercompany journal entries, from another system into NetSuite. Each import job can include data for any combination of classes, department, locations, and for NetSuite OneWorld, subsidiaries. Journal entry import and intercompany journal entry import are two separate tasks in the Import Assistant. For information about importing advanced intercompany journal entries, see [Advanced Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498465157.html).

Note:

The Journal Entry and Intercompany Journal Entry record types have been enhanced with two fields: `Accounting Book` and `Is Book Specific`. Use these fields only in accounts that have the Multi-Book Accounting feature enabled to create book specific journal entries and book specific intercompany journal entries. If you have questions about Multi-Book Accounting, see [Multi-Book Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831567542.html) and [Using Multi-Book Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3831569045.html).

After journal entry data is in a CSV file, users with required permissions can start a journal entry import by going to _Setup > Import/Export > Import CSV Records_, selecting an Import Type of Transactions and a Record Type of Journal Entry (or Intercompany Journal Entry), and completing other Import Assistant pages.

Important:

To import a single journal entry, you can use a simpler import process available at _Transactions > Financial > Make Journal Entries > Import_. If you use NetSuite OneWorld, you can go to _Transactions > Financial > Make Intercompany Journal Entries > Import_ to import a single intercompany journal entry. See [Single Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html).

Import is supported for journal entries with up to 10,000 lines. However, poor performance results during import and in the user interface for journal entries with over 1000 lines, and these large journal entries may not be editable in the user interface.

See the following for more information about using the Import Assistant to import journal entries or intercompany journal entries.

-   [Permissions for Importing Journal Entries with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534489333.html)
    
-   [Journal Entry CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534489651.html)
    
-   [Journal Entry Import Supported Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534489954.html)
    
-   [Journal Entry and Intercompany Journal Entry Header Fields Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534492479.html)
    
-   [Journal Entry and Intercompany Journal Entry Line-Level Fields Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534492737.html)
    
-   [Using Journal Entry Import for Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534490251.html)
    
-   [Custom Form Specification for Journal Entry Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534490534.html)
    

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Single Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
