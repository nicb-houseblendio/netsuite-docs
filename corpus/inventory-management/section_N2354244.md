---
id: "section_N2354244"
type: "section"
title: "How Kits and Kit Parts Affect Quantities Displayed in Reports"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Reporting > How Kits and Kit Parts Affect Quantities Displayed in Reports"
parent: "chapter_N2353200"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2354244.html"
anchors: ["bridgehead_N2354327"]
sha256: "5daf9332fa72a8d3574b333db9933682e15b85fb1a19d09063d572224c117156"
---

When using reports that display inventory item quantities, it is useful to familiarize yourself with how kits and 'kit part' quantities are displayed. Some items can be listed both as parts of kits and as individual items, so quantities may appear larger than they are. This is especially relevant for the following reports:

-   [Items Pending Fulfillment Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2356254.html)
    
-   [Inventory Back Order Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2355658.html)
    
-   [Sales Back Order Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1315076.html)
    
-   [Sales Orders Pending Fulfillment Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1315755.html)
    

These standard reports show quantities for individual items which can include quantities attributed to kits. Using the Sold as a Kit/Assembly Member filter, you can modify the way that standard reports display quantities.

## Example using the Sold as a Kit/Assembly Member filter {#bridgehead_N2354327}

A Custom Items Pending Fulfillment Report might have the following two items of inventory:

-   DVD-R
    
-   DVD-R 5 Pack
    

The second item DVD-R 5 pack is a kit which consists of 5 DVD-R items. You have 4 kits of DVD-R 5 pack committed items and 3 DVD-R committed items. On the standard report those 2 line items will be displayed with the following quantities:

-   DVD-R: 23
    
-   DVD-R 5 pack: 4
    

This report correctly displays a total of 23 DVD-Rs committed. However, it does not highlight that 20 of the 23 are part of the kit listed as the next line item. This may in some cases give the illusion that 43 DVD-Rs have been committed, whereas in fact only 23 have been committed.

Using the filter Sold as a Kit/Assembly Member, you can modify the standard report. Set the filter to false and the report will display the following 2 line items:

-   DVD-R: 3
    
-   DVD-R 5 Pack: 4
    

Now the line item DVD-R does not include the 20 DVD-Rs sold as part of DVD-R 5 pack kits. See [Filtering Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742381.html) for more details on how to apply filters to reports.

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
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
