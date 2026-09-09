---
id: "section_N1486928"
type: "section"
title: "Intercompany Accounts"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Intercompany Accounts"
parent: "section_N1486610"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html"
anchors: ["bridgehead_156811728030", "bridgehead_156811733323", "bridgehead_156811737888"]
sha256: "27c993eceaa2949b63e5fd24862fc1cbb8e0340e48f3e57a22788d335d69fd7d"
---

Intercompany accounts are general ledger accounts used to record transactions, such as intercompany payments, loans, and funds transfers between subsidiaries. These accounts track the intercompany amounts to be eliminated. When you run the intercompany elimination period end close task, amounts posted to intercompany accounts eligible for elimination are eliminated for consolidated financial statements. Posting occurs during the period close process.

An intercompany account is an account that has the **Eliminate Intercompany Transactions** box checked. For accounts that can't be used for intercompany transactions, the field is dimmed. You can post both intercompany transactions and non-intercompany transactions to most intercompany accounts. Intercompany Accounts Receivable and intercompany Accounts Payable accounts, however, can be used only for recording amounts that are candidates for eliminations. **NetSuite requires an intercompany customer or intercompany vendor for intercompany A/R and A/P accounts.**

## Double-Entry Bookkeeping {#bridgehead_156811728030}

NetSuite enforces double-entry bookkeeping, therefore, journal entries post changes to accounts using offsetting debits and credits. Each posting transaction in NetSuite posts to at least two accounts. Each journal entry includes at least one debit amount and at least one credit amount. For information about journal entries, see [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html).

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In 2013.1, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This account replaced the Intercompany Payable/Receivable XXX account for new implementations. In 2014.1, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that are not currency locked. NetSuite uses these clearing accounts for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

## Account Groups {#bridgehead_156811733323}

You can create an intercompany account for the following groups of accounts:

-   [Accounts Receivable and Accounts Payable](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1487235.html)
    
-   [Equity, Income Statement, and Inventory Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1488569.html)
    
-   [Balance Sheet Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1489083.html)
    

You can't create intercompany accounts for the following system-generated accounts:

-   Unrealized Matching Gain/Loss
    
-   Unrealized Gain/Loss
    
-   Realized Gain/Loss
    
-   Rounding Gain/Loss
    
-   Exchange Rate Variance
    
-   Cumulative Translation Adjustment-Elimination
    
-   Cumulative Translation Adjustment
    
-   Undeposited Funds
    
-   Intercompany Clearing XXX (deferred Cost of Goods Sold (COGS))
    

For more information about features and system-generated accounts, see [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html).

## Account Types {#bridgehead_156811737888}

You can create more than one intercompany account for each account type. For a list of account types and accounts that you can't use for elimination, see [Other Account Types and Exceptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1489533.html).

Best practice is to create new intercompany A/R and intercompany A/P accounts for intercompany transactions. Existing A/R and A/P accounts have accumulated balances from non-intercompany transactions that can't be combined with future intercompany transactions to be eliminated.

To use existing item income and expense accounts for new intercompany transactions, check the **Eliminate Intercompany Transactions** box. You must check this box for all income and expense accounts associated with items used in intercompany transactions.

Note:

If you modify an existing account to be an intercompany account, existing transactions posted to the account are not automatically marked for elimination. You must edit any historical transaction to be included for elimination. When you save the transaction with an intercompany entity, NetSuite marks transaction lines associated with the intercompany account for elimination.

### Related Topics:

-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)
-   [Creating Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html)
-   [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html)
-   [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html)
-   [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
