---
id: "section_N1186943"
type: "section"
title: "Using the Project Consolidation Preference"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Using the Project Consolidation Preference"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186943.html"
anchors: []
sha256: "5a496ad3377c7b74f06d923ff7727a065a7970b1237dcdd6c000d3d4996b8d33"
---

The Consolidate Projects on Sales Transactions preference determines whether you track one project on sales transactions at the header level or multiple projects at the line level. It also determines how [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html) creates projects from items.

Project consolidation affects project creation and transaction processing.

-   With Consolidate Projects Enabled **:**
    
    You can associate one project with each line item on sales transactions, such as a billable item, expense, or time. The customer relationship displays at the header.
    

If you use Project Management and create projects in bulk from items, one project is created for each project-tagged line item on sales transactions and each project is billed separately to the customer. The estimated revenue for each project is the net amount of the corresponding line item.

-   With Consolidate Projects Disabled:
    
    Disable this preference to associate all items on a sales transaction with only one customer or project. The customer and project displays at the header level.
    

If you use Project Management and create projects in bulk from items, one project is created that contains all project-tagged line items on the order. In other words, project-generating items are consolidated and billed as one project. The estimated revenue for each project is the sum of the net amounts of all corresponding line items.

Note:

When the consolidation preference is enabled, you are no longer able to issue sales transactions to a specific project. Instead, you issue the sales transactions to the customer with line items attributed to each project.

For details about creating projects from items, read [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html) and [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html).

#### To set the Consolidate Projects on Sales Transactions preference:

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_. Choose **Items/Transactions**.
    
2.  In the Sales & Pricing section, set your preference for consolidating projects based on the information above.
    
    -   Check the **Consolidate Projects on Sales Transactions** box to enable the preference.
        
    -   Clear the **Consolidate Projects on Sales Transactions** box to disable the preference.
        
3.  Click **Save**.
    

Using this preference can affect the following:

-   Steps for [Refreshing Project Items on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204541.html).
    
-   [Billing and Project Consolidation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205308.html)
    

### Related Topics:

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
