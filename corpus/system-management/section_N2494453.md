---
id: "section_N2494453"
type: "section"
title: "View and Add Application Publishers"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > The URL Root and its Components > View and Add Application Publishers"
parent: "bridgehead_N2491541"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494453.html"
anchors: []
sha256: "701346e59aa42a1ff0bd486123b9a2fbff0f908880de5f52873dda5d9b35fd9e"
---

To view a list of application publishers, go to Setup > Company > Application Publishers (Admin).

#### To create a new application publisher

1.  Go to Setup > Company > Application Publishers (Admin).
    
2.  Click **New Application Publisher**.
    
3.  Enter a **Name** for the application publisher.
    
    Important:
    
    An application publisher must be unique across all NetSuite accounts. If you enter a name that is already in use, an error is displayed. Also, if you want to use SuiteCloud Development Framework (SDF) to create or edit SSP applications, you must use the SuiteApp application ID as the application publisher name. For information about SuiteApp application IDs, see [SuiteApp Application ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1509931104.html#subsect_1522775442).
    
4.  Click **Save**.
    

The application publisher appears as a component in the URL root that points to the SSP application and all its assets. The SSP application folder path includes a subfolder named for the application publisher and a subfolder with the application name. (The default can be edited.)

The SSP application folder path has a format like the following:

**<HTML Hosting Root>: /SSP Applications/<Application Publisher>/<Application Name>**

### Related Topics

-   [Create an SSP Application Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4343918704.html)
-   [The URL Root and its Components](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2491541.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
