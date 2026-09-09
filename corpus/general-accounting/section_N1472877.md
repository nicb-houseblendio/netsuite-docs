---
id: "section_N1472877"
type: "section"
title: "Importing a Journal Entry"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Importing a Journal Entry"
parent: "chapter_N1468455"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html"
anchors: ["procedure_N1472932"]
sha256: "58a546466cfabc42fa40ef92ac0d1319ab160468541e936e9fc23f0a50be4699"
---

If you have the Make Journal Entry and Posting Period on Transactions permissions, you can import a single journal entry from an external system into NetSuite.

If you use NetSuite OneWorld, you can also import a single intercompany journal entry.

Import is supported for journal entries with up to 10,000 lines. You may notice a performance impact during import and in the user interface for journal entries with over 1000 lines. In addition, these large journal entries may not be editable in the user interface.

Note:

Journal entry and intercompany journal entry records include a **Memo** body field and a **Journal Entry - Line : Memo** field. When mapping:

-   If you include only a **Line Memo** or **Memo** field in your CSV file, it's mapped to the **Journal Entry - Line : Memo** field.
    
-   If you include both a **Line Memo** and **Memo** field in your CSV file, **Line Memo** is mapped to **Journal Entry - Line : Memo** and **Memo** is mapped to the **Memo** body field.
    

Auto-mapping works differently if you're using the CSV Import Assistant. For details on that method, see [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html).

#### To import a journal entry: {#procedure_N1472932}

1.  Go to Transactions > Financial > Make Journal Entries > Import.
    
    (To import an intercompany journal entry, go to Transactions > Financial > Make Intercompany Journal Entries > Import.)
    
2.  On the Import Assistant's Scan & Upload CSV File page, select the type of character encoding for imported data.
    
    For information about available options, see [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).
    
    For more information about the Import Assistant, see [Single Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html).
    
3.  Click the **Single Journal Entry Template File** link to download a CSV template file.
    
4.  Save the file to your system and then populate the saved file with your journal entry data. Note the following conditions:
    
    -   Each imported journal entry must include at least two lines and have balancing debits and credits.
        
    -   Each imported intercompany journal entry must include at four lines with one debit and credit for both the originating and receiving subsidiary.
        
    -   You can add columns to the file to import data for additional journal entry fields.
        
    -   For more information about supported CSV file values, see [Supported Values for Journal Entry Import CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html#bridgehead_N433782).
        
5.  Click **Select**, choose the CSV file you've populated and then click **Open**.
    
6.  Click **Next**.
    
7.  On the View Mapping / Start Import page, review the automappings of CSV file fields to NetSuite fields.
    
    Accept the default mappings and start the import, or make changes by dragging and dropping fields. You can also click the pencil icon to open a popup and set default values.
    
    If you don't map or set defaults for the **Date** and **Entry No.** fields, the import process provides default values.
    
    Note:
    
    If you want to know what the defaulted number is going to be for an imported statistical journal, you can check this value prior to the import by going to _Setup > Company > Auto-Generated Numbers_ > **Document Numbers** subtab > **Journal** field > **Current Number** column. For details about field mapping, see [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html) and [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html).
    
8.  Click **Run** to immediately start the import.
    
    When the import process successfully completes, the record created by the journal entry import displays. This page lets you immediately review import results.
    
    If an import doesn't successfully complete, a Job Status page appears. Click the **CSV Response** link to view a results.csv file that contains your CSV file data and the error message.
    
    Correct the error in your CSV file and then retry the import. For information about import errors, see [Journal Entry Import Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4570029068.html).
    

Note:

Users who have the **Import CSV File** permission can import multiple journal entries at one time and take advantage of additional import options. For details about this more complex capability, see [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html). For details about importing advanced intercompany journal entries, see [Advanced Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498465157.html).

### Additional Information

-   [Single Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433632.html)
-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html)
-   [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html)

### Related Topics

-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Journal Entries Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1468996.html)
-   [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html)
-   [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html)
-   [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html)
-   [Reversing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471552.html)
-   [Viewing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472027.html)
-   [Printing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472381.html)
-   [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html)
-   [Bad Debt Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481280.html)
-   [Writing Off Customer Overpayments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483085.html)
-   [Expense Allocation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html)
-   [Period End Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531269686.html)
-   [Balancing Segments and Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157358611227.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
