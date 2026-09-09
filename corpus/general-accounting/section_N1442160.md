---
id: "section_N1442160"
type: "section"
title: "Setting Up Historical Balances in OneWorld"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Chart of Accounts Management > Setting Up Historical Balances in OneWorld"
parent: "chapter_N1439850"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442160.html"
anchors: ["procedure_N1442223"]
sha256: "ea3ba326832e31cce1763cbbda6577bce4213deecb305356c85701e72e8f11db"
---

it's recommended that you don't load a complete transaction history to set up or upgrade to NetSuite OneWorld. Instead, to bring in the general ledger, best practice is to journal in the balances of all balance sheet accounts as of a period end.

Exchange rate issues can cause complications for journal entries representing child subsidiary equity accounts, if these accounts' amounts are translated into the parent subsidiary's currency for consolidated financials. You may require more than one historical rate to translate different equity accounts such as capital stock and retained earnings for the consolidated balance sheet.

The Consolidated Exchange Rates table stores one historical rate per time period. Extra steps are necessary to use a different historical rate for a particular equity account such as capital stock. These steps include the following:

-   Setting up a historical rate used for most equity accounts in the most recently completed period
    
-   Setting up an additional historical rate used for the capital stock account in a previous period
    
-   Creating journal entries to ensure that the earlier rate is used to translate capital stock accounts for the consolidated balance sheet
    

The following example illustrates this process. In this example:

-   The intent is to journal in balances to result in an accurate balance sheet as of 12/31/13, for a U.S. child subsidiary of a U.K. parent subsidiary.
    
-   An Opening Balance equity account starts with a zero balance.
    
-   The balance in the Retained Earnings equity account is 1,500 GBP and needs to be translated at a rate of .5 USD/1 GBP.
    
-   The balance in the Capital Stock equity account is 1,000 GBP and needs to be translated at a rate of .6 USD/1 GBP.
    

#### To ensure that capital stock amounts are translated at the correct rate: {#procedure_N1442223}

1.  Ensure the **Opening Balance** equity account has a **General Rate Type** value of **Current**.
    
    Because the default general rate type for equity accounts is **Historical**, you may be required to edit this value. You can edit an account record at _Lists > Accounting > Accounts_.
    
2.  In the example above, ensure that the November 2013 period has a status of open.
    
    If this period has been closed, you need to reopen it. See [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html) . Opening this period causes all later periods to be reopened as necessary.
    
3.  In the Consolidated Exchange Rates table, set the following historical exchange rates from the U.S. subsidiary to the U.K. subsidiary:
    
    -   For the period of November 2013, set a historical rate of .6. This rate is used for capital stock.
        
    -   For the period of December 2013, set a historical rate of .5. This rate is used for retained earnings and other equity accounts.
        
    
    For instructions for adding or editing these rates, see [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html).
    
4.  Post the following journal entries:
    
    -   For December 2013:
        
        DEBIT Capital Stock 1,000 GBP
        
        CREDIT Opening Balance account 1,000 GBP
        
    -   For November 2013:
        
        DEBIT Opening Balance account 1,000 GBP
        
        CREDIT Capital Stock 1,000 GBP
        
5.  Close November 2013, December 2013, and any other periods as necessary. See [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html).
    

After these steps are completed, the balance in the Capital Stock account is translated at the .6 rate, for any Balance Sheet as of December 2013 or a later period.

### Related Topics:

-   [Feature-Specific, System-Generated Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4078513386.html)
-   [Chart of Account Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440268.html)
-   [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html)
-   [Account Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3947502870.html)
-   [Entering Opening Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1441761.html)
-   [Viewing the Chart of Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442506.html)
-   [Making Changes to Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1442743.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
