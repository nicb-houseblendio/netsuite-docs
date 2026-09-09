---
id: "section_N1507638"
type: "section"
title: "Guidelines for Copying a Subsidiary Budget"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Subsidiary Budgets in OneWorld > Guidelines for Copying a Subsidiary Budget"
parent: "section_N1506361"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507638.html"
anchors: []
sha256: "e1108852b7f7e5e1483d1b0179a3c3d279ca7092006b682d2ca426d62460fff1"
---

In NetSuite OneWorld, you can copy a subsidiary's actual amounts or a budget to use as the basis for different versions of the same subsidiary's budget.

To create or copy budgets for an elimination subsidiary, set the **Enable Budget with Elimination Subsidiaries** accounting preference.

For the specific steps to copy a budget, see [Copying a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505228.html).

The Budget Category you select on the Copy Budgets page as the target (To) affects the amounts in the budget copy as follows:

| From - source budget category type | To - target budget budget category type | Impact |
| --- | --- | --- |
| Local | Local | 1-to-1, no change from local. |
| Local | Global | Use Budget Exchange Rates table to convert local currency amounts to global currency amounts. |
| Global | Local | Use Budget Exchange Rates table to convert global currency amounts to local currency amounts. |
| Global | Global | 1-to-1, no change from global. |

When copying actual amounts into a budget, the Budget Category you select as the target (To) affects the amounts in the budget copy as follows:

| From - source budget category type | To - target budget category type | Impact |
| --- | --- | --- |
| Local | Local | 1-to-1, no change from local. |
| Local | Global | Use Consolidated Exchange Rates table to convert local currency amounts to global currency amounts. |

A budget with a global budget category type has source amounts in the root parent's base currency. When you copy that global budget as the basis for a local budget, NetSuite converts the amounts into the subsidiary's base currency. The exchange rates for the conversion are those in the Budget Exchange Rates table.

For example, you copy a budget with a global budget category type in U.S. dollars (USD) as the basis for a local budget in Canadian dollars (CAD). NetSuite converts the budget amounts from USD to CAD when copying the budget. The conversion uses the **inverse** of the CAD to USD exchange rate from the Budget Exchange Rate table. The inverse rate is used because the Budget Exchanges Rates table stores only bottom-up exchange rates (CAD to USD), not top-down (USD to CAD).

### Related Topics

-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Subsidiary Budgeting Scenario](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506662.html)
-   [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html)
-   [Setting Up a Subsidiary Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1507295.html)
-   [CSV Import for Subsidiary Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508163.html)
-   [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
