---
id: "section_N1019075"
type: "section"
title: "Campaign Offers"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Setting Up Marketing > Campaign Offers"
parent: "chapter_N1017289"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1019075.html"
anchors: []
sha256: "e88325a9d08abdf8afb3e1e3cb16260fbbc17744b7982650cb5f26af72dc755c"
---

Use campaign offers to group marketing campaigns by assigning each one to a specific offer. Campaign offers let you create reports that provide the combined revenue or activity of a group, rather than individual campaign performance. Only users with the Marketing Administrator or Administrator role can create campaign offers. You can assign only one campaign offer to a marketing campaign.

#### To create a Campaign Offer:

1.  Go to _Setup > Sales & Marketing Automation > Campaign Offers > New_
    
2.  Enter a name for the offer.
    
3.  Enter a short description. This appears on the list page of campaign offers.
    
4.  Click **Save**.
    

To assign an offer to a particular marketing campaign, go to _Lists > Marketing > Marketing Campaigns_. Open the campaign record in edit mode and select the offer from the Offer list in the Related Information section.

## Using Campaign Offers to Track Multiple Campaign Revenues

Wolfe Electronics run several marketing campaigns throughout the year that qualify for financial support from the manufacturers they promote. Wolfe uses campaign offers to track the results of these campaigns so they can claim a rebate from the manufacturer. They create a transaction saved search that groups together campaign revenues that are associated with a particular campaign offer.

#### To create a grouped campaign offer transaction search:

1.  Go to _Reports > New Search > Transaction_.
    
2.  Click the **Results** subtab.
    
3.  From the **Field** list, select **Lead Source Fields...**.
    
4.  From the **Lead Source Field** list, select **Offer**.
    
5.  In the **Summary Type** column, select **Group**, and click **Add**.
    
6.  In the **Summary Type** column, select **Amount (Gross)** and summary type, **Sum**. Click **Add**.
    
    These selections give you a consolidated revenue for each campaign offer.
    
7.  Click the **Create Saved Search** button.
    
8.  Enter **Campaign Offer Consolidated Revenue** in the **Search Title** field.
    
9.  Click **Preview** to test the results of your newly created search.
    
10.  Click **Return to Criteria**.
     
11.  Set any search visibility options, for example **Public**.
     
12.  Click **Save**.
     

The newly created search generates a report similar to the following:

![An example of a Campaign Offer Consolodated Revenue: Results report.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/Campaign_Offer_consolidated_rev_rep_example.png)

### Related Topics

-   [Creating a Campaign Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986170.html)
-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)
-   [Marketing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1017620.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
