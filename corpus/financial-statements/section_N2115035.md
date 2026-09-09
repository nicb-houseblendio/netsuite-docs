---
id: "section_N2115035"
type: "section"
title: "Adding Subsection Examples"
branch: "financial-statements"
category: "accounting"
breadcrumb: "Accounting > Financial Statements > Financial Report Builder > Financial Statement Sections > Adding Subsection Examples"
parent: "section_N2112804"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2115035.html"
anchors: ["bridgehead_N2115094", "bridgehead_N2115186"]
sha256: "9fe912aa1a4f73970bb31a994e0527d8ecca72794447faac3d285ca314e2ba7a"
---

On the Financial Report Builder's Edit Layout page, you can add subsections within any financial statement section or header and summary row grouping. You can indicate the subsection's parent section or parent header/summary row grouping by your selection in the Child Of dropdown or by the subsection's placement in the Layout outline. You may need to add a new header and summary row to group data from multiple subsections.

The following steps provide examples for adding subsections.

-   [Creating Two Income Statement Fixed Assets Subsections](#bridgehead_N2115094)
    
-   [Creating a Cash Flow Statement Depreciation Expense Subsection](#bridgehead_N2115186)
    

#### Creating Two Income Statement Fixed Assets Subsections {#bridgehead_N2115094}

1.  Go to Reports > New Financial Report, and choose the Standard Balance Sheet Layout.
    
2.  On the Financial Report Builder Edit Layout page, modify the **Name** for the report as desired.
    
3.  From the **Add Row/Section** list, select **Add Header and Summary Rows**.
    
4.  Edit the **Header Label** to be **Fixed Assets (new)** and the **Total Label** to be **Fixed Assets (new) - Total**.
    
5.  From the **Add Row/Section** list, select **Add Financial Section**. In the popup, choose **Use Existing Shared Section**, and select **Fixed Assets** from the **Section Name/ID** list. Click **OK** if a popup appears asking you if you want to continue.
    
6.  Edit the **Header Label** to be **Accumulated Depreciation (new)** and the **Total Label** to be **Accumulated Depreciation - Total**.
    
7.  In the **Child Of** list, select **Fixed Assets (new)**.
    
8.  On the **Section** subtab, click **Edit Criteria**, and click **OK** in the popup. Check **Use Expressions**. Select **Account Name** from the **Filter** list, and in the Filter popup, select all accumulated depreciation accounts.
    
9.  In the Layout outline, select the original Fixed Assets section, and change **Child Of** to **Fixed Assets (new)**.
    
10.  On the **Section** subtab, click **Edit Criteria**, and click **OK** in the popup. Check **Use Expressions**. Select **Account Name** from the **Filter** list. In the Filter popup, change the list selection to **None Of**, and select all depreciation accounts.
     
11.  Click **Save**.
     

#### Creating a Cash Flow Statement Depreciation Expense Subsection {#bridgehead_N2115186}

1.  Go to Reports > New Financial Report, and choose the Standard Cash Flow Statement Layout.
    
2.  On the Financial Report Builder Edit Layout page, modify the **Name** for the report as desired.
    
3.  From the **Add Row/Section** list, select **Add Financial Section**. In the popup, choose **Create New Section**.
    
4.  Change the **Header Label** to **Depreciation Expense** and the **Total Label** to **Depreciation Expense - Total**.
    
5.  In the **Child Of** list, select **Adjustments to Net Income**.
    
6.  In the **Display** list, select **Can not Expand**.
    
7.  On the **Section** subtab, select **Account Name** from the **Filter** list, and in the Filter popup, select all depreciation accounts.
    
8.  On the **Format** subtab under Account Row Format, check **Reverse Sign**.
    
9.  In the Layout outline, select the **Fixed Asset** section.
    
10.  On the **Section** subtab, click **Edit Criteria**, and click **OK** in the popup. Check **Use Expressions**. Select **Account Name** in the **Filter** column. In the Filter popup, change the dropdown to **None Of** and select all depreciation accounts.
     
11.  Click **Save**.
     

You need both the Financial Statements permission and the Report Customization permission to customize reports in the Financial Report Builder. If you don't have necessary permissions, contact your account administrator. See [Giving Access to Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N327139.html) for more information.

### Related Topics

-   [Financial Statement Sections](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2112804.html)
-   [Creating a Custom Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113041.html)
-   [Editing a Financial Statement Section](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2113644.html)
-   [Adding a Section to a Custom Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2114746.html)
-   [Organizing Financial Statement Data by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2124036.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
