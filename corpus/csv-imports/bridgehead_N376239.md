---
id: "bridgehead_N376239"
type: "bridgehead"
title: "Setting Up Your CSV File for Matrix Items Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import > Importing Matrix Options for Items > Setting Up Your CSV File for Matrix Items Import"
parent: "section_N375701"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376239.html"
anchors: []
sha256: "8d9b629e7c4f0a218351c00b8c2a6cc40d9606fe5a0dfcd217b0393e0247bbe3"
---

The CSV file containing your matrix items data should include columns that map to the following fields. For best results, set the column headers to match these field names.

-   External ID: Preferred for all CSV imports, to serve as a unique identifier for each record.
    
-   Item Name/Number: Name for each matrix item.
    
-   Matrix Type: Possible values for this column are Parent Matrix Item, Child Matrix Item.
    
-   Subitem of: For each child matrix item, this column's value is the name of the parent matrix item. For each parent matrix item, this column is blank.
    
-   Columns that map to custom lists, such as Color, Size. Values for these columns should match those in the custom lists you set up.
    

Your CSV file also can include columns that map to other Item record fields.

Important:

In CSV import, updating parent item values for the Asset Account, Cost of Goods Sold (COGS) account, or Income Account fields doesn't automatically update child item field values. You need to set these values for each child item row. The system doesn't enforce that child item values match the parent item values for these fields, so you need to ensure that they match yourself.

The following table shows the contents of a sample matrix items CSV file. Notice that the parent matrix item is an individual record, and each child matrix item also is an individual record.

| External ID | Item Name/Number | Display Name/Code | Color | Size | Matrix Type | Subitem of |
| --- | --- | --- | --- | --- | --- | --- |
| 12000 | CottCrewSweat | Cotton Crewneck Sweater | \- | \- | Parent Matrix Item | \- |
| 12011 | CottCrewSweat-ES | Cotton Crewneck Sweater | Ecru | S | Child Matrix Item | CottCrewSweat |
| 12012 | CottCrewSweat-EM | Cotton Crewneck Sweater | Ecru | M | Child Matrix Item | CottCrewSweat |
| 12021 | CottCrewSweat-RS | Cotton Crewneck Sweater | Rose | S | Child Matrix Item | CottCrewSweat |
| 12022 | CottCrewSweat-RM | Cotton Crewneck Sweater | Rose | M | Child Matrix Item | CottCrewSweat |
| 12031 | CottCrewSweat-SS | Cotton Crewneck Sweater | SkyBlue | S | Child Matrix Item | CottCrewSweat |
| 12032 | CottCrewSweat-SM | Cotton Crewneck Sweater | SkyBlue | M | Child Matrix Item | CottCrewSweat |

### Related Topics

-   [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html)
-   [Item Types that Support Matrix Options Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375858.html)
-   [Prerequisites for Importing Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N375963.html)
-   [Setting Up Custom Lists and Item Fields for Matrix Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376031.html)
-   [Mapping Fields for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N376956.html)
-   [Tips for Matrix Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N377033.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
