---
id: "section_N278654"
type: "section"
title: "Consolidated Reporting in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Consolidated Reporting in OneWorld"
parent: "preface_1540397395"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278654.html"
anchors: []
sha256: "6b5ec9b48db9ac038ec125ac4a4f5e4a99162d1f4270e2f968828b250597a287"
---

With NetSuite OneWorld, you can view data consolidated from multiple subsidiaries on many reports.

Important:

Some reports do not support consolidation. These reports return results for only one subsidiary at a time. Before you can run one of the consolidated reports, you must set your user preferences to restrict your view to a single subsidiary. Go to _Home > Set Preferences_ and then set the preference on the Restrict View subtab.

If a report can show consolidated information, the Subsidiary Context field in the footer of the report includes options appended with (Consolidated). For example, the report titled HEADQUARTERS(Consolidated). When you select a consolidated subsidiary on a report, the data displayed is for the selected subsidiary and its child subsidiaries including elimination subsidiaries. For example, if you choose Subsidiary Context HEADQUARTERS (Consolidated), the report displays consolidated data for the UK and its child subsidiaries, Germany and Italy.

When you select a subsidiary that is not consolidated, the data displayed is for that selected subsidiary. For example, selecting Subsidiary Context UK displays only the UK subsidiary data. For more description and examples of the Subsidiary Context filter, see [Subsidiary Context for Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278946.html).

Note:

If you use Multi-Book Accounting, you can run consolidated reporting on any accounting book enabled for consolidation.

When the data displayed is for a single subsidiary, NetSuite uses the base currency of that subsidiary for amounts. When the data displayed is consolidated for multiple related subsidiaries, NetSuite uses the base currency of the parent subsidiary for amounts. Consolidated reports use the Consolidated Exchange Rates table to translate child subsidiaries' amounts to roll up into consolidated parent subsidiary amounts. See [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html).

Reports that include budget and actual amounts, such as some financial statements, use a separate Budget Exchange Rates table for translation of budget amounts. See [Subsidiary-Specific Budget Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2125541.html).

Financial statements have other specialized capabilities in OneWorld, including subsidiary-specific layouts. See [OneWorld Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2119691.html).

Consolidated balance sheet and cash flow statement reports use a special account called Cumulative Translation Adjustment (CTA). The CTA account achieves balance when there is more than one currency. This account is necessary because the rate types of accounts may differ, which results in different rates being used that can cause an imbalance. The CTA account is also used wherever consolidation across accounts with different rate types occurs, such as the consolidated trial balance. See [Cumulative Translation Adjustment (CTA) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124272.html).

### Related Topics

-   [Currency for Multiple Subsidiary Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N279420.html)
-   [Introduction to NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N266468.html)
-   [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html)
-   [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html)
-   [Set up NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268052.html)
-   [Intercompany Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1549982657.html)
-   [Intercompany Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158142795285.html)
-   [Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1486105.html)
-   [Viewing Open Intercompany Balances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_159430217340.html)
-   [Subsidiary Settings Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1541422716.html)
-   [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html)
-   [Subsidiary Navigator](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3811225086.html)
-   [OneWorld ERP Accounting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N279572.html)
-   [OneWorld CRM](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281005.html)
-   [OneWorld and SuiteCommerce](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282701.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
