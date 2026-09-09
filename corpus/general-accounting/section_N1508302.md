---
id: "section_N1508302"
type: "section"
title: "Budget Exchange Rates"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Subsidiary Budgets in OneWorld > Budget Exchange Rates"
parent: "section_N1506361"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html"
anchors: []
sha256: "c1285a48d285ff89ac7be72274384393675a179f2bb669672c70ffbffa88bd3c"
---

Budget exchange rates ensure that currency amounts for budgets translate properly from child to parent subsidiaries for consolidated budget reports. The Budget Exchange Rates list is available at _Lists > Accounting > Budget Exchange Rates_. This table is available only when the Multiple Currencies and Multiple Budgets features are enabled. Your user role must have the Currency permission with Full permission level to work with budget exchange rates.

The Budget Exchange Rates list is similar to the Consolidated Exchange Rates list, and NetSuite uses consolidated exchange rates for the initial budget exchange rates. The budget exchange rates enable you to use different rates from the consolidated rates for budget. On budget-related reports and financial statements, you can use both consolidated exchange rates and budget exchange rates. For information, see [Budget-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158801165026.html) and [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html).

For instructions for editing the budget exchange rates, see [Editing Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1508439.html).

The Budget Exchange Rates page includes the following filters, all of which include an - All - option:

-   **Period** - Accounting period.
    
-   **Accounting Book** - Included only when the Multi-Book Accounting feature is enabled.
    
-   **From Subsidiary** - Child subsidiaries.
    
-   **To Subsidiary** - The list of options includes all subsidiaries, but only parent subsidiaries return results.
    

You can also search for budget exchange rates. For information, see [Search for Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1508542.html).

The Budget Exchange Rates list stores three rate type values for each period, accounting book, and subsidiary pair. You can see only those subsidiaries and accounting books to which you have access. The rate types correspond with the consolidated exchange rate types. For an explanation of these rate types, see [Consolidated Exchange Rate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1405625.html).

Rates in this table are either direct or indirect (derived).

-   **Direct rates** are set between a child and parent subsidiary. You can edit these rates.
    
-   **Indirect rates** are calculated between subsidiaries more than one hierarchical level removed from each other, such as between a parent and grandchild. Indirect rates are always calculated by the system. You can't edit them. When the direct rates change, NetSuite updates the indirect rates.
    

### Related Topics

-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Subsidiary Budgeting Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506662.html)
-   [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html)
-   [Setting Up a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507295.html)
-   [Guidelines for Copying a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html)
-   [CSV Import for Subsidiary Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508163.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
