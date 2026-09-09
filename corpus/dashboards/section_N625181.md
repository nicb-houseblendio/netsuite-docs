---
id: "section_N625181"
type: "section"
title: "Financial Ratios Scorecard Formulas"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > KPI Scorecards > Financial Ratios Scorecard > Financial Ratios Scorecard Formulas"
parent: "section_N624824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N625181.html"
anchors: []
sha256: "4c694af1dd4edcb1bda559c1345ca7673378273f44d3e7c177a8f7ce7708d8ef"
---

The following table lists the formulas used to calculate data for the prebuilt Financial Ratios scorecard. This scorecard is available if you have permission to see the Trial Balance report. Formula components are standard NetSuite KPI IDs.

| **Scorecard Ratio** | **Formula** |
| --- | --- |
| Current Ratio | ({BANKBAL}+{RECEIVABLES}+{OTHERCURRENTASSET})/({PAYABLES}+{CREDITCARDBAL}+{OTHERCURRENTLIAB}) |
| Receivables | {SALES}/{RECEIVABLES} |
| Days Sales Outstanding | {DAYS}/({SALES}/{RECEIVABLES}) |
| Inventory Turnover | {COGS}/{INVENTORY} |
| Days Inventory On Hand | {DAYS}/({COGS}/{INVENTORY}) |
| Asset Turnover | 
{SALES}/({BANKBAL}+{RECEIVABLES}+{OTHERCURRENTASSET}+

{FIXEDASSET}+{OTHERASSET})



 |
| Profit Margin on Sales | {PROFIT}/{INCOME} |
| Return on Assets | 

{PROFIT}/({BANKBAL}+{RECEIVABLES}+

{OTHERCURRENTASSET}+{FIXEDASSET}+{OTHERASSET})



 |
| Return on Equity | {PROFIT}/{EQUITY} |
| Debt to Total Assets | 

({PAYABLES}+{CREDITCARDBAL}+{OTHERCURRENTLIAB}+

{LONGTERMLIAB})/({BANKBAL}+{RECEIVABLES}+

{OTHERCURRENTASSET}+{FIXEDASSET}+{OTHERASSET})



 |
| Debt to Equity | 

({PAYABLES}+{CREDITCARDBAL}+{OTHERCURRENTLIAB}+

{LONGTERMLIAB})/{EQUITY}



 |

-   For more information about this scorecard, see [Financial Ratios Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624824.html).
    
-   For information about the underlying report, see [Trial Balance Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1520986.html).
    
-   For a list of standard KPI IDs, see [KPI IDs Available for Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613450.html).
    
-   For a list of standard KPIs and descriptions, see [Standard Key Performance Indicators Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N601098.html).
    
-   For information about adding formulas to KPI scorecards, see [Defining KPI Scorecard Formulas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N613116.html).
    

### Related Topics

-   [Financial Ratios Scorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N624824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
