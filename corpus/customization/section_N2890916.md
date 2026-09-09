---
id: "section_N2890916"
type: "section"
title: "Creating Center Categories"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Centers > Creating Center Categories"
parent: "chapter_N2890160"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890916.html"
anchors: ["procedure_N2890962"]
sha256: "296ae716ef1b2725160ee333b4dbbe7438b57586c4cf4ff6b9e8ac6e6d3b7e27"
---

Administrators and users with the Custom Center Categories permission can create center categories.

Use the following steps to add custom categories to standard, built-in NetSuite tabs. After creating custom categories for standard tabs, you can then add links to each category. The links can go to NetSuite pages, custom records, Suitelets, or external websites. You need to enable the Custom Records feature to customize center categories.

Note:

To add custom categories to custom tabs, see [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html). On the Categories subtab, in the Label column, enter a name for a category of links. After creating the categories, you will later follow the steps in [Creating Center Links](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2891250.html) to assign specific links to each category.

#### To add custom categories to standard tabs: {#procedure_N2890962}

1.  Go to _Customization > Center and Tabs > Center Categories_ > **New**.
    
    ![Custom Center Category Values subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/CustCenterCategory.png)
2.  On the Center Category page, complete the following steps:
    
    1.  In the **Label** field, enter a category name.
        
    2.  In the **ID** field, enter an ID for the category, if required.
        
    3.  From the **Center Type** list, select an existing center.
        
        Note:
        
        If you're adding a custom category to a center tab that's configured to appear in all centers, you must select **Classic Center** as the **Center Type**. Selecting any other center type won't permit association of the category with an all-centers tab.
        
    4.  From the **Center Tab** list, select one of the standard, built-in NetSuite tabs (also referred to as sections).
        
    5.  From the **Insert Before** list, select where to insert the custom category.
        
3.  On the **Values** subtab, in the **Link** list, select the appropriate link.
    
    Available links include NetSuite pages, custom records, Suitelets, and external websites. Links to NetSuite pages, custom records, and Suitelets appear by default.
    
    To select a link to an external website, you must have already created that link by going to _Customization > Centers and Tabs > Center Link_. See [Creating Center Links](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2891250.html) for details. After the link is created, the link appears in the **Link** list.
    
4.  In the **Label** field, enter a UI label for the link.
    
5.  The short list setting is applicable to some center types. In the **Short List** column, to indicate that the link should appear in a portlet when the link is in a narrow column of the dashboard, check the box.
    
6.  Click **Add**.
    
7.  Click **Save**.
    
8.  On the **Translation** subtab, enter translated labels for the category. The Translation subtab is available only if the Multi-Languages feature is enabled in your account. For more information, see [Configuring Multiple Languages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N247147.html).
    

Note:

If you return to the tab and don't see the changes you've made, clear your browser cache.

You can use SuiteCloud Development Framework (SDF) to manage custom center categories as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual custom center category to another of your accounts. Each custom center category page has a clickable Copy to Account option in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

### Related Topics

-   [Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2890160.html)
-   [Creating and Editing Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890334.html)
-   [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html)
-   [Creating Center Links](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2891250.html)
-   [Assigning a Custom Center to a Custom Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4363781223.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
