---
id: "section_N2124272"
type: "section"
title: "Cumulative Translation Adjustment (CTA) Overview"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > OneWorld Financial Statements > Cumulative Translation Adjustment (CTA) Overview"
parent: "chapter_N2119691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html"
anchors: ["bridgehead_N2124311", "bridgehead_N2124380", "bridgehead_N2124865"]
sha256: "53d547280a9dff76a187cb9928ef3a6870cb6c3fd3f12eafc6f3e6289a4f4838"
---

Cumulative Translation Adjustment (CTA) is a special type of account that is required for consolidated balance sheets in NetSuite OneWorld accounts with multi-currency enabled.

The CTA is used on the consolidated balance sheet to make it balance. This account is necessary because consolidated exchange rate types of the accounts on the balance sheet may differ. The result is different consolidated exchange rates, which cause an imbalance. Three types of consolidated exchange rates apply to different account types during consolidation:

-   **Current rate** - Applies to most asset and liability accounts
    
-   **Average rate** - Applies to all income statement accounts, such as income and expense.
    
-   **Historical rate** - Applies to accounts in the capital section of the balance sheet including equity and dividends.
    

For more information about the consolidated exchange rate types and how they are calculated, see [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html).

NetSuite dynamically calculates CTA for each account and then displays the total in the CTA account line. You can customize balance sheet reports to include a column titled **Translation Adjustment**. This column shows the amount resulting from the difference between the consolidated exchange rate that is used on each account and the current exchange rate.

The CTA is used wherever consolidation across accounts with different consolidated rate types occurs, such as the consolidated trial balance.

Important:

The consolidated cash flow statement includes a row called **Effect of Exchange Rate on Cash**. This row adjusts for the effects of consolidated exchange rate differences in cash flow statement accounts. These adjustments ensure that the cash flow statement's **Cash at End of Period** is consistent with the balance sheet's bank or cash equivalent. The Effect of Exchange Rate on Cash row includes amounts that may not be posted to the CTA account. See [Cash Flow Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103273.html).

## CTA Account Record {#bridgehead_N2124311}

When you use the Multiple Currencies feature in a NetSuite OneWorld account, the CTA account is included as an account in the chart of accounts. You can't delete the account, and the following fields on the account record are not editable:

-   General Rate Type
    
-   Cash Flow Rate Type
    
-   Subaccount of
    
-   Restrict To Department
    
-   Restrict to Class
    
-   Restrict to Location
    
-   Subsidiary
    

The CTA account is used solely for balancing consolidated balance sheets. You can't select the CTA account on items, tax codes, nexus records, or most transactions. The CTA account isn't available when setting up credit card processing. The CTA account is, however, available for selection on journal entries. The amount you see in consolidated reports for CTA is calculated dynamically, not posted to the account.

The CTA account is separate from the Cumulative Translation Adjustment-Elimination (CTA-E) that NetSuite adds to your account when you enable the Automated Intercompany Management feature. For information about the CTA-E account, see [Cumulative Translation Adjustment-Elimination (CTA-E)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498539.html).

## Example Use of CTA in Balance Sheet {#bridgehead_N2124380}

In the sample hierarchy below, you are rolling up the balances from Wolfe UK into the Wolfe US consolidated parent. The appropriate consolidated exchange rate for each account is used to roll up the balances into U.S. dollars.

![Diagram of sample subsidiary hierarchy to show how balances roll up to the consolidated parent using the appropriate consolidated exchange rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/UnderstandingSubsidiariesContextForReports_2.png)

The Wolfe UK consolidated balance sheet appears as follows:

|  | Amount (GBP) | Consolidated Rate Type | Consolidated Exchange Rate | Calculation | Consolidated Amount (USD) |
| --- | --- | --- | --- | --- | --- |
| Assets | £250 | Current | 2.0 | 250 × 2 | $500 |
| Liabilities | (£100) | Current | 2.0 | 100 × 2 | ($200) |
| Retained Earnings | (£100) | Average | 2.5 | 100 × 2.5 | ($250) |
| Equity | (£50) | Historical | 3.0 | 50 × 3 | ($150) |
| Balance in GBP | £0 |  |  | CTA | ($100) |

The balance sheet always balances in the local currency, as shown in the last line of the previous table. However, because the consolidated rates for equity and retained earnings are different than those for assets and liabilities, the consolidated balance sheet may not balance. The CTA equals the amount that is required to balance the consolidated balance sheet. In this example, the CTA is **($100)**.

## Auditing CTA Calculation {#bridgehead_N2124865}

To help you audit the calculation of CTA, NetSuite includes the CTA Balance Audit report. To open this report, click the amount for the Cumulative Translation Adjustment in the Balance Sheet, Comparative Balance Sheet, or Trial Balance. You can also go to _Reports > Financial > CTA Balance Audit_ to open the report. For information about using the report, see [CTA Balance Audit Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4688047790.html).

### Related Topics

-   [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html)
-   [Subsidiary Context for a Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123544.html)
-   [Subsidiary-Specific Financial Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123802.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)
-   [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statements Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html)
-   [Available Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092953.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
