---
id: "bridgehead_N281858"
type: "bridgehead"
title: "Quota-Based Commission Schedules in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > OneWorld CRM > Employee and Partner Commission in OneWorld > Quota-Based Commission Schedules in OneWorld"
parent: "section_N281296"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281858.html"
anchors: ["svg_1", "svg_1Node_2", "svg_1Arrow_1", "svg_1Arrow_1_4_", "svg_1Arrowhead", "svg_1background", "svg_1Arc_Arrow_Solid", "svg_1Arc_Arrow_Solid_1_"]
sha256: "c883c8072d8c6b42bff8ac8beef3433aab210358c859b80602989ff65f3ec261"
---

A quota-based schedule for a subsidiary that has child subsidiaries includes the transactions from those child subsidiaries in the quota amount used for commission.

For example, if your company has the following subsidiary hierarchy:

<a id="svg_1"></a>

                                                                       

If you establish a quota for the U.S. parent subsidiary and for Wolfe U.K.:

-   Sales made for the U.S., U.K., or Germany subsidiaries are included toward the U.S. quota.
    
-   The U.K. quota would include only sales made on behalf of the U.K. subsidiary.
    

Following this example, a rep is assigned a commission plan with a schedule that is associated with the U.S. subsidiary. This schedule pays 10% of all sales exceeding quota.

The rep has a quota of $3000 for this period, and makes the following sales:

| Transaction | Subsidiary | Currency | Amount | Rate | Amount in USD |
| --- | --- | --- | --- | --- | --- |
| Invoice 1 | U.S. | USD | $1000 | U.S. to U.S.: 1 | $1000 |
| Invoice 2 | U.K. | GBP | £1000 | U.K. to U.S.: 2 | $2000 |
| Invoice 3 | CAN | CAD | $1000 | CAN to U.S.: .5 | $500 |

The rep exceeded quota by $500 and receives a commission payout equal to 10% of $500, or $50 USD.

Note:

If changes are made to the consolidated exchange rates, the commission schedule must be recalculated.

### Related Topics

-   [Consolidated Exchange Rates With Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281410.html)
-   [Authorize Commissions in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N282241.html)
-   [Employee and Partner Commission in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
