---
id: "section_N2043102"
type: "section"
title: "Sales Tax Liability by Tax Agency Report"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > U.S. Tax Reports > Sales Tax Liability by Tax Agency Report"
parent: "section_N2042330"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2043102.html"
anchors: []
sha256: "5283e1c3676c8b734903c00794ecc12c40f8f5a89970348333dd58f023392a28"
---

The Sales Tax Liability by Tax Agency report shows sales tax liabilities that have accrued for the date range selected, and the amounts due as payable at the end of that date range. Amounts in the **Tax Collected** and **Tax Due** columns are determined by the transaction date. The liabilities on this report are grouped by reporting tax authority.

The following columns are included in this report:

-   **Total Sales** - This column reports the amount from invoices, cash sales and credits that included any taxable items sold at the rate for the tax code listed.
    
    It won't match the Sales Summary report because it includes only sales with taxable items.
    
    It will equal the total of the Nontaxable Sales column and the Taxable Sales column on this liability report.
    
-   **Nontaxable Sales** - This column reports the amount of sales that are excluded from sales tax calculations.
    
-   **Taxable Sales** - This column reports the difference between the Total Sales column and the Nontaxable Sales column.
    
    This amount is used as the base for calculation of your sales tax liability.
    
-   **Tax Collected** - This column shows the tax amount that results from multiplying the amount in the Taxable Sales column by the Tax Rate for that transaction.
    
-   **Tax Due** - This column reports the total tax amount due to the tax agency for this tax code. This amount is the total as of the last date selected on this report.
    

Note:

The column values will be retrieved from the **Reporting Tax Authority Name** field on the tax code record.

To see the Sales Tax Liability by Tax Agency report, go to _Reports > Sales Tax US > Sales Tax Liability by Tax Agency_.

A message on the screen indicates that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click **Cancel Report** next to the status bar to stop the report from loading.

You can run this report on a cash basis. The Cash Basis Reporting preference at _Setup > Accounting > Accounting Preferences_, on the General Ledger subtab, applies to all standard reports that support cash basis reporting. If this preference is enabled, the report is on a cash basis rather than an accrual basis. If this preference isn't enabled, you can create a custom cash basis report by enabling Cash Basis on the More Options page of the Financial Report Builder. See [Setting Up Cash Basis Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N744837.html).

### Related Reports

-   [Sales Tax Liability by Tax Item Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2042683.html)
-   [Sales Tax on Sales Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2044611.html)
-   [Sales Tax on Sales Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2044970.html)
-   [Sales Tax Analysis Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2045340.html)
-   [Form 1099-MISC - Miscellaneous Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2045726.html)

### Related Topics

-   [Drilling Down to Records or Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719130.html)
-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
