---
id: "section_N1040011"
type: "section"
title: "Sales Territories"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Sales Territories"
parent: "chapter_N1035717"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html"
anchors: ["svg_1", "svg_1Node_3_", "svg_1Node_5_", "svg_1Node_4_", "svg_1Node_1_", "svg_1Node_17_", "svg_1Node_8_", "svg_1Node_7_", "svg_1Node_6_", "svg_1Node_16_", "svg_1Node_15_", "svg_1Node_14_", "svg_1Node_13_", "svg_1Node_12_", "svg_1Node_11_", "svg_1Node_10_", "svg_1Node_9_"]
sha256: "87ce25c004c4343adfa7bc8a4bf36c01e59370cfa4e3d412d15a201df279b9be"
---

Sales territories use sales rules to determine how NetSuite distributes new potential customers to your sales reps, sales groups, and sales teams.

In NetSuite, you can define sales territories by using multiple sales rules. The information in a lead, prospect, or customer's record has to match one or more of the sales rule criteria to get assigned to that territory.

Note:

Territory assignment works on a first come, first served basis. When NetSuite finds a successful Sales Territory rule and assigns the Lead, it stops processing Sales Territory rules. Subsequent rules aren't considered and can't overwrite the initial assignment.

For example, Wolfe Electronics assigns most of their leads to traveling sales reps based on geographic location. The company also purchases lists of leads to cold call and assigns them to telesales reps.

Wolfe sales administrators want leads from purchased lists to go to the telesales team regardless of their location. They set up a sales territory that filters all leads with the lead source: Imported List.

On the Manage Sales Territories page, the sales administrator gives this territory priority over the geographic territories. This way, NetSuite separates these leads before it assigns them based on their location.

When a new lead record is created and it has the Imported List lead source, NetSuite assigns it to the internal sales team, even if the lead's address matched the criteria of the Mountain West territory. If it has a different lead source, NetSuite assigns it to the geographic sales territory that matches its telephone area code.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                       

To automate lead prospect and customer assignment, all new leads and prospects should fit the sales rules. Go to Setup > Sales > Sales Management > Sales Rules to edit or add sales rules. After you group the rules into territories, NetSuite assigns sales reps and sales groups to the territories. Then, NetSuite automatically sends new customers to the correct sales person or team.

By default, NetSuite assigns customers to sales reps through a round robin process, if they are not assigned by sales territories.

Note:

NetSuite only assigns newly created lead, prospect, and customer records by sales territories. It doesn't reassign records that were already assigned to a sales rep or sales team. To reassign, you can use the Reassign Customers by Sales Territory Rules mass update. For more information, see [Reassigning Customers to Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1042981.html).

### Related Topics

-   [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html)
-   [Sales Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039705.html)
-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)
-   [Reassigning Customers to Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1042981.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
