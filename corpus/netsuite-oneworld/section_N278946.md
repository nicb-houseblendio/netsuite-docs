---
id: "section_N278946"
type: "section"
title: "Subsidiary Context for Reports"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Consolidated Reporting in OneWorld > Subsidiary Context for Reports"
parent: "section_N278654"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278946.html"
anchors: []
sha256: "21f67932ac304f4030f6a9593aabdeef93d9a684a41cdaf14f9798364821709c"
---

If you have access to multiple subsidiaries, you can view the data for all subsidiaries at one time. You can also view data for individual subsidiaries. In the report footer, select the subsidiary in the Subsidiary Context filter.

Note:

The Subsidiary Context list includes active subsidiaries and inactive subsidiaries with posted transactions. Inactive subsidiaries without posted transactions are hidden.

Note:

If you use Multi-Book Accounting, you can run consolidated reports for any accounting book enabled for consolidation. Use the Accounting Book list to choose the primary or secondary accounting book that correlates with the selected subsidiary context.

When you select a subsidiary, including elimination subsidiaries, NetSuite filters the report data to display data only from the selected subsidiary. In the case of consolidated subsidiaries, the data that displays is for all child subsidiaries of the consolidated parent subsidiary, including elimination subsidiaries.

For example, if a company has the following subsidiary hierarchy:

![Diagram of subsidiary context specific to reporting.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/NetSuiteOneWorld/UnderstandingSubsidiariesContextForReports.png)

The Subsidiary Context filter on reports would be organized as follows:

Wolfe US (Consolidated)

Wolfe US

Wolfe Germany

Wolfe UK (Consolidated)

Wolfe UK

Wolfe Japan

Wolfe Singapore

NetSuite inserts a virtual consolidated node for each parent. When you select a consolidated node, the data returned is a summary of all transactions associated with the node's child subsidiaries, including elimination subsidiaries.

If you use a role that is restricted to specific subsidiaries, the data returned is based on your level of access.

Using the preceding example hierarchy, if you have access to only the Japan subsidiary, the Subsidiary Context filter would be organized as follows:

Wolfe US (Context)

Wolfe UK (Context)

Wolfe Japan

You would see the following for each selection:

| Selection | Transactions Included | Currency Shown | Financial Statement Layout |
| --- | --- | --- | --- |
| Wolfe US (Context) | Wolfe Japan | US dollar | Wolfe US |
| Wolfe UK (Context) | Wolfe Japan | British pound (GBP) | Wolfe UK |
| Wolfe Japan | Wolfe Japan | Japanese yen | Wolfe Japan |

Because this role is restricted to a single subsidiary, the results do not include consolidated data. However, you can still see the data in Wolfe Japan as it would appear in the currencies and layouts of parent subsidiaries.

Important:

Some reports do not support consolidation and return results for only one subsidiary at a time. These reports do not include the Subsidiary Context filter in the report footer. Before you can run one of these reports, you must set your user preferences to restrict your view to a single subsidiary. Go to _Home > Set Preferences_ and then click the Restrict View subtab. See [Restrict Your Subsidiary View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278473.html).

### Related Topics

-   [Currency for Multiple Subsidiary Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N279420.html)
-   [Consolidated Reporting in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278654.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
