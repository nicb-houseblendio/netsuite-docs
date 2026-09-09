---
id: "section_N659760"
type: "section"
title: "Summary Type Example Screenshots"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining an Advanced Search > Summary Types for Search Results > Summary Type Example Screenshots"
parent: "section_N659258"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659760.html"
anchors: ["bridgehead_N659810", "bridgehead_N659877", "bridgehead_N660000", "bridgehead_N660086", "bridgehead_N660208", "bridgehead_N660304", "bridgehead_N660396"]
sha256: "010f2da57671866cae4e5e9744a3fae68cb3c9f6f86a6612bfb98957e8124512"
---

The sections below guide you through setting up criteria and results, including summary types, for a sales order transaction search. Screenshots show the definitions and results pages for each summary type.

#### To create a search and define search criteria: {#bridgehead_N659810}

1.  Go to _Reports > Saved Searches > All Saved Searches_ > New and select **Transaction**.
    
2.  Select **Type** from the **Filter** field and Sales Order in the popup window. Then click **Set**.
    
3.  Select Main Line from the **Filter** field and No in the popup window. Then click **Set**.
    
    ![Filter field to define search criteria.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/salesorder1.png)

#### To define a Group summary type: {#bridgehead_N659877}

1.  Click the **Results** subtab and add the following fields: **Amount**, **Name**, **Date**.
    
2.  Select Group from the Summary Type dropdown list for Name, to group transactions by Customer.
    
    ![Group summary type selected for the Name field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/salesorder2.png)
3.  Click the **Preview** button. The first level of results lists customers.
    
    ![Search preview results.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/customer4.png)
4.  Click a customer name to drill down into a list of transactions for that customer.
    
    ![Customer drill down.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/customer5.png)

#### To define a Sum summary type: {#bridgehead_N660000}

1.  Click **Return to Summary**, then click **Return to Criteria**.
    
2.  Click the **Results** subtab and select Sum from the Summary Type dropdown list for Amount.
    
    ![Sum summary type selected for the Amount field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results2.png)
3.  Click **Preview**. The results page shows the total amount of transactions for each customer.
    
    ![Preview of custom search results.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results3.png)

#### To define a Count summary type: {#bridgehead_N660086}

1.  Click **Return to Criteria**.
    
2.  Click the **Results** subtab, add the Item field, and select Count from the Summary Type for Item. Also, remove the Sum from Amount, by selecting a blank from the Summary Type dropdown list.
    
    ![Count summary type selected for the Item field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/columns1.png)
3.  Click **Preview**. The results page shows how many items were sold for each customer.
    
    ![Preview of Custom Transaction search results.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results4.png)
4.  Click a customer to drill down to a list of transactions and items.
    
    ![Drill down of Custom Transaction search results.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results5.png)

#### To define a Minimum summary type: {#bridgehead_N660208}

1.  Click **Return to Summary**, then click **Return to Criteria**.
    
2.  Click the **Results** subtab, remove the **Item** field, and select **Minimum** from the Summary Type dropdown list for **Amount**.
    
    ![Mnimum summary type selected for the Amount field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/columns2.png)
3.  Click **Preview**. The results page shows the minimum transaction amount for each customer.
    
    ![Custom Transaction search results with a minimum summary type.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results6.png)

#### To define a Maximum summary type: {#bridgehead_N660304}

1.  Click **Return to Criteria**.
    
2.  Click the **Results** subtab, and select **Maximum** from the Summary Type dropdown list for **Amount**.
    
    ![Maximum summary type selected for the Amount field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results7.png)
3.  Click **Preview**. The results page shows the maximum transaction amount for each customer.
    
    ![Custom Transaction search results with a maximum summary type.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results8.png)

#### To define an Average summary type: {#bridgehead_N660396}

1.  Click **Return to Criteria**.
    
2.  Click the **Results** subtab, and select **Average** from the Summary Type dropdown list for **Amount**.
    
    ![Average summary type selected for the Amount field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results9.png)
3.  Click **Preview**. The results page shows the average transaction amount for each customer.
    
    ![Custom Transaction search results with an average summary type.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/results10.png)

### Related Topics

-   [Summary Types for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659258.html)
-   [Summary Type Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N659383.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
