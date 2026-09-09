---
id: "section_N697145"
type: "section"
title: "Creating a Search for Customers with No Recent Activity"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Saved Search Examples > Creating a Search for Customers with No Recent Activity"
parent: "section_N691341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N697145.html"
anchors: ["kaltura_player_44", "procedure_N697166"]
sha256: "81cd9ea6246f19217f0fbc46b52c8a6fc3d66333ed0b87dcc45a465a34ac2ce4"
---

To get a list of customers who have not made any purchases for a specified period of time, create a saved search for customers with no recent activity. You can use this search to identify customers you may want to contact.

Watch the following video for a tutorial on how to create a saved search for customers with no recent activity.

<a id="kaltura_player_44"></a>

#### To create a search for customers with no recent activity: {#procedure_N697166}

1.  Go to _Reports > Saved Searches > All Saved Searches > New_ and click **Customer**.
    
2.  Enter a title for the saved search.
    
3.  On the **Criteria** subtab, click **Summary**.
    
    1.  In the **Summary Type** field, select **Maximum**.
        
    2.  In the **Field** column, select **Activity Fields...**.
        
    3.  In the popup, select **Date**.
        
    4.  Select **not after**, and then **(Relative)**. On the next line, enter **1** and select **months ago**.
        
    5.  Click **Set**. This filter limits results to customers with no activity in the past month. You can enter a different relative time period to search for customers with no activity for a different period of time.
        
4.  On the **Results** subtab, click **Columns**.
    
    1.  Select **Name** from the list. In the **Summary Type** field, select **Group**.
        
    2.  Click **OK**.
        
    3.  Add a new column and select **Activity fields...**.
        
    4.  In the popup, select **Date**.
        
    5.  In the **Summary Type** column, select **Maximum**.
        
    6.  Click **Add**.
        
5.  Save the search.
    

### Related Topics

-   [Saved Search Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N691341.html)
-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
