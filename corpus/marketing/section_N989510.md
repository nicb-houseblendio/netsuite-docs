---
id: "section_N989510"
type: "section"
title: "Sales Campaigns"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Managing Campaigns > Sales Campaigns"
parent: "chapter_N985526"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N989510.html"
anchors: ["bridgehead_N989696", "bridgehead_N989782", "bridgehead_N989809", "bridgehead_N989902", "bridgehead_N989992"]
sha256: "89b904e77a9afda2eea930932b6e71a6a8cc7a94beecba3519e1efe44caea716"
---

Sales campaigns enable your sales reps to send email campaigns to their customers and track the responses. Sales campaigns enable reps to better assess their customers' interest.

Sales reps can use campaign response reports to view each recipient's response. This helps reps identify interested customers.

When reps use sales campaigns to send offers, they know which recipients opened or clicked a link in the email. Reps can view the Campaign Responses Detail report to see each recipient and their response. Reps can use this information to determine which prospects to follow up with.

Note:

NetSuite tracks recipient response data only for links to NetSuite pages. For example, NetSuite tracks a link to a page in your NetSuite website, but not a link to a third-party site.

Reps can send sales campaigns to the customers, contacts, and other records that the sales rep's role gives them permission to view or edit.

Note:

You can edit a sales campaign only when you are logged in with the role you used to create the campaign. The role in which you created a sales campaign displays in the Manager Role field on the sales campaign. Only the manager of a sales campaign can edit it.

You can create sales campaigns at _Lists > Marketing > Sales Campaigns > New_.

To view a list of sales campaigns, go to _Lists > Marketing > Sales Campaigns_.

By default, sales campaigns do not appear in the list at _Lists > Marketing > Marketing Campaigns_. However, you can create a custom list view to include sales campaigns. To do this, edit the view of the marketing campaign list, and set the Is Sales Campaign filter to Either. The sales campaign list can't show marketing campaigns.

Note:

NetSuite does not send sales campaigns for inactive campaign owners (sales reps no longer with your company).

For information about email marketing campaigns, see [Creating an Email Marketing Campaign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1002625.html).

## Giving Access to Sales Campaigns {#bridgehead_N989696}

To grant access to sales campaigns, an administrator must enable the Sales Campaigns feature at Setup > Company > Enable Features > CRM. The Sales Campaigns feature grants the standard sales roles (Sales Person, Sales Manager, and Sales Administrator) access to the following:

-   the Sales Campaign page and search
    
-   marketing templates
    
-   CRM groups
    
-   marketing reports
    

Sales reps conduct sales campaigns in a manner similar to marketing user who conducts marketing campaigns.

## Target Group Restrictions {#bridgehead_N989782}

Sales reps can send sales campaigns only to customers and contacts that meet the restrictions defined by their assigned role. A sales rep restricted to the customers assigned to themselves and their subordinates can send sales campaigns to only those customers.

## Sales Campaign Templates {#bridgehead_N989809}

Marketing templates permit NetSuite to automatically track the response to sales campaign email.

Sales campaigns use the sender's information for the From and Reply To email addresses. The nickname and From address entered in the sales rep's profile (Home > Set Preferences > General subtab) define these email addresses.

Note:

NetSuite does not use marketing email addresses in the From Email Address and Reply To Email Address fields (campaign email template) in email sent through sales campaigns. The exception to this is when someone sends a campaign on behalf of a sales rep. For example, if a sales manager sent a campaign on behalf of their subordinates. Sales campaigns created with a marketing template marked to Email as Sales Rep uses the sales rep's email address as the From and Reply To addresses. For more information, see [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).

If a sales rep hasn't set up a profile, NetSuite uses the rep's login email address as the email's From address. NetSuite uses the name on the sales rep's employee record in the To field on the email.

## Sales Campaign Reports and Search {#bridgehead_N989902}

Marketing campaign reports include data on both sales campaigns and marketing campaigns, by default. If you have access to both kinds of campaigns, your campaign reports include both sales and marketing campaign data.

To filter the report results to display only one kind of campaign, customize the report and add the Is Sales Campaign filter. Set this filter to True to view only sales campaigns. Set the filter to False to view only marketing campaigns.

![A custom report with the Is Sales Campaign filter set to True to view only sales campaigns.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/salesCampaigns_addIsSalesCamp_filter.png)

To view campaigns for a specific sales rep, customize the report and add the Campaign Manager filter.

NetSuite returns only sales campaigns when you search at _Lists > Marketing > Sales Campaigns > Search_. NetSuite returns marketing campaigns and sales campaigns when you search at _Lists > Marketing > Marketing Campaigns > Search_. To limit the results of this search to display only marketing campaigns, set the Is Sales Campaign filter to False.

## Tracking the Success of Your Sales Campaigns {#bridgehead_N989992}

You can track the responses of your sales campaigns on the sales campaign record. The Statistics subtab gives an overview of how your campaigns were received and responded to. For more information about campaign responses, see [Tracking Campaign Responses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990539.html).

For details about how your customers responded to your campaigns, view the [Campaign Response Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1012922.html). Go to Reports > Marketing > Campaign Response > Detail Report. This report lists the campaign recipients and how they responded, which provide understanding into which customers have interest in your offer.

For more information, see [Marketing Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1010316.html).

### Related Topics

-   [Creating a Campaign Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986170.html)
-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)
-   [Marketing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1017620.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
