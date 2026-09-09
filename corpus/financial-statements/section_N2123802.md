---
id: "section_N2123802"
type: "section"
title: "Subsidiary-Specific Financial Layouts"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > OneWorld Financial Statements > Subsidiary-Specific Financial Layouts"
parent: "chapter_N2119691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123802.html"
anchors: ["procedure_N2123847"]
sha256: "408a5ac927b7646695d1bb29758b05bc8fbb104943ac9dac8c32935191b47587"
---

When you use NetSuite OneWorld, NetSuite provides specialized country-specific layouts for each subsidiary's financial statements. When you customize a financial statement, the most recently used subsidiary context for that report is selected for your custom report. The selected subsidiary context and its associated layout display on the Edit Layout page in the Financial Report Builder.

For example, run the Balance Sheet report with the Australian subsidiary selected in the Subsidiary Context list and then click Customize. The Australian subsidiary is shown as the subsidiary context and the Australian Balance Sheet layout is used.

![Screenshot of a portion of the Edit Layout page of the Financial Report Builder with the Subsidiary Context field outlined in red](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBCustSubCont.png)

To customize a balance sheet for a different subsidiary, first rerun the report and select a new subsidiary context. When you select a new layout from the Layout list on the Financial Report Builder Edit Layout page, the subsidiary context does not change. Instead, the new layout is assigned to the currently displayed subsidiary.

#### To customize a OneWorld financial statement using the correct subsidiary context and layout: {#procedure_N2123847}

1.  Run the selected financial statement.
    
2.  In the **Subsidiary Context** list in footer of the report, select a subsidiary context.
    
3.  Click the **Refresh** button.
    
4.  Click the **Customize** button to access the Financial Report Builder.
    

The preceding steps are the recommended method for customizing a OneWorld financial statement. If you access the Financial Report Builder by going to Reports > New Financial Report or Reports > Financial > `Report_Name` > Customize, the most recently selected subsidiary context is used. This context may not be the subsidiary context you want.

If the subsidiary context displayed in the Financial Report Builder for your custom statement isn't correct, exit the Financial Report Builder and follow the above steps.

For more information about financial statement layouts, see [Financial Statement Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2110511.html).

### Related Topics

-   [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html)
-   [Subsidiary Context for a Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123544.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)
-   [Cumulative Translation Adjustment (CTA) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html)
-   [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html)
-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statements Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
