---
id: "section_N585781"
type: "section"
title: "Creating Custom Reminders"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Dashboards Overview > Setting Up Dashboard Portlet Content > Setting Up Reminders > Creating Custom Reminders"
parent: "section_N581945"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N585781.html"
anchors: ["procedure_N585797", "bridgehead_N586073"]
sha256: "b178db301e383a90d843aedd4dd1682fe98473f120f903035b817e100da587f3"
---

If the reminders NetSuite provides don't meet all your needs, you can create your own and add them to the Reminders portlet on your dashboard. Each reminder is based on a count of the results of a saved search.

To create a custom reminder, enable the **Available for Reminders** option on the saved search definition page. When you do, the saved search is listed as a reminder on the Set Up Reminders page, and you can choose to show it in the Reminders portlet.

#### To create a custom reminder: {#procedure_N585797}

1.  Create a new saved search or edit an existing saved search. See [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
    
2.  On the saved search definition page, check the **Available for Reminders** box.
    
    ![Saved Case Search page with the Available for Reminders box selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/RemCheckBox.png)
3.  Make sure the search name is something you'll recognize in the Reminders portlet.
    
    The search name is displayed in the Reminders portlet, with the format: <number\_of\_results> <saved\_search\_name>
    
4.  On the **Results** subtab of the saved search, check whether any summary types that group search results are included.
    
    -   Custom reminders work best for saved searches with no grouped results. Reminders are based on a count of the number of results and only display when there's a non-zero count.
        
    -   If you set up a reminder for a saved search that groups results by a summary type other than a count, the reminder won't display.
        
    -   You can add a count for a grouped field so the reminder displays, but grouping may affect what's shown, so it might not be a true total.
        
    -   It's usually best to remove summary types or make a separate search without them for reminders.
        
    -   For information about grouping search results with summary types, see [Summary Types for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659258.html).
        
5.  Click **Save** to save the search.
    

#### To add a custom reminder to the Reminders portlet:

1.  Go to your home page. If this page does not include a Reminders portlet, click **Personalize Dashboard** and add it. See [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html).
    
2.  In the Reminders portlet menu, click **Set Up**.
    
3.  In the **Type** list, select **Custom**.
    
    You'll see your available custom reminders listed
    
    All saved searches you can access are listed if **Available for Reminders** is checked. The list isn't limited to only searches you created. See [Accessing a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N685689.html).
    
4.  Click a reminder in the left list or drag it to the **Current Selections** list on the right.
    
5.  You can change the reminder order by dragging them up or down in the Reminders portlet.
    
6.  If you want a reminder to be a headline, drag it under Headline.
    
    Headline reminders are displayed in the upper part of the portlet and use a more prominent layout.
    
7.  If you want reminders to show up even with zero results, check **Show reminders with zero results**.
    
8.  When ready, click **Save**.
    

The Reminders portlet displays a count of search results. Click a custom reminder to see detailed search results and complete related tasks.

Note:

If a custom reminder causes an error that prevents the Reminders portlet from displaying reminder links properly, click **Set Up** in the Reminders portlet's menu, remove the reminder from the Current Selections list, and click Save. Optionally, you can edit the related saved search and clear the Available for Reminders box. After you save this change, the problematic reminder is removed, and the portlet should be able to display. Note that you may need to refresh the page.

## Example Custom Reminder {#bridgehead_N586073}

Custom reminders are based on saved search results, which enables you to include more fine-tuned reminders in your dashboard. This can be especially helpful when you need reminders for custom record types, because system-defined reminders are not provided for custom records.

For example, if your account has an Equipment custom record with a Last Service field, and you're in charge of service scheduling, you can create a saved search and custom reminder to track if Equipment was serviced in the last Fiscal Year.

#### To set a custom reminder for servicing Equipment:

1.  Go to _Reports > Saved Searches > All Saved Searches > New_, and choose **Equipment Service**.
    
2.  A saved search definition page opens.
    
3.  Enter a meaningful name for the search.
    
4.  Check the **Available for Reminders** box.
    
5.  On the **Criteria** subtab, define a filter for the Last Service field to include equipment records with a Last Service is within last fiscal year.
    
6.  On the **Results** subtab, choose the columns to be displayed in search results.
    
7.  Save the search.
    
    ![The Saved Equipment Search page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/equipment4.png)
8.  Go to your Home page. If this page does not include a Reminders portlet, click **Personalize Dashboard** and add it. See [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html).
    
9.  In the Reminders portlet, click **Set Up**.
    
10.  Click the new reminder on the left to move it to the right, and then click **Save**.
     
11.  Review the Reminders portlet on your Home page.
     
12.  Click **Reminder** to see the list of expiring warranties and the information you need to renew them.
     

### Related Topics

-   [Setting Up Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581945.html)
-   [System-Defined Reminders Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N582302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
