---
id: "section_N2334812"
type: "section"
title: "Setting an Assembly to Use Revision Control"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Bill of Materials Member Control for Assembly Items > Setting an Assembly to Use Revision Control"
parent: "chapter_N2332509"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334812.html"
anchors: ["procedure_N2334824"]
sha256: "fe1e2562ca8d38ef9c3e50f9709a8e7e2a0dd96d45a44788b23841e5be7a3f52"
---

Important:

With the release of NetSuite 2023.1 Bills of Materials, where components are embedded to an Assembly Item, will no longer be supported. Only business critical issues will be fixed. To continue working with this functionality you should transition to the [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html) feature, which is free of charge. After you enable this feature, NetSuite will automatically migrate all of your Bill of Materials to the new structure.

To use revision records to manage effective and obsolete dates, set the assembly record to use revision control.

#### To set an assembly to use revision control: {#procedure_N2334824}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the assembly item record you want to set.
    
3.  On the **Purchasing/Inventory** subtab, in the **Effective BOM Control** list, select **Revision Control**.
    
    Note:
    
    If you select Revision Control, you must use revision control for this item.
    
4.  The **Default Revision** field displays the default revision for this item.
    
5.  If you are creating a new item record, click **Save** and then click **Edit** to re-open the item.
    
    If you are editing an item already set to revision control, go to the next step.
    
6.  Click the **Components** subtab.
    
7.  Select an existing member **Item** or add a new one.
    
8.  In the **Effective Revision** field, enter a revision or create a new one. The revision record effective date determines the start time when this item is included as a member for an assembly.
    
    For each member, the default selection is **Default**. The item will then be included in builds by default.
    
    1.  To define a non-default date revision record, in the **Effective Revision** field, select **New**
        
    2.  In the **New Item Revision** popup window, define the following for the assembly item:
        
    
    -   **Name** (for example, Version 2)
        
    -   **Effective Date** (for example, 4/1/2020)
        
    -   **Memo** - Optionally enter a memo.
        
    -   **Inactive** - Check this box to not display this revision in lists.
        
    
    Alternatively, enter new revision records at Lists > Accounting > Item Revisions. For more information about revision records, see [Creating Revision Records for BOM Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335150.html).
    
    For more information about using effective fields, see [Setting Up BOM Control on Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334154.html).
    
9.  Select an **Obsolete Revision**. The obsolete revision record date determines the end time that an item is to be used for an assembly.
    
    When you select an obsolete revision, the correct obsolete date displays in that field.
    
10.  Click **Done** or **Add**.
     
11.  Repeat the steps 1 to 4 for each member item you want to assign a revision to.
     
12.  Click **Save**.
     

The BOM for this assembly is determined by referencing the production date of each work order against the revision record dates for member items.

### Related Topics

-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
