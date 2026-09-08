---
id: "section_N265988"
type: "section"
title: "Using Per-Line Classifications"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Using Per-Line Classifications"
parent: "chapter_N261411"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html"
anchors: ["bridgehead_N266003", "bridgehead_3705023045"]
sha256: "7e17d60ddfabb238c8c465de9cab34cc2c8742237bc221bba80720f8d8c5b00c"
---

If you enable classifications such as departments, classes, locations, and custom segments, a field for each classification shows in the header of transaction forms. When you select a classification in a transaction header, all lines on that transaction use that classification. For example, if you choose the location East Coast in the Location field on a sales order, all lines on that sales order use East Coast.

You can also use per-line classifications to select a classification on each transaction line. You can use per-line classifications instead of header classifications or you can use both.

## Per-Line Classifications Only {#bridgehead_N266003}

If you use per-line classifications instead of header classifications, you'll see a classification field on each transaction line, but not in the header. For example, if Locations is enabled, there's a Location field on each transaction line. You can choose the location East Coast on one line and West Coast on another.

The items on each line are associated with individual locations, but the entire transaction isn't associated with a location. For example, on an invoice, line one is associated with East Coast and line two is associated with West Coast, but the Accounts Receivable line isn't associated with any location.

## Per-Line Classifications with Header Classifications {#bridgehead_3705023045}

If you use per-line classes, departments, locations, or custom segments, you can customize transaction forms to show the classification at both the header and line level.

For example, if you enable both Locations and Allow Per-Line Locations, a Location field displays on each transaction line **and** the form header. You can choose the East Coast on one line and West Coast on another. Then, you can choose United States in the transaction header so the Accounts Receivable line is associated with the United States.

These classifications are useful if you use locations for legal entities or geographical segments and want to report separate balance sheets and income statements for each. From the previous example, a sales order posts line items to the correct locations (East and West Coast), while the header location lets you run a correct income statement for United States transaction totals. For example:

Location: United States

Sublocation: East Coast

Sublocation: West Coast

When you use a form customized to show classification fields at both the header and line level, both are required. If either the line or header field isn't filled, both are cleared unless required. If you've enabled a preference to make classes, departments, locations, or custom segments required, then you have to select them at both the header and line level.

Note:

Tax and shipping lines use the class selected in the transaction header, if there is one.

The following preferences can be set at _Setup > Accounting > Accounting Preferences_:

-   **Make Departments Mandatory**
    
-   **Make Classes Mandatory**
    
-   **Make Locations Mandatory**
    
-   **Allow Per-Line Departments**
    
-   **Allow Per-Line Classes**
    
-   **Always Allow Per-Line Classifications on Journals**
    
    For only journal entries, this preference overrides any other **Allow Per-Line** preferences you have set.
    
-   **Allow Non-Balancing Classifications on Journals**
    
-   **Allow Empty Classifications on Journals**
    

For more information about these preferences, see [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).

To specify that a custom segment is required, check the Mandatory box on the Validation & Defaulting subtab of the Custom Segment configuration page.

For more information about customizing a form to set a classification at both the header and line level, see [Customizing Forms for Per-Line and Header Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N266299.html).

### Related Topics

-   [Classifications in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N261411.html)
-   [Classifications Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261486.html)
-   [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html)
-   [Locations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
