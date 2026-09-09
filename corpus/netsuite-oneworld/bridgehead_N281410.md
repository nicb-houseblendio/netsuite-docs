---
id: "bridgehead_N281410"
type: "bridgehead"
title: "Consolidated Exchange Rates With Commissions"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > OneWorld CRM > Employee and Partner Commission in OneWorld > Consolidated Exchange Rates With Commissions"
parent: "section_N281296"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281410.html"
anchors: ["svg_1", "svg_1Node_2", "svg_1Arrow_1", "svg_1Arrow_1_4_", "svg_1Arrowhead", "svg_1background", "svg_1Arc_Arrow_Solid", "svg_1Arc_Arrow_Solid_1_"]
sha256: "7a1d0bb18e1f14226f66965e631784e86a9aff44c965dff648bc14dc39516eda"
---

When NetSuite converts commission amounts to the base currency of the employee or partner's subsidiary, it uses consolidated exchange rates. You can view consolidated exchange rates at _Lists > Accounting > Consolidated Exchange Rates_.

For example, if a company has the following subsidiary hierarchy:

<a id="svg_1"></a>

                                                                       

Three invoices qualify for commission:

| Transaction | Subsidiary | Currency | Commission Amount |
| --- | --- | --- | --- |
| Invoice 1 | U.S. | USD | $100 |
| Invoice 2 | U.K. | GBP | £100 |
| Invoice 3 | Germany | euro | €100 |

The estimated commission reports, commission plan, and commission transaction display the commission amounts converted to USD. This conversion is based on the consolidated exchange rates table for the period in which each transaction was booked:

| Amount | Exchange Rate | USD Amount |
| --- | --- | --- |
| $100 | U.S. to U.S.: 1 | $100 |
| £100 | U.K. to U.S.: 2 | $200 |
| €100 | EURO to U.S.:.5 | $50 |

Note:

NetSuite stores the exchange rates used for commission calculations. If the rate on the consolidated exchange rates table changes, the schedule must be recalculated to reflect the change.

A quota for a sales rep associated with the U.S. subsidiary would include sales made for the U.S. subsidiary and its child subsidiaries.

### Related Topics

-   [Quota-Based Commission Schedules in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281858.html)
-   [Authorize Commissions in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N282241.html)
-   [Employee and Partner Commission in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
