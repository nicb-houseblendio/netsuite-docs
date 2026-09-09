---
id: "section_N633690"
type: "section"
title: "Publishing a Dashboard"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Publishing Dashboards > Publishing a Dashboard"
parent: "chapter_N633149"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633690.html"
anchors: ["procedure_N633771"]
sha256: "d7749c50b3b9eaaf0b6f60cb05dcd3891c39259ba1459eebd1785f2747f24541"
---

You can share your personalized dashboard with other users in your center by publishing it. A published dashboard can consist of one tabbed page or of multiple pages. When you publish a dashboard, you define the roles for users who will see the published dashboard, and what changes users will be able to make to the published dashboard.

Note:

The minimum required screen width size when using a three column layout is 1400 pixels.

Before you attempt to publish a dashboard:

-   Verify that you have the Publish Dashboards permission by checking for the Publish Dashboard link in your home page Settings portlet.
    
-   Verify that the role you're currently using shares the same center as the roles to which you want to publish the dashboard. Do not begin personalizing a dashboard until you are sure that your role can publish to the users you want!
    
    For more information, see [Publish Dashboards Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633401.html).
    
-   Personalize the home page by adding portlets that you want to be part of the published home page dashboard. For more information, see [Setting Up Dashboard Portlet Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581550.html).
    
    Note:
    
    Please note that if your dashboard contains a calendar portlet that displays My Calendar, the published dashboard users will see their personal calendar, not the publisher's one.
    
-   Personalize one or more of your own tabbed pages to be part of the published dashboard. You can personalize a page by making changes to a standard NetSuite tabbed page, as described in [Dashboard Personalization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N578457.html). Or, you can create your own custom tabbed page, as described in [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html).
    
    When you create a custom tab, you select the centers where it will display. For example, for a tab used by sales reps, you would select the Sales Center, and for a tab used by accounting clerks, you would select the Accounting Center. You also have the option of making a tab display in all centers. However, be aware that tabs applied to all centers aren't available in published dashboards.
    

#### To publish a dashboard: {#procedure_N633771}

1.  Go to your home page, and in the **Settings** portlet, click **Publish Dashboard**.
    
2.  On the Publish Dashboard page, enter a name for the dashboard in the **Name** field, and, if desired, descriptive text in the **Notes** field. These fields are for your reference only and aren't exposed to other users.
    
3.  If you want to prevent users from removing Shortcuts portlet links on the published dashboard's pages, check the **Lock Shortcuts** box.
    
    -   When you enable this option, users still can add and reorder links in their Shortcuts portlets.
        
    -   For information about the Shortcuts portlet, see [Shortcuts Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N587785.html).
        
4.  To prevent users from removing Create New menu links on the published dashboard's page, check the **Lock New Bar** box.
    
    -   When you enable this option, users still can add and reorder links in their Create New menu.
        
    -   For information about the Create New menu, see [Create New Menu](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N588325.html).
        
5.  On the **Apply To Roles** subtab, select the roles to which you want to publish this dashboard and indicate whether to publish the dashboard to new users only or to both new and existing users.
    
    1.  Select a role from the **Role** list.
        
        Only roles tied to the center that your current role uses are listed here, because you can only publish a dashboard to roles that share your center. If a role isn't listed here, you can't publish the dashboard to it when you're logged in with your current role. You may be able to log in with a different role, personalize a dashboard, and publish it to additional roles. For more information, see [Publish Dashboards Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633401.html).
        
        Roles that are inactive aren't included in the list.
        
    2.  By default, for a dashboard being published for the first time **Override existing user's settings** is set to **Yes**, indicating that this dashboard should be published to existing users with the selected role, replacing their current dashboards. Clear this box if you want to publish the dashboard only to new users assigned the selected role.
        
    3.  Click **Add**.
        
    4.  Repeat the preceding steps for additional roles to which you want to publish the dashboard.
        
    
    Only a part of the published dashboard content may be available to some users. Users can view only the dashboard content that their assigned roles give them permission to see.
    
6.  On the **Apply To Tabs** subtab, select the tabbed pages that you've customized to be part of the published dashboard, and choose how you want to restrict users' changes to the published dashboard's pages.
    
    1.  Check the box in the **Apply** column next to each tabbed page you want to include in this dashboard.
        
    2.  In the **Mode** column, choose the level of restriction for users' changes to the selected page:
        
        -   **Unlocked** - lets users make all changes to the selected page.
            
        -   **Locked** - restricts users from making any changes to the selected page.
            
        -   **Add/Move Content** - enables users to add and rearrange portlets on the selected page, and at the same time prevents them from removing portlets.
            
        
        Note:
        
        The **Add/Move Content** option prevents users from removing not only portlets that were added as part of the published dashboard but also the portlets they added themselves.
        
        For more information, see [Restricting Users' Dashboard Personalizations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N634268.html).
        
7.  Click **Save**.
    
    The published dashboard is applied to users assigned the selected roles. They may need to log out and log back in to the system for changes to be visible. They also may need to clear their browser cache.
    

### Related Topics

-   [Publishing Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N633149.html)
-   [Publish Dashboards Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633401.html)
-   [Applying Changes to Published Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N634404.html)
-   [Copying a Published Dashboard to Another Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554476919.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
