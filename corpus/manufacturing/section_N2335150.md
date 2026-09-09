---
id: "section_N2335150"
type: "section"
title: "Creating Revision Records for BOM Control"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Bill of Materials Member Control for Assembly Items > Creating Revision Records for BOM Control"
parent: "chapter_N2332509"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335150.html"
anchors: ["procedure_N2335184", "bridgehead_N2335264"]
sha256: "c19f98b29f04ff68ed7c85b5d638304bbc27df7dbdf199f73956e7737d9a6ddf"
---

Important:

With the release of NetSuite 2023.1 Bills of Materials, where components are embedded to an Assembly Item, will no longer be supported. Only business critical issues will be fixed. To continue working with this functionality you should transition to the [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html) feature, which is free of charge. After you enable this feature, NetSuite will automatically migrate all of your Bill of Materials to the new structure.

When using the Revision Control method for Bill of Materials (BOM) management, create revision records to assign to assembly items. These revision records define effective and obsolete dates and can be assigned to many items.

Update effective and obsolete dates on the revision record one time to change the dates for many items.

#### To create a revision record: {#procedure_N2335184}

1.  Go to _Lists > Accounting > Item Revisions > New_.
    
2.  Select an **Item** to be associated with this revision.
    
    Required fields display a red asterisk (**\***).
    
3.  Enter a revision **Name**. For example, Version One.
    
4.  Enter the revision **Effective Date**.
    
5.  Enter a **Memo** about this revision. You can later search for this version by memo text, if needed.
    
6.  Check the **Inactive** box to not display this revision in lists.
    
7.  Click **Save**.
    

## Obsolete Dates {#bridgehead_N2335264}

Obsolete dates on a revision record cannot be edited. You can set the effective date and then save the revision. NetSuite then determines the obsolete date to avoid gaps or overlaps in dates covered by revisions.

The obsolete date field does display a value if you try to insert a revision record between two others.

For example, you have a default revision and one with an obsolete date of 1/1/2017. The default revision has an obsolete date of 12/31/2017. Next, you create a revision with an effective date of 1/1/2017. In this case, the obsolete date is set to 12/31/2017. After you save, NetSuite changes the obsolete date of the Default revision to 12/31/2016. If you create another revision with an effective date of 1/1/2018, it has no obsolete date. This is because it is the one with the latest effective date. When you save it, it still has no obsolete date and the 2017 revision has its obsolete date set to 12/31/2017.

Note:

You can use the Import Assistant to add or update item revision records based on CSV file data. For more information, see [Item Revision Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395019.html).

### Related Topics

-   [Setting Up BOM Control on Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334154.html)
-   [Setting an Assembly to Use Revision Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334812.html)
-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
