---
id: "section_N744837"
type: "section"
title: "Setting Up Cash Basis Reporting"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Setting Up Cash Basis Reporting"
parent: "chapter_N736328"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html"
anchors: ["procedure_N744869"]
sha256: "48c44ebe0080d742c7262df0a32c4782cec4442f9604c429156b4795ebc99799"
---

By default, NetSuite reports use an accrual basis to meet generally accepted accounting standards. You can choose cash basis for your report data. Your choice is applied only to reports where the distinction is relevant. You can change this default for all relevant reports or for certain custom reports only.

To change the default globally, use the Cash Basis Reporting preference at _Setup > Accounting > Accounting Preferences_ on the General subtab. Setting this preference makes all standard reports that support cash basis use cash instead of accrual.

Custom reports use the Cash Basis Reporting preference by default, but you can choose cash or accrual for each custom report.

Reports that currently have access to the Cash Basis box are the following reports:

-   Account Detail
    
-   Cost by Customer Detail
    
-   Budget vs. Actual
    
-   Budget Income Statement
    
-   Budget Income Statement Detail
    
-   Income Statement
    
-   Income Statement Detail
    
-   Comparative Income Statement
    
-   Multi-Book Income Statement
    
-   Multi-Book Income Statement Detail
    
-   Financial Layout Description
    
-   GST on Purchases Detail
    
-   GST on Sales Detail
    
-   GST on Purchases Summary
    
-   GST on Sales Summary
    
-   Customer Profitability Detail
    
-   Customer Profitability Summary
    
-   Purchase by Item Detail
    
-   Purchase by Vendor Detail
    
-   Purchase by Item Summary
    
-   Purchase by Vendor Summary
    
-   Sales by Customer Detail
    
-   Sales by Item Detail
    
-   Sales by Promotion Detail
    
-   Sales by Sales Rep Detail
    
-   Sales by Partner Detail
    
-   Sales by Partner Summary
    
-   Sales by Customer Summary
    
-   Sales by Item Summary
    
-   Sales by Promotion Summary
    
-   Sales by Sales Rep
    
-   Summary Sales Tax Liability by Tax Item
    
-   Sales Tax Liability By Tax Agency
    
-   Sales Tax Transaction Detail
    
-   VAT on Purchases Detail
    
-   VAT on Sales Detail
    
-   VAT on Purchases Summary
    
-   VAT on Sales Summary
    

#### To change a custom report between cash basis and accrual basis: {#procedure_N744869}

1.  Go to _Reports > Saved Reports > All Saved Reports_ and click **Edit** next to the custom report you want to edit to open the Report Builder (or Financial Report Builder).
    
2.  Click **More Options**.
    
3.  On the More Options page, use the **Cash Basis** menu to switch between cash and accrual reporting.
    
    -   **Enable** - Select this option if you want to use cash-basis tax data for the report.
        
    -   **Disable** - Select this option if you want to use accrual-basis tax data for the report.
        
    -   **Nexus setting** - Select this option if you want to use nexus settings for tax data. If the nexus has cash-basis tax reporting enabled, the tax data in the report is cash-based. Otherwise, it is accrual-based. To check nexus settings, a user with the Administrator role can go to _Setup > Accounting > Set Up Taxes_, and see if the **Tax Reporting Cash Basis** box is checked for that nexus. See also [Setting Tax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1813668.html).
        
4.  Click **Save**.
    

Note:

If you don't see the Cash Basis option on the More Options page for a report, choosing between cash basis and accrual basis doesn't matter for that report.

### Related Topics

-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Report Builder Interface](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736822.html)
-   [Report Customization Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738489.html)
-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)
-   [Formatting Numbers on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741457.html)
-   [Filtering Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742381.html)
-   [Sorting Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N743154.html)
-   [Setting Additional Options for Custom Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744268.html)
-   [Arranging Data on Summary Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4353206428.html)
-   [Sharing Custom Reports with Other Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745002.html)
-   [Exporting a Saved Report as an Excel Web Query](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745334.html)
-   [Example Report Format Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745576.html)
-   [Saving a Custom Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513909963.html)
-   [Deleting a Custom Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4224521464.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
