---
id: "section_N690632"
type: "section"
title: "Displaying Saved Search Results in Dashboard Portlets"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Displaying Saved Search Results on Your Dashboard > Displaying Saved Search Results in Dashboard Portlets"
parent: "section_N689267"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690632.html"
anchors: ["procedure_N690683"]
sha256: "06e7b1979d31f04f3aad01c010dad7dd21b972d533b9b89a9ee755bd94792dd7"
---

To make dynamically updated saved search results immediately available, you can add Custom Search portlets to dashboards on one or more NetSuite tabbed pages. Each Custom Search portlet displays results for a saved search that you select. Results are updated every time the page loads. The portlet also has a Refresh link that you can click to update search results. In addition, you can change the search portlet title by assigning a custom title to this portlet.

Note:

When placed in the right or left narrow columns of a dashboard, custom search portlets display only the first 2 results columns of the saved search. When placed in the center column, they display the first seven results columns. Custom search portlets also include New, Edit, and View columns with clickable links for each result record. If your saved search results include fields using custom labels that contain HTML markup or JavaScript code, those fields may not be displayed correctly in the dashboard view.

You are limited to six Custom Search portlets on the home page dashboard, but if you want to display results of additional searches on your dashboard, you have some other options to make this happen. For information, see [Displaying Multiple Saved Searches on Your Home Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690950.html).

#### To add a Custom Search portlet to a page: {#procedure_N690683}

1.  On the page where you want to display saved search results, click **Personalize Dashboard**.
    
2.  In the **Personalize Dashboard** panel, under the **Standard Content** folder, click or drag the **Custom Search** item.
    
3.  In the **Custom Search** portlet, click **Set Up**.
    
4.  In the **Custom Search** setup window:
    
    1.  Select a saved search from the **Search** dropdown list.
        
    2.  In the **Custom Portlet Title** field, you can specify your custom title for this custom search portlet.
        
    3.  In the **Results Size** field, enter the number of results you want displayed at one time in the portlet. If the total number of results exceeds this number, a **From-To** dropdown list appears that you can use to go to the results pages.
        
    4.  In the **Drill Down** field, select whether to open an individual result in the portlet or in a new page. If you set this option as **To New Page**, you will be redirected to a page that displays the results for the drilldown.
        
    5.  (If the Inline Editing feature is enabled) Check or clear the **Allow Inline Editing** box to indicate whether records returned as search results can be edited directly in the portlet.
        
        -   When the Inline Editing feature is enabled in an account, inline editing is available by default in all custom search portlets. You can clear this box to selectively disable inline editing per portlet.
            
        -   To limit other users' inline editing of custom search portlets, you can disable the **Allow Inline Editing** option for these portlets in personalized dashboards that you publish to users. See [Publishing Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N633149.html).
            
        -   For details about inline editing capabilities, see [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html).
            
    6.  Click **Save**.
        
5.  You can move the portlet around on the dashboard. For information, see [Arranging Dashboard Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N581190.html).
    

When search results are available in the portlet, you can choose to view or edit records. If you have Inline Editing enabled, you can edit information shown in the portlet without opening the record and the record is updated automatically. You also may be able to use Quick Add to create a new record or add new information to a record, all from within the portlet, or to click **Edit** in the portlet to modify the saved search definitions.

If you do not need access to full search results on your dashboard, you can use the following alternatives for quick access to saved searches:

-   Include summary results for saved searches on your dashboard by defining them as custom KPIs. You can display them in Key Performance Indicators, KPI Scorecard, KPI Meter, or Trend Graph portlets. See [Custom KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N609047.html).
    
-   Add links to saved search results pages in your dashboard Shortcuts portlet. See [Creating Shortcuts to Saved Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690347.html).
    

### Related Topics

-   [Displaying Saved Search Results on Your Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N689267.html)
-   [Creating Shortcuts to Saved Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690347.html)
-   [Displaying Multiple Saved Searches on Your Home Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690950.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
