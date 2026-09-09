---
id: "section_N433632"
type: "section"
title: "Single Journal Entry Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Simple Imports > Single Journal Entry Import"
parent: "section_N433480"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html"
anchors: ["bridgehead_N433782"]
sha256: "b712203f4b60bdeab0d716fac42ca0354d3ce4cf1f6c2e6a0a06d898ece3c6a8"
---

You can use the Single Journal Entry Import Assistant to import a single journal entry's data from an external system into NetSuite. The Single Journal Entry is available in _Transactions > Financial > Make Journal Entries > Import_. If you use NetSuite OneWorld, you can use a similar assistant to import data from a single intercompany journal entry.

You need the Make Journal Entry and Posting Period on Transactions permissions to import a single journal entry. You don't need the Import CSV File permission.

Important:

The Single Journal Entry Import Assistant preserves the journal entry import process available prior to Version 2010 Release 1, with a modified user interface. More complex journal entry import functions are also available. See [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html) and [Advanced Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498465157.html).

The Single Journal Entry Import Assistant is available at _Transactions > Financial > Make Journal Entries > Import_. For intercompany journal entries, a similar assistant is available at _Transactions > Financial > Make Intercompany Journal Entries > Import_. For advanced intercompany journal entries, a similar assistant is available at _Transactions > Financial > Make Advanced Intercompany Journal Entries > Import_.

If you're using statistical accounts, the Single Journal Entry Import Assistant is available at _Transactions > Financial > Make Statistical Journal Entries > Import_. For information about statistical accounting, see [Statistical Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3842142868.html).

The Assistant includes the following steps:

-   The first page of the Single Journal Entry Import Assistant provides a link to a CSV journal entry template file that is identical to the template for the previously available journal import process.
    
    -   Click this link to download the template file and populate it with your data.
        
        Note that you can add columns to your CSV file for journal entry fields that aren't included in the template, if you want to import data for these fields.
        
        For more information, see [Supported Values for Journal Entry Import CSV Files](#bridgehead_N433782).
        
    -   After you have a CSV file with data in it, click the Select button in the Import Assistant and select your file, then click Next.
        
-   The Assistant automatically maps fields in your CSV file to NetSuite journal entry fields and lets you view these mappings.
    
    -   You can simply click Run to accept the default mappings and immediately start the import.
        
    -   Or, you can make changes: You can move fields to change or add mappings. Also, you can click the edit icon for a field to open a popup where you can set a default value.
        
    -   Note that if you don't map or set defaults for the Date and Entry No. fields, the import process provides defaults.
        

After you click Run and the import process completes, the newly created journal record displays. The Entry No. field shows the journal entry number for the transaction.

If errors prevent the process from completing, a status page displays instead. Note that, unlike other imports, an email notification isn't sent for single journal entry import.

## Supported Values for Journal Entry Import CSV Files {#bridgehead_N433782}

For ease of use and compatibility with the previous journal import, the following values are supported in your CSV files:

-   For **Account** - If the Use Account Numbers preference is enabled, Account field values should include both numbers and names, such as **11000 Accounts Payable**. Number-only values, such as **11000**, are also supported. Name-only values, such as **Accounts Payable**, aren't supported when this preference is enabled. If this preference isn't enabled, name-only values should be used.
    
-   For (Entity) **Name** - If auto-generated numbering is enabled, you should make sure that Name field values include both entity ID and name, such as **A2255 ABC Company**. ID-only values, such as **A2255**, also are supported.
    
-   For **Account, Class**, **Department, Location**, and **Subsidiary** - Most CSV imports require the use of the full hierarchical name, but journal entry import supports the use of the simplified name. For example, for location name, both **California : Los Angeles** and **Los Angeles** are supported.
    

For more information about supported CSV file fields, see [Journal Entry and Intercompany Journal Entry Header Fields Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534492479.html) and [Journal Entry and Intercompany Journal Entry Line-Level Fields Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1534492737.html).

Important:

Import is supported for journal entries with up to 10,000 lines. However, poor performance results during import and in the user interface for journal entries with over 1000 lines, and these large journal entries may not be editable in the user interface.

For more information about journal entries, see the following.

-   For step-by-step instructions for importing a single journal entry, see [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html).
    
-   For more information about working with journal entries, see [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html).
    
-   To import multiple journal entries, see [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html).
    

### Related Topics

-   [Simple Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
