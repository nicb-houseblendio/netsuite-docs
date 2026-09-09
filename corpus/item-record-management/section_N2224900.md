---
id: "section_N2224900"
type: "section"
title: "Showing Groups on Member Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Item Groups > Showing Groups on Member Item Records"
parent: "section_N2224824"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224900.html"
anchors: ["procedure_N2224910"]
sha256: "a56127aea936fde35cec8428cfd3dda0f9f4f42612803411a3a82be0ebf793a3"
---

You can add a custom subtab on item records that shows the groups that item is a member of.

#### To apply a custom sublist to a standard item record: {#procedure_N2224910}

1.  Create a saved search for the information you want to show. The results of this search should include the information you want to show on your sublist.
    
    1.  Go to _Lists > Search > Saved Search > New_.
        
    2.  On the New Saved Search page, click **Item**.
        
    3.  On the Saved Item Search page, click the **Available Filters** subtab.
        
    4.  In the **Filter** column, select **Component Item**.
        
    5.  Click **Add**.
        
    6.  In the header, check **Available as a Sublist View**.
        
    7.  Enter a **Search Title**.
        
    8.  Click **Save**.
        
2.  Apply the sublist to item records.
    
    1.  Go to _Customization > Forms > Sublists_.
        
    2.  Click the **Item** subtab.
        
    3.  In the Custom Sublists page **Search** column, select the saved search that you created in step 1.
        
    4.  Enter a label for this sublist, such as **Groups**.
        
    5.  In the **Tab** column, select the subtab you want this sublist to appear on, such as **Inventory**.
        
    6.  Select the record you want this sublist to appear on, such as **Inventory**.
        
        This sublist shows on the standard and custom forms of the types you select.
        
    7.  Click **Add**.
        
    8.  Click **Save**.
        

The search results appear on the records you selected. Based on the suggestions in the preceding steps, you can view the record of an inventory item. Click Inventory > Groups to see which groups the item is a member of.

### Related Topics

-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
