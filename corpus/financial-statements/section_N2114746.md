---
id: "section_N2114746"
type: "section"
title: "Adding a Section to a Custom Financial Statement"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Sections > Adding a Section to a Custom Financial Statement"
parent: "section_N2112804"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html"
anchors: ["procedure_N2114797"]
sha256: "5b44a9eebbfd08b943a15cc75cec3dd445756366a7953c906fed0432e701e0cd"
---

You can add sections to a custom financial statement. An added section can be:

-   a standard section defined within NetSuite
    
-   an existing custom section that has been designated as shared by its creator, meaning it can be used by any custom financial statement
    
-   a new custom section that you create
    

Warning:

To prevent unexpected results, don't add two or more different sections with overlapping criteria to a single financial statement. If an account fits the criteria for more than one section, the system determines the account's section, which may not be the one you expect.

#### To add a section to a custom financial statement: {#procedure_N2114797}

1.  Start the Financial Report Builder, and ensure an editable custom layout is selected in the Edit Layout page. For information, see [Accessing the Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2105846.html).
    
2.  In the Layout outline, select the row above which you want to insert the new section. (Note that you also can use the up arrow or down arrow buttons or drag and drop the section to move it after it's added.)
    
3.  From the **Add Row/Section...** dropdown list, select **Add Financial Section**.
    
    ![Screenshot of the Layout Add Row/Section list of the Edit Layout page in the Financial Report Builder with Add Financial Section selected](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/FinancialStatements/FRBSectionAdd.png)
4.  In the New Section Row popup, do one of the following:
    
    -   Choose the **Use Existing Shared Section** option, select a **Section Name/ID**, and click **OK**.
        
    -   Choose the **Create New Section** option, and click **OK**. Follow the instructions in [Adding a New Custom Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html#bridgehead_N2113321) to define section criteria.
        
5.  Make other edits to the section as desired. See [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html).
    

Note:

If you create a custom Cash Flow Statement that includes custom sections, its value for the Cash at Beginning of Period row is likely to be incorrect. To ensure accuracy, create a custom Cash Statement that shares these custom sections and make that custom Cash Statement the referenced report for the Cash at Beginning of Period row. For more information, see [Customizing Cash Flow Statement Account Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2103948.html).

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html)
-   [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html)
-   [Creating a Custom Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
