---
id: "section_N1405625"
type: "section"
title: "Consolidated Exchange Rate Types"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Consolidated Exchange Rate Types"
parent: "section_N1404834"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html"
anchors: []
sha256: "42820a064d317c9bc85325e41614ab5177f7df88d2e3873f82ad833a77d3ba5f"
---

The Consolidated Exchange Rates table includes three consolidated exchange rate types. Current, Average, and Historical. Each accounting period, accounting book (when Multi-Book Accounting is enabled) and subsidiary pair has its own set of three consolidated exchange rate types. The value of a subsidiary account multiplied by its consolidated exchange rate provides the account value in consolidated financial statements.

The consolidated exchange rate types and the types of accounts that use them are as follows:

-   **Average** - The weighted average of the currency exchange rates for all transactions posted during the period to accounts with a rate type of Average. This rate is used to translate accounts in the income statement and to build retained earnings.
    
-   **Current** - Also referred to as ending rate. This rate is the currency exchange rate that is effective at the end of the reported upon period. This rate is used for most asset and liability accounts in the balance sheet.
    
-   **Historical** - Same as Average rates, except for accounts with a rate type of Historical. This rate is used for equity accounts and owners' investments.
    

You can't select the transactions that are included in the weighted averages NetSuite uses to calculate average and historical rates. High volumes of transactions posted at the end of a period may skew these weighted averages. For an example of how NetSuite calculates the weighted averages, see [Consolidated Exchange Rate Automatic Calculation Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407165.html).

Each account has two consolidated exchange rate type values: a general rate type and a cash flow rate type. The general rate type is used for the income statement, balance sheet, and other general purposes. The cash flow rate type is used for cash flow statements.

Following are the default rate types for accounts:

-   General Rate Type:
    
    -   Current - for all balance sheet accounts other than equity accounts
        
    -   Average - for all income statement accounts
        
    -   Historical - for all equity accounts
        
-   Cash Flow Rate Type: Average - for all accounts except equity
    

Important:

Setting different exchange rate types for different accounts can result in balance sheet discrepancies, particularly discrepancies in consolidated reports.

For information about setting up accounts, see [Creating Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1440518.html).

The difference between values of consolidated exchange rates types results in a balance in the line for Cumulative Translation Adjustment (CTA) on some financial statements. This account line is used in consolidated balance sheet and trial balance reports. The CTA represents the cumulative foreign currency gain or loss resulting from the net investment in the subsidiary. A related line called Effect of Exchange Rate on Cash is used for cash flow statements. For more information, see [Cumulative Translation Adjustment (CTA) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html).

### Related Topics

-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Consolidated Exchange Rates vs. Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405239.html)
-   [Viewing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405950.html)
-   [Editing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406714.html)
-   [Calculating Consolidated Exchange Rates Automatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html)
-   [Consolidated Exchange Rates on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407782.html)
-   [Search for Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1408952.html)
-   [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
