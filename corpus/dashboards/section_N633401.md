---
id: "section_N633401"
type: "section"
title: "Publish Dashboards Permission"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Publishing Dashboards > Publish Dashboards Permission"
parent: "chapter_N633149"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633401.html"
anchors: ["bridgehead_N633480", "bridgehead_N633533", "bridgehead_N633569"]
sha256: "61d9aa5587b7a28f0fae1d4104486d12269e3b826f02635839274685779e7fa4"
---

To publish dashboards, you must have the Publish Dashboards permission. A few administrative roles have this permission assigned by default, but most users don't. When you use the Publish Dashboard button, the dashboard will appear in the state of the dashboard for you and your corresponding role that is currently logged into NetSuite. If you make a change to a published dashboard, the dashboard will publish with those edits included. It's not possible to revert back to dashboard settings that were previously published.

If you have the Publish Dashboards permission, a Publish Dashboard link displays in the Settings portlet on your home page. If this link isn't available, you don't have the permission.

For information, see the following topics:

-   [Roles with Publish Dashboards Permission](#bridgehead_N633480)
    
-   [Adding the Publish Dashboards Permission](#bridgehead_N633533)
    
-   [Can Publish to Own Center Only](#bridgehead_N633569)
    

## Roles with Publish Dashboards Permission {#bridgehead_N633480}

By default, the Publish Dashboards permission is available to users assigned the following roles:

-   **Administrator** - can publish dashboards to users assigned roles in the Classic Center.
    
-   **Intranet Manager** - can publish dashboards to users assigned roles in the Ecommerce Management Center.
    
-   **Issue Administrator** - can publish dashboards to users assigned roles in the Engineering Center
    
-   **Marketing Administrator** - can publish dashboards to users assigned roles in the Marketing Center.
    
-   **Product Manager** - can publish dashboards to users assigned roles in the Support Center.
    
-   **QA Manager** - can publish dashboards to users assigned to roles in the Engineering Center.
    
-   **Sales Administrator** - can publish dashboards to users assigned roles in the Sales Center.
    
-   **Support Administrator** - can publish dashboards to users assigned roles in the Support Center.
    
-   **System Administrator** - can publish dashboards to users assigned roles in the System Administrator Center.
    

## Adding the Publish Dashboards Permission {#bridgehead_N633533}

If additional users require the Publish Dashboards permission, for example, in cases where centers don't have any existing roles with this permission, the account administrator can customize the users' roles to add the permission, or create a custom role with the permission.

For example, to allow the publishing of a dashboard to roles that use the Advanced Partner Center role, the account administrator can create a customized Advanced Partner Center role, add the Publish Dashboards permission to it, and assign the role to the user who needs to publish the dashboard.

The Publish Dashboards permission is listed on the Setup subtab of each Role record's Permissions subtab. For more information, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

Note:

If the Global Permissions feature is enabled, the account administrator can add the Publish Dashboards permission directly to employee records' Global Permissions subtab, to be applicable to all of the employees' assigned roles.

## Can Publish to Own Center Only {#bridgehead_N633569}

Be aware that even with the Publish Dashboards permission, you can publish dashboards only to other users with roles tied to the same center where you've personalized your dashboard, because only roles tied to the same center share the same set of tabbed pages. For example, if you're logged in as a sales administrator when you personalize a dashboard, only sales roles are available when you attempt to publish that dashboard.

The account administrator generally uses the Classic Center, which may not be shared with many other users. For this user to publish dashboards to users with roles in other centers, the user must be assigned an additional role for each center where a published dashboard is needed. If any of these roles don't have the Publish Dashboards permission, it needs to be added. Then, this user can log in with each role to personalize and publish a dashboard to roles for the related center.

In other cases, it may make more sense for different users to publish dashboards to different centers. In all cases, you should be aware of the center for your role, know which other roles share your center, and ensure that you have the Publish Dashboards permission, BEFORE you personalize a dashboard that you want to publish.

Note:

Dashboards published to the Advanced Partner Center are published to partner contacts as well as partners. If a partner or a partner contact modifies the dashboard content by, for example, adding a portlet, this change will appear on the dashboards of the partner and all partner contacts logged in using the same role.

### Related Topics

-   [Publishing Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N633149.html)
-   [Publishing a Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N633690.html)
-   [Applying Changes to Published Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N634404.html)
-   [Copying a Published Dashboard to Another Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554476919.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
