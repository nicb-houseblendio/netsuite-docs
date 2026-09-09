---
id: "section_N2103948"
type: "section"
title: "Customizing Cash Flow Statement Account Sections"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Available Financial Statements > Cash Statements > Customizing Cash Flow Statement Account Sections"
parent: "section_N2103136"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103948.html"
anchors: ["bridgehead_N2104206"]
sha256: "7b2b90dfbfd2b4ea3cef18a72da1c7d6c830acc7c1a1f9a5b51f8159e841ffd8"
---

The standard Cash Flow Statement's Cash at Beginning of Period row references the Total Cash row in the standard Cash Statement. Consequently, if you create a custom Cash Flow Statement that includes changes to standard account sections, it's likely to have an incorrect value for Cash at Beginning of Period. This is because the Total Cash value referenced from the Cash Statement doesn't include the added or changed sections.

To avoid this issue, create a custom Cash Statement that shares the Cash Flow Statement's added or changed sections. Then, define this custom Cash Statement as the reference report for your custom Cash Flow Statement's Cash at Beginning of Period row.

See the following example to get a better understanding of how to match up Cash Flow Statement and Cash Statement section customizations. This helps maintain an accurate value for the Cash at Beginning of Period row.

For information about the permissions required to view and customize financial statements, see [Permissions and Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html#bridgehead_4425151234).

## Example Cash Flow Statement Customization {#bridgehead_N2104206}

This example provides steps for customizing the Cash Flow Statement to reflect non-cash additions and deductions to Net Income, such as depreciation and amortization.

1.  Customize the Cash Flow Statement to add an Expense section.
    
    1.  Go to _Reports > Financial > Cash Flow Statement_ and click **Customize** after the report loads.
        
    2.  On the Financial Report Builder Edit Layout page, set the **Name** to **Custom Cash Flow Statement**.
        
    3.  In the Layout section, expand the **Adjustments to Net Income** item, and select the row directly below it.
        
    4.  From the **Add Row/Section** list, select **Add Financial Section**.
        
    5.  In the popup, choose **Create New Section**, and click **OK**.
        
    6.  Set **Header Label** to be **Expense**, **Child Of** to be **Adjustments to Net Income**, and **Display** to be **Can not Expand**.
        
    7.  On the **Section** subtab, click **Share Section**.
        
    8.  For the **Section Name/ID**, enter **Expense Section**.
        
    9.  Set section criteria. Check the **Use Expressions** box. Select **Account Name** from the **Filter** list, choose **Depreciation Expense**, select **Or** from the **And/Or** list, and click **Add**. Select **Account Name** from the **Filter** list, choose **Amortization Expense**, select a blank from the **And/Or** list, and click **Add**.
        
    10.  Click **Save**.
         
2.  Customize the Cash Statement to add an Expense section.
    
    1.  Go to _Reports > Banking/Budgeting > Cash Statement > Customize Summary_.
        
    2.  On the Financial Report Builder Edit Layout page, set the **Name** to **Custom Cash Statement**.
        
    3.  In the Layout section, select the row directly below the **Cash Accounts**.
        
    4.  From the **Add Row/Section** list, select **Add Financial Section**.
        
    5.  In the popup, choose **Use Existing Shared Section**, for **Section Name/ID** enter **Expense Section**, and click **OK**.
        
    6.  For **Header Label** enter **Expense**, and for **Child Of** enter **Cash Accounts**.
        
    7.  Click **Save**.
        
3.  Set the Custom Cash Flow Statement's Cash at Beginning of Period Row to reference the new Custom Cash Statement.
    
    1.  Go to Reports > Saved Reports > Custom Cash Flow Statement > Customize.
        
    2.  On the Financial Report Builder Edit Layout page, select the **Cash at Beginning of Period** row.
        
    3.  Select the **Custom Cash Statement** from the **Report** list, select **Total Cash** from the **Row** list, and click **Save**.
        

Cash at Beginning of Period now includes expense accounts added to the Expense Section.

### Related Topics

-   [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Adding a Section to a Custom Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html)
-   [Cash Flow Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103273.html)
-   [Cash Statement Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2104490.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
