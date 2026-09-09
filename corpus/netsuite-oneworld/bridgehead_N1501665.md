---
id: "bridgehead_N1501665"
type: "bridgehead"
title: "Enter Intercompany Transactions for Elimination"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Elimination Through the Automated Intercompany Management Feature > Enter Intercompany Transactions for Elimination"
parent: "section_N1501565"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501665.html"
anchors: ["bridgehead_156813069405", "bridgehead_156820946693", "bridgehead_N1501765"]
sha256: "f01917b714b8a8a2aa813dc044260a191fb7e55c5a4dc892d18ec2e3f8c4d622"
---

During an accounting period, you can enter the intercompany transactions for elimination by:

-   posting vendor bills and sales invoices
    
-   entering advanced intercompany journal entries (AICJE)
    

Create intercompany vendor bills and sales invoices from paired intercompany purchase orders and sales orders. Intercompany vendor bills and sales invoices are transactions for intercompany entities. Intercompany entities use intercompany A/R and intercompany A/P accounts as their default A/R and A/P accounts. The income, expense, A/R, and A/P lines on the intercompany vendor bills and sales invoices are automatically marked for elimination. There is no Elimination flag on the these transactions lines.

The following account types should be used only for elimination purposes:

-   Other Current Asset (Non-Inventory)
    
-   Other Asset
    
-   Defer Expense
    
-   Defer Revenue
    
-   Other Current Liability
    
-   Long Term Liability
    

Warning:

Note the following if you use this preference: Do not update COGS and Asset accounts on existing transactions when accounts are changed. To avoid mismatch in the consolidated financials, ensure you change the COGS accounts on item records when all the transactions with those items are eliminated.

## Journal Entries for Intercompany Transaction Activity {#bridgehead_156813069405}

Use advanced intercompany journal entries (AICJE) to enter intercompany transactions and flag journal lines to be eliminated. In an AICJE, adding an intercompany account to a journal line automatically sets the Eliminate flag for the line to Yes. This setting defaults from the value set for the Eliminate Intercompany Transactions box on the intercompany account record. Advanced intercompany journal entries force you to have balanced elimination lines.

Warning:

Regular journal entries used for intercompany transaction activity do not automatically balance lines to be eliminated. If you do not balance the lines, NetSuite posts the journal lines without validating the accounts used and the elimination flags.

Advanced intercompany journal entries require balanced debits and credits across subsidiaries for journal line pairs that use balance sheet accounts (A/R, A/P). These journal entries also require balanced debits and credits for lines using income statement accounts (Income, Expense, Cost of Goods Sold (COGS)). NetSuite validates the journal lines when you save an AICJE. It also displays an error if the debit and credits do not balance for the line pairs.

Warning:

In book specific journal entries with accounts receivable, accounts payable or both, NetSuite doesn't validate the journal lines. The reason for not validating is that you can't add accounts receivable or accounts payable lines with named entities because the name field is disabled. Therefore, these journal lines can't be eliminated.

## Customers With Multiple Currencies {#bridgehead_156820946693}

If you have customers who use multiple currencies, create the AICJE in the base currency of the sales subsidiary (the vendor for the transaction). For more information about account types and intercompany transactions, see [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html) and [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html).

You can't check the Eliminate Intercompany Transactions box on AICJE lines posting to non intercompany accounts or to equity type accounts.

## Classify Intercompany Transactions {#bridgehead_N1501765}

Some elimination type accounts such as Other Current Asset and Other Current Liability are eliminated based on cumulative amounts. Therefore, these accounts can't be isolated into distinct class, department, and location based on source transactions.

You can specify a class, department, and location on the Intercompany Eliminations page when you run intercompany eliminations. The class, department, and location you select populates the corresponding fields on the elimination journal entries.

Important:

If you use the **Make Locations Mandatory** accounting preference, Location is a required field on the Intercompany Eliminations page. The Location list defaults to the Default Elimination Subsidiary Location option, but you can select any location that has been associated with elimination subsidiaries.

If you use the **Multi-Location Inventory** feature, Location is a required field on the Intercompany Eliminations page.

The location you select on this page overrides the location entered on the source transaction, and becomes the location specified on the elimination journal entry.

If you do not use the **Make Locations Mandatory** accounting preference or the **Multi-Location Inventory** feature, the Location list defaults to the blank option. You can, however, select the Default Elimination Subsidiary Location option, or any location that has been associated with elimination subsidiaries.

### Related Topics:

-   [Running Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501792.html)
-   [Viewing Intercompany Elimination Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1501917.html)
-   [Processed Intercompany Elimination Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4812930211.html)
-   [Elimination Through the Automated Intercompany Management Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1501565.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
