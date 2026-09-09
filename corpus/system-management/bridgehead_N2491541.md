---
id: "bridgehead_N2491541"
type: "bridgehead"
title: "The URL Root and its Components"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SSP Applications > Create and Use SSP Applications > The URL Root and its Components"
parent: "section_N2491902"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2491541.html"
anchors: []
sha256: "dcb75dc7adecb681fdfbcefad3cff845679f35cf463c698dd0e2110e5b5977e8"
---

Every SSP application has an **application publisher** and an **application name**. The application name is the name of the folder where all SSP application assets are stored and is therefore also called the **SSP application folder**.

The application publisher is the creator of the SSP application. You can create multiple application publishers in your NetSuite account, but the names must be unique across all NetSuite accounts. The default application publisher setting is your NetSuite account name.

Note:

If you want to use SuiteCloud Development Framework (SDF) to create or edit SSP applications, you must use the SuiteApp application ID as the application publisher name. For information about SuiteApp application IDs, see [SuiteApp Application ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1509931104.html#subsect_1522775442).

The SSP application folder and its subfolders contain all the SSP application scripts, libraries, images, and other assets. Each SSP application in your NetSuite account has its own SSP application folder and the SSP Application folders are grouped according to their application publishers.

The **URL root**, or base URL, for an SSP application specifies the path that points to the location of SSP application assets. By default, the URL root includes the application publisher and application name. However, the base URL may include as many path components as desired. The ability to set the base URL yourself provides flexibility and readability.

Note:

The URL root can include letters, digits, hyphens (-), and underscores (\_). Any other characters are **forbidden** when setting the URL root.

NetSuite recommends that the base URL include at least one path component that distinguishes SSP application assets from other root assets in the domain. You must specify the URL root of the SSP application when you create the SSP application record.

Note:

For Aconcagua and later releases of SuiteCommerce and SuiteCommerce Advanced, make sure the URL root for each SSP application is unique. Using the same URL root for multiple SSP applications can cause confusion about which SSP application is handling requests. If for some reason you do specify the same URL root for more than one SSP application, remember that precedence plays a role in determining which SSP application is used first. For more information, see [Change SSP Application Precedence](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2496052.html).

For example, an SSP application named NextGenSite with an application publisher of SCA-NextGen, has the following default URL root: **/SCA-NextGen/NextGenSite/**. For testing purposes, you can access SSP application assets by navigating directly to the URL. For example, you can use the URL, **http://www.example.com/SCA-NextGen/NextGenSite/index.ssp**.

Note:

You must have the SuiteScript permission to access SSP application records.

You can either create an application publisher and an application folder when you create the SSP application record or you can create them in advance from the Web Site Hosting Files Folder in the file cabinet. For information on how to view and add an:

-   Application publisher - see [View and Add Application Publishers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494453.html)
    
-   Application folder - see [Create an SSP Application Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4343918704.html)
    

### Related Topics

-   [View and Add Application Publishers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2494453.html)
-   [Create an SSP Application Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4343918704.html)
-   [SuiteScript 1.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529595280.html)
-   [SuiteScript 2.0 SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529598062.html)
-   [Create and Use SSP Applications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2491902.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
