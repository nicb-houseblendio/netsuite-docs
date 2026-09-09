---
id: "bridgehead_N1501792"
type: "bridgehead"
title: "Running Intercompany Elimination"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Elimination Through the Automated Intercompany Management Feature > Running Intercompany Elimination"
parent: "section_N1501565"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501792.html"
anchors: ["procedure_N1501813"]
sha256: "1302da2b343e2f5694edd1275362c4c2abb3206c634afd6c9288ab73607a3c3c"
---

You can run the intercompany elimination process only from the Period Close Checklist. Ensure that you have completed all other period closing tasks before you run elimination. The Revalue Open Foreign Currency Balances and Calculate Consolidated Exchange Rates determine the gains and losses that post. These gains and losses post to the Cumulative Translation Adjustment - Elimination (CTA-E) account.

When you run elimination, NetSuite posts elimination journal entries. You can run intercompany elimination for a period multiple times, as needed. NetSuite doesn't support running multiple intercompany elimination process at the same time.

#### To run intercompany elimination: {#procedure_N1501813}

1.  From the Period Close Checklist, click the **Eliminate Intercompany Transactions** icon.
    
2.  Verify the **Period** is correct.
    
3.  Click **Run Intercompany Elimination**.
    
    Select a class, department, and location, if used. Optionally, add a memo.
    
    If you use Automated Intercompany Management and Multi-Location Inventory features, and the Make Location Mandatory accounting preference, note the following. You must assign a default elimination location to each elimination subsidiary. Then, on the Task: Eliminate Intercompany Transactions page, select the elimination subsidiary from the Location list. The default value is the Default Elimination Subsidiary Location. NetSuite assigns the elimination subsidiary to each intercompany elimination journal entry generated through completing this task.
    
    If you use Multi-Book Accounting, the read-only Accounting Book field displays the accounting book for which you are running intercompany transaction elimination.
    
4.  Click **Save** to run intercompany elimination and post the elimination journal entries for the period.
    
    Note:
    
    If there is an amount not eliminated due to a currency delta, make a manual journal entry to eliminate the amount.
    

Important:

Do not close the accounting period during the time that the intercompany transaction elimination process is still running. The process may take time depending on the number of transactions to be eliminated. You can check the Status subtab on the **Task: Eliminate Intercompany Transactions** page. When the status says **Complete**, you can click **Back to Period Close** to return to the task page and close the accounting period.

You can find more details about the elimination process you initiated by viewing the following subtabs on the **Task: Eliminate Intercompany Transactions** page:

-   **Notes** - displays system and user notes for all eliminations run for the period.
    
-   **Results** - displays a line for each intercompany elimination process run (number of runs).
    
    Information displayed includes the elimination subsidiary, currency, amount, and a link to elimination journal. You can drill down to view the elimination journal entry created. See [Viewing Intercompany Elimination Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501917.html).
    
-   **Status** - displays the date submitted, submitted by, submission status, any message, and percent complete of each intercompany elimination request.
    
    The **Process Type** column helps you identify whether elimination journal entries are being deleted or created during each intercompany elimination process.
    
    When the submission status is in the initializing state, the **Message** column shows the number of lines processing. This number increases as the initialization detects more lines that require processing.
    
    In the **Submission Status** column, click the **Complete** link to open the Processed Records page. This page provides the results of that elimination request. For information about this page, see [Processed Intercompany Elimination Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4812930211.html).
    
    Note:
    
    The percent complete is an estimate of overall elimination progress. It doesn't represent progress in terms of time.
    

### Related Topics:

-   [Enter Intercompany Transactions for Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501665.html)
-   [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
