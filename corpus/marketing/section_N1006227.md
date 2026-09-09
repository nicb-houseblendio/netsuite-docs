---
id: "section_N1006227"
type: "section"
title: "Submitting Your Paid Search Proposal"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Keyword Campaigns > Submitting Your Paid Search Proposal"
parent: "chapter_N1004769"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1006227.html"
anchors: ["bridgehead_N1006287", "bridgehead_N1006326"]
sha256: "8cd86ec09b1249f8384308b8b0466ba63ae19f135baa200cff6390c99a9696e6"
---

With the Advanced Web Reports feature, when a customer finds your site through a search engine, NetSuite captures that customer's keyword campaign information. This lets you track revenue and lead generation for your paid keywords.

To make this information available on the lead or customer record, you should do the following:

-   Have an administrator enable the Advanced Web Reports feature at _Setup > Company > Setup Tasks > Enable Features_. Create campaign records for each keyword you purchase.
    
-   Provide a URL with the proper lead source parameter when you register a keyword with a paid keyword service.
    

## Formatting Destination URLs {#bridgehead_N1006287}

When you register keywords with a paid search service, give the landing page URL that customers see when they click your site in search results.

You should format the landing page URL as follows so that NetSuite associates the correct keyword campaign with the customer record:

          `http://yourlandingpage.com?leadsource=yourcampaignID` 
        

When you enter a keyword campaign record in NetSuite, you only enter the URL for the landing page. When you save it, NetSuite adds the lead source parameter and campaign ID to the URL.

You can copy and paste this URL from the record when you register the keyword with the search engine You can also export this URL into a spreadsheet. For more information, see [Exporting Keywords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1006031.html).

When a lead clicks the link to your site, NetSuite saves the lead source in the cookie from your website. NetSuite keeps this information no matter how many times the lead leaves your site and returns. When the lead registers with your website, or submits an online customer form, NetSuite saves the lead source to the record.

## Managing Cost-Per-Click {#bridgehead_N1006326}

Many paid search services don't charge up front, but get paid each time someone clicks your search result. You can calculate ROI anytime by updating a campaign's total cost with the cost you incurred for a certain time period.

### Related Topics

-   [Creating Keyword Campaigns in Bulk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1005080.html)
-   [Importing Keyword Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1005411.html)
-   [Creating a Campaign Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986170.html)
-   [Exporting Keywords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1006031.html)
-   [Tracking Campaign Revenue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990329.html)
-   [Associating a Customer With a Campaign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N991789.html)
-   [Associating a Transaction With a Campaign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N991927.html)
-   [Tracking Campaign Lead Generation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N992223.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
