---
id: "section_N581945"
type: "section"
title: "Setting Up Reminders"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Dashboards Overview > Setting Up Dashboard Portlet Content > Setting Up Reminders"
parent: "section_N581550"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html"
anchors: ["procedure_N581964", "bridgehead_4552875541"]
sha256: "f5822e2f571d8a152ed8d617468a9251c20a05d79d917d41e69196cdf32560fb"
---

You can set up reminders for important data or tasks in NetSuite. Reminders appear in the Reminders portlet on dashboards. Click a reminder to see more details and take action if needed.

![Reminders portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/Reminders_Headline.png)

For example, Wolfe Electronics sets up a reminder for receiving orders. When there are orders to receive, a reminder shows up in the Reminders portlet. A user clicks it to go to the Receive Orders page.

#### To add a Reminders portlet:

1.  If you don't see the Reminders portlet on your dashboard, click **Personalize** in the upper right corner of your dashboard, or click **Personalize Dashboard** in the **Settings** portlet.
    
2.  On the **Standard Content** tab of the **Personalize Dashboard** palette, click the **Reminders** icon or drag it onto the dashboard.
    
    ![Reminders portlet icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/Reminders_portlet_icon.png)

#### To set up the Reminders portlet: {#procedure_N581964}

1.  In the Reminders portlet's menu, click **Set Up**.
    
2.  Click a reminder in the left list or drag it to the **Current Selections** list on the right.
    
    The reminders are arranged alphabetically. To view custom reminders, select **Custom** from the **Type** list.
    
    The available system-defined reminders depend on your role and the features enabled in your account. For a list of the reminders NetSuite offers, see [System-Defined Reminders Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N582302.html). Custom reminders are available when saved searches to which you have access are marked as available for reminders. For information, see [Creating Custom Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N585781.html).
    
    ![Select reminders popup window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/Reminders_Setup.png)
3.  You can rearrange reminders in the portlet by dragging them up or down the list.
    
4.  If you want a reminder to be used as a headline reminder, drag it under the **Headline**.
    
    Headline reminders show up at the top and stand out more.
    
5.  If you want the reminders to be shown even when there are no results, select **Show reminders with zero results**.
    
6.  When ready, click **Save**.
    
    For each reminder with results, you'll see a count and a link. Click the reminder to see the matching task or search results.
    
    Note:
    
    The Reminders portlet refreshes every 30 minutes. The portlet displays the last refresh time, which indicates when the next refresh occurs.
    

You can add highlighting rules to any reminder. Each rule adds a color when a certain threshold is reached.

#### To set up highlighting rules:

1.  In the Reminders portlet, point to a reminder you want to edit and click the edit icon ![Edit Reminder icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/EditReminder_icon.png).
    
2.  To add a highlighting rule, click **Add Rule**, choose the color to use, and specify the threshold.
    
    You can add as many rules as you want.
    
    ![Edit reminder: Orders to Receive popup window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/Reminders_HighlightRules.png)
3.  Click **Save** to apply your highlighting rules.
    

## Reminder alerts {#bridgehead_4552875541}

The Reminders portlet displays a yellow triangle icon if a standard or custom saved search gets interrupted for any reason.

All other saved searches that finish successfully show a reminder count as expected. If you point to the icon, you'll see a hint based on your role, permissions, and saved search ownership.

![Reminders alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/Reminders_Alerts.png)

-   For Administrators, the message for errors for standard reminders appears as **Unable to load. Please contact Support**.
    
-   For non-Administrators, a message of **Unable to load. Please contact your Administrator** will appear.
    
-   For Administrators who are also owners, the message of **Unable to load. Please modify your search** will appear.
    
-   For Administrators who are not owners, the message of **Unable to load. Please contact the owner or create a new reminder** will appear.
    
-   For non-Administrators who are owners, the message of **Unable to load. Please modify your search** will appear.
    
-   For non-Administrators who are owners and can perform search, the message **View: Unable to load. Please change to a role with sufficient permissions and modify your search** will appear.
    
-   For non-Administrators who are not owners but can perform Search, the message **Full: Unable to load. Please contact the owner or create a new reminder** will appear.
    
-   For non-Administrators who are not owners and cannot perform search, the message **View: Unable to load. Please contact your Administrator** will appear.
    

### Related Topics

-   [Setting Up Dashboard Portlet Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581550.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
