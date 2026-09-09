---
id: "bridgehead_N1087722"
type: "bridgehead"
title: "Performing a Mass Update on Customer Statuses"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Record Management > Lead Management > Performing a Mass Update on Customer Statuses"
parent: "section_N1086131"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1087722.html"
anchors: ["procedure_N1088350"]
sha256: "bab737869e011d7aee1be6bf36eb0bdf726f60e02b41059ad898707ef465b7e9"
---

With NetSuite you can find records that meet a specific criteria and update their fields values at the same time by doing a mass update. The mass update process requires the Mass Updates permission. For details, see [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html).

Administrators create customer statuses as part of the setup for the Sales Force Automation feature. For information, see [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html).

This topic includes a procedure for mass updates to convert existing leads to prospects without the Lead Conversion feature. The procedure also gives you an example you can use with the Lead Conversion feature.

#### To convert leads to prospects by mass update: {#procedure_N1088350}

1.  Go to _Lists > Mass Update > Mass Updates_.
    
2.  Under **Contact Management**, click **Change Customer Status**.
    
3.  (Optional)If you want to save the mass update for later, enter a name for the mass update in the **Title of Action** field on the Mass Update page.
    
4.  From the **Change Status To** list, select the prospect status you want the newly converted leads to have.
    
5.  Enter criteria to find the leads you want to convert as follows:
    
    1.  In the **Filter** column, select **Stage**, set the filter to **any of** and **Lead**, and then click **Add**.
        
    2.  (Optional) Add other filters to find leads that you want to convert.
        
        **Example:** You use the Lead Conversion feature for leads of the type Individual, but you want to use mass updates to convert leads of the type Company. To filter out leads of the type Individual, you add the **Is Individual** filter and set it to **No**.
        
6.  Click **Preview** to see a list of leads that will be converted to prospects.
    
7.  When you've reviewed the list, do one of the following:
    
    -   Click **Return To Criteria** to change the action name and adjust your filters.
        
        You can clear the box in the Apply column for specific leads you don't want to convert, but you'll need to adjust your filters to add to the list.
        
    -   (Optional) Click **Save** to save the action for future use.
        
        After you save, to return to the Mass Update Preview Results page, go to _Lists > Mass Update > Saved Mass Updates_ and click **Preview**.
        
    -   Click **Perform Update** to complete the conversion.
        

### Related Topics

-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Lead Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086363.html)
-   [Lead Conversion](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086628.html)
-   [Assigning Leads](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093032.html)
-   [Lead Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093883.html)
-   [Lead Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095188.html)
-   [Lead Conversion Reports, Search, and KPIs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095502.html)
-   [Setting Up Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1093237.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
