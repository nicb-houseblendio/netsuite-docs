---
id: "section_N1489768"
type: "section"
title: "Creating Intercompany Accounts"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Creating Intercompany Accounts"
parent: "section_N1486610"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html"
anchors: ["procedure_N1489799", "bridgehead_159248476836"]
sha256: "839191a28471e19ddc559fb7961a1c7ce647351dd517ac2a1e5ee1166d638529"
---

You can create intercompany accounts by adding a new account or by modifying an existing account, when permitted. Before you create intercompany accounts, ensure that you understand the different types of accounts that can be used to record intercompany transactions. For more information, see [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html).

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

At a minimum, to properly account for and eliminate intercompany transactions, you need the following accounts:

-   Expense Account
    
-   Income Account
    
-   Receivables Account
    
-   Payables Account
    
-   Deferred Revenue Account
    

#### To add a new intercompany account: {#procedure_N1489799}

1.  Go to _Setup > Accounting > Chart of Accounts > New_.
    
2.  Select the type of account to create based on the account purpose.
    
    Note:
    
    NetSuite requires an intercompany customer or intercompany vendor for intercompany A/R and A/P accounts.
    
    The values for **General Rate Type** and **Cash Flow Rate Type** default to the rate types of the type of account selected.
    
3.  Enter a name for the account.
    
4.  Check the **Eliminate Intercompany Transaction** box.
    
5.  Complete other fields, as needed.
    
6.  For **Subsidiaries**, select the parent or top level subsidiary and then check **Include All Children**.
    
7.  Click **Save**.
    

## Making an Existing Intercompany Account an Elimination Account {#bridgehead_159248476836}

Use the following procedure to change an intercompany account into an elimination account.

#### To make an existing intercompany account an intercompany elimination account:

1.  Go to _Setup > Accounting > Manage G/L > Chart of Accounts_.
    
2.  Click **Edit** next to the account you want to modify.
    
3.  Check the **Eliminate Intercompany Transactions** box, and then click **Save**.
    

### Related Topics:

-   [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html)
-   [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html)
-   [Intercompany Inventory Items Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html)
-   [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
