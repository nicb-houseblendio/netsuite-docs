---
id: "chapter_N2890160"
type: "chapter"
title: "Custom Centers"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Centers"
parent: "book_N2823893"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2890160.html"
anchors: []
sha256: "4dce8fbc4f235bc63527a769e1012ee338d9b77fb4e57ea2e360abb3649138f0"
---

Administrators and users with Custom Centers permissions can create and apply custom centers to custom roles. To use the Custom Centers feature, you need to enable the Custom Records feature, at _Setup > Company > Setup Tasks > Enable Features_ > SuiteCloud.

NetSuite Centers determine which tabs and links are available for groups of similar user roles. For example, the Sales Center is used by the Sales Rep, Sales Manager, and Sales Administrator roles and includes tabs like Leads, Opportunities, and Forecast. For a visual representation of a center, see [Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2824967.html) in the [Customization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html) section.

Each tab contains links to transactions, lists, and setup pages, which are determined by the user's role and permissions for that role. For example, users assigned to the Sales Rep role would not see the same links on the Forecast tab as users with the Sales Administrator role because of permissions granted to each role. However, both roles share the Sales Center.

To create a custom center, you create a center record and then create its custom tabs. When you create custom tabs, you choose the center where you want the tab to appear. The center can be either an existing or custom center. You also choose the links and portlets that will appear in the center. You can customize centers and tabs only if the Custom Records feature is enabled.

Note:

Users can use only links and information that their roles have access to. To customize roles, go to _Setup > Users/Roles > Manage Roles_. You must create a new role to apply a custom center to it. To create a new role, click New on the Manage Roles page, select your custom center in the Center Type field and customize your new role.

Note that newly enabled feature menu items aren't automatically added to custom centers. You must manually add menu items to custom centers after a feature is enabled.

Important:

SuiteScript doesn't support direct access to the NetSuite UI through the Document Object Model (DOM). You should access the NetSuite UI only by using SuiteScript APIs. For information about using SuiteScript APIs to customize the UI, see [SuiteScript 2.1 Custom Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1518456405.html).

Custom Centers are supported in SuiteCloud Development Framework (SDF). SDF is a development framework that you can use to create SDF SuiteApps, or to customize NetSuite accounts, using an integrated development environment (IDE) on your local computer. SuiteCloud projects are file-based and use XML definitions of custom NetSuite objects. For more information, see [SDF Custom Object and File Development in SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4715411907.html).

See the following topics.

-   [Account-Specific Domains in Custom Center Links](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_157954623778.html)
    
-   [Creating and Editing Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890334.html)
    
-   [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html)
    
-   [Creating Center Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890916.html)
    
-   [Creating Center Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890916.html)
    
-   [Assigning a Custom Center to a Custom Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4363781223.html)
    

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2823893.html)
-   [Customization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html)
-   [Customization Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163039950342.html)
-   [Customizing Field Level Help for Standard Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1530729846.html)
-   [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html)
-   [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html)
-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Custom Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4172599049.html)
-   [Custom Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4313464438.html)
-   [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
