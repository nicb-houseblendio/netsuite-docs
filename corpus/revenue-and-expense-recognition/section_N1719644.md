---
id: "section_N1719644"
type: "section"
title: "Creating an Item Group VSOE Bundle"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Creating VSOE Bundles > Creating an Item Group VSOE Bundle"
parent: "section_N1719451"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719644.html"
anchors: ["procedure_N1719664"]
sha256: "45289bd56acc54214618ae32a66387a6cd89846b300f346cfda7b6047737d0db"
---

To sell vendor-specific objective evidence (VSOE) item group bundles, create an item group record to identify the members of the bundle.

Note:

If you include an item group VSOE bundle in a transaction VSOE bundle, allocation ignores the item group settings and allocates across the entire transaction.

#### To set up a bundled item group record: {#procedure_N1719664}

1.  Go to _Lists > Accounting > Items > New_.
    
2.  Click **Item Group**.
    
3.  On the **Revenue Recognition / Amortization** subtab, check the **Is VSOE Bundle** box.
    
4.  Click the **Purchasing/Inventory** subtab.
    
5.  In the **Item** field, select the first item that is a member of this bundle.
    
    The VSOE settings from this member's item record appear, such as discount, deferral, and delivery settings. You can change these settings if needed.
    
6.  Click **Add**.
    
7.  In the **Item** field, select and add all member items to complete this bundle.
    
    VSOE bundles must contain at least two members.
    
8.  Complete other fields on the item record as necessary.
    
9.  Click **Save**.
    

Now, these members are identified as a group bundle. When this item group is sold, the VSOE prices are allocated and deferred according to the VSOE settings for its member items. See [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html).

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Creating VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719451.html)
-   [Creating a Transaction VSOE Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719864.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
