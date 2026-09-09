---
id: "section_N1405950"
type: "section"
title: "Viewing Consolidated Exchange Rates"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Consolidated Exchange Rates > Viewing Consolidated Exchange Rates"
parent: "section_N1404834"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405950.html"
anchors: []
sha256: "34a6b82ac08e974c7602c101a8e62813603b0050560f1f66f28722e4ebf66b65"
---

You can access the Consolidated Exchange Rates list at _Lists > Accounting > Consolidated Exchange Rates_. Your user role must have the Currency permission with Full permission level to work with consolidated exchange rates.

You can also access this list from the Period Close Checklist. See [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).

Filters for the list include accounting Period, Accounting Book (when Multi-Book Accounting is enabled), From Subsidiary, and To Subsidiary. When you access this page from the Period Close Checklist, NetSuite automatically filters the list to show only the checklist period.

The Consolidated Exchange Rates list stores three consolidated rate type values for each period, accounting book, and subsidiary pair. You can see only those subsidiaries and accounting books to which you have access. List columns include the accounting period, whether the period is closed, From (child) subsidiary, To (parent) subsidiary, and consolidated exchange rates for each. Rate values are displayed up to seven decimal places. In the System Notes column, click the History link to open a page with an audit trail of changes for each line.

Rates in this table are either direct or indirect (derived).

-   **Direct rates** are set between a child and parent subsidiary. You can edit these rates or auto calculate them.
    
-   **Indirect rates** are calculated between subsidiaries more than one hierarchical level removed from each other, such as between a parent and grandchild. Indirect rates are always calculated by the system. You can't edit them. When the direct rates change, NetSuite updates the indirect rates.
    
    To derive consolidated exchange rates between grandchild and parent in a parent-child-grandchild hierarchy, get the rates from child to parent and from grandchild to child. Those rates multiplied by each other equal the rate from grandchild to parent.
    

To change the filters or results column in this table, click **Customize View**. For more information, see [Customizing List Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N496170.html). When you access this page from the Period Close Checklist, the Customize View function isn't available.

Click **Calculate** to update multiple rates for a single period. When you click this button, all rates for the subsidiaries to which you have access are updated.

The Calculate button is always available when you go to this page from the Period Close Checklist because only a single period is displayed. When multiple periods are shown, this button is dimmed.

To print the table of consolidated exchange rates, click the print icon ![Print icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PrintIcon.png).

To export consolidated exchange rates to a file, click one of the export icons:

-   ![CSV file icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/ExportCSV.png) Export - CSV
    
-   ![Excel file icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/ExportExcel.png) Export - Microsoft Excel
    
-   ![PDF file icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/ExportPDF.png) Export - PDF
    

### Related Topics

-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
-   [Consolidated Exchange Rates vs. Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405239.html)
-   [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html)
-   [Editing Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406714.html)
-   [Calculating Consolidated Exchange Rates Automatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1406908.html)
-   [Consolidated Exchange Rates on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1407782.html)
-   [Search for Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1408952.html)
-   [Consolidated Exchange Rate Types for Transaction Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1409190.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
