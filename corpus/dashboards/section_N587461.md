---
id: "section_N587461"
type: "section"
title: "Creating Custom RSS/Atom Feeds"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Dashboards Overview > Setting Up Dashboard Portlet Content > RSS/Atom Feed Portlets > Creating Custom RSS/Atom Feeds"
parent: "section_N586341"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N587461.html"
anchors: ["procedure_N587481"]
sha256: "7027493d09a2031b57d527b27e7b5515beccbb450e04f691b6baa654609db83b"
---

You can create your own custom RSS/Atom feeds to publish information to users in dashboard portlets. In this case, the RSS/Atom Feed portlet shows links to HTML pages in the File Cabinet, with a short description for each page.

To create a custom feed, first make HTML documents with the information you want to link to from the RSS/Atom Feed portlet. Then, upload these files to the File Cabinet. Finally, create an RSS Feed record in NetSuite that lists links to your HTML files. This record also lets you define the audience for the file. The audience may include different roles, employees, customers, and more.

#### To create a custom RSS/Atom feed: {#procedure_N587481}

1.  Create HTML documents outside of NetSuite that you'll link to from the RSS/Atom Feed portlet.
    
2.  Go to _Documents > Files > File Cabinet_. Upload your HTML files.
    
3.  For each file, click **Edit** and copy the file's URL.
    
4.  Go to _Setup > Intranet > RSS Feeds_ or _Commerce > Site Builder > Marketing/Upsell > RSS Feeds_. Click **New**. The RSS Feed record stores the links and information to display in your custom RSS/Atom Feed portlet.
    
5.  In the **Title** field, enter a title for your feed. This title is displayed as the portlet title.
    
6.  In the **Alias** field, enter a name to describe this feed in the custom RSS Feeds list.
    
7.  In the **Description** field, enter a description for the feed.
    
8.  Check or clear the **Available Externally** box to define the audience for your feed:
    
    -   If you clear this box, the RSS feed is only for users with login access to your account, and you'll need to choose who can access it on the **Audience** subtab.
        
    -   If you check this box, all users will have access to this feed.
        
9.  On the **Items** subtab, add the titles, descriptions, and URLs for each of your HTML files.
    
    -   The **Title** appears as the link text in the RSS/Atom Feed portlet.
        
    -   The **Description** field contains details about what's on the linked HTML page.
        
    -   The **URL** field should contain the URL for the linked HTML file.
        
10.  When you've added titles, descriptions, and URLs for all your HTML files, click **Save**.
     

Now, users you've chosen as the audience can display the custom feed in an RSS/Atom Feed portlet on their dashboard. For information, see [RSS/Atom Feed Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N586341.html). If you are an administrator, you can publish your dashboard with this feed to users with other related roles. For information, see [Publishing Dashboards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N633149.html).

Note:

Currently, you can add only two RSS feeds each on the **Home** tab and **Issues** tab (if available). You can get around this limitation by creating a custom tab, where there is no limitation on the number of RSS feeds. For information, see [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html).

### Related Topics

-   [RSS/Atom Feed Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N586341.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
