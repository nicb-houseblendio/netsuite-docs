---
id: "section_N1478200"
type: "section"
title: "Creating Intercompany Adjustments for Time and Expenses"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Journal Entries in OneWorld > Enabling Intercompany Time and Expenses > Creating Intercompany Adjustments for Time and Expenses"
parent: "section_N1476983"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478200.html"
anchors: ["procedure_N1478270"]
sha256: "2e45fe2ef4bce828761d6ef0dc6dfb5bf5dfa1cadf6e289098a8f65f1a08649d"
---

If the Intercompany Time and Expense feature has been enabled, and the Intercompany Expenses preference has been set to Allow and Adjust, you can create automated intercompany expense adjustments. If you also use Job Costing, you can create intercompany adjustments to account for posted project time transactions. See [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In a later release, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. Still later, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that aren't currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

Users with the Intercompany Adjustments permission and access to all subsidiaries, can generate all required adjustments for a selected posting period. You should complete this task as part of the period close process, but it can be done at any time. To access this task from the Period Close Checklist, users need the Manage Accounting Periods permission. To complete this task for a locked period, users need the Override Period Restrictions permission.

Note:

To have the required permission and access, users must be administrators or have a custom role. The standard CFO role has the Intercompany Adjustments permission but needs to be customized to be granted access to all subsidiaries. See [Control Employee Access to Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278097.html).

#### To create intercompany adjustments: {#procedure_N1478270}

1.  Go to _Transactions > Financial > Create Intercompany Adjustments_.
    
    (You can reach this page either from the Period Close Checklist page or from its own task link.)
    
    You can't access this page unless you have the **Intercompany Adjustments** permission **and** access to all active subsidiaries. The **Intercompany Time and Expense** feature must be enabled and the **Intercompany Expenses** preference must be set to **Allow and Auto Adjust**.
    
    If you also use Job Costing, the **Intercompany Time** preference must be set to **Allow**.
    
2.  In the **Posting Period** field, select a posting period.
    
    (If you accessed this page from the period close checklist, the posting period is preselected.)
    
    The journal entry date is set to the last day of the selected period.
    
    A list of adjustments displays expense and posted time amounts to be transferred from the subsidiary of the employee (Originating Subsidiary) to the subsidiary of the customer or project (Related Subsidiary). One adjustment is listed for each subsidiary pair.
    
    Each adjustment line displays the base currency of the originating subsidiary. It also displays the amount required to adjust for expenses entered by employees in the originating subsidiary that must be charged to the related subsidiary.
    
    This currency may not reflect the currency used on the expense report, which is used primarily for receipt matching. Only approved expense transactions are used to calculate the amount of each adjustment.
    
3.  To view a detailed list of expense and time transactions covered by an adjustment, click an adjustment line's **Amount** field. The list displays in a separate Required Subsidiary Adjustments window.
    
    Note:
    
    Only approved expense transactions and posted time transactions are included in this list. Currency values may not match the currency used in the transaction.
    
    \* To view an expense report record, click its **Date** link.
    
    \* To edit an expense report record, click its **Edit** link.
    
    \* To customize the view, click the **Customize View** button. For more information, see [Customizing Sublist Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N496633.html).
    
    \* To view a job costing journal entry, click its **View** link.
    
4.  To automatically generate journal entries that implement the listed adjustments, click **Submit**.
    
    The intercompany clearing account is created if one doesn't exist. For more information, see [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html).
    
    If generation of journal entries takes an extended period of time, a status page displays.
    
    After the adjusting journal entries are generated, the Processed Adjustments page displays.
    
5.  After journal entries have been created, you can see journal entry detail for each adjustment by clicking a **Journal** field on the Processed Adjustments page.
    
    -   Journal date is the last day of the selected posting period.
        
    -   The intercompany clearing account is used to balance debits and credits in each subsidiary.
        
    -   All journal amounts are in the base currency of the originating subsidiary, for accounts in both the originating subsidiary and the related subsidiary. General ledger impact to each subsidiary is in its own base currency.
        
        Each journal entry includes an exchange rate used to translate general ledger impact from the originating subsidiary's base currency to the related subsidiary's base currency. This exchange rate corresponds to the date the transaction occurred.
        
    -   To review the general ledger impact of an adjustment, click the link in the header of the adjustment record.
        
        Amounts for originating subsidiary accounts remain in that base currency. Amounts for the related subsidiary are converted using the exchange rate on the adjustment record.
        

To review previously processed adjustments, you can:

-   Go to _Transactions > Financial > Create Intercompany Adjustments_ > Status. Click a **COMPLETE** link in the **Status** column to view the list of adjustments processed as part of each job.
    
-   Do a transaction search, specifying a value of **Yes** for the newly added search field **Is Intercompany Adjustment**. For an example, see [Example Intercompany Adjustment Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478633.html).
    

Important:

For the system to generate an adjustment that includes a class, department, or location, the specified classification must be available to the selected customer's subsidiary. You can also enable the option **Allow Empty Classifications on Journals** at _Setup > Accounting > Accounting Preferences_ > General subtab.

### Related Topics:

-   [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html)
-   [Intercompany Clearing Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1477786.html)
-   [Example Intercompany Adjustment Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1478633.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
