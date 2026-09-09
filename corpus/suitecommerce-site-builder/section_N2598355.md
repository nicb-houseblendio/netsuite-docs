---
id: "section_N2598355"
type: "section"
title: "Hosting HTML Websites with NetSuite Site Builder"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Website Hosting with Site Builder > Hosting HTML Websites with NetSuite Site Builder"
parent: "chapter_N2598224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598355.html"
anchors: ["procedure_N2598479", "bridgehead_N2598698", "procedure_N2598719"]
sha256: "836f4451486bd388cda9c2e1e8c5bece07acd22c40e70774425f988b4afdc686"
---

With the Host HTML Files feature, you can host a custom HTML website in the NetSuite file cabinet. Use the Advanced Web Reports feature to track site visitors and determine the most popular pages on your website. For more information, see [Hosted Page Hits by Customer Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2647049.html).

To enable the Host HTML Files and the Advanced Web Reports features, go to Setup > Company > Enable Features. Click the Web Presence subtab, and then check the boxes next to the features you want to use.

If you want to run your site as a web store, use NetSuite website tags to integrate your site with NetSuite web store checkout by adding links to the shopping cart and registration pages in your custom HTML. For more information, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html).

You can also use tags to display items from your NetSuite account in your hosted HTML website. Note, however, that tags are not substituted in hosted files greater than 2 MB in size. For more information, see [Using Web Site Tags in Hosted Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616592.html).

Note:

NetSuite supports the use of client-side JavaScript in hosted pages; however, server-side scripts are not currently supported.

NetSuite also supports audience permissions on hosted sites. This lets you restrict intranet sites and hosted tabs on your website for specific users, roles, or groups. For more information, see [Audience Permissions for Hosted Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598904.html).

#### To host your custom HTML site with NetSuite: {#procedure_N2598479}

1.  Go to _Commerce > Hosting > Website Hosting Files_.
    
2.  Select the folder where you want to upload your site files.
    
    -   To publish your site on the web, use the **Live Hosting Files** folder.
        
    -   For more information about staging your hosted site before publishing it to your online customers, see [Website Staging Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599525.html).
        
    -   To move an existing HTML site to NetSuite, see [Moving an HTML Website to NetSuite](#bridgehead_N2598698).
        
    
    Note:
    
    If you name a hosting folder or file the same name as a default NetSuite folder or file, you may lose images or HTML from NetSuite basic site themes.
    
3.  Select the folder where you want to store your site, and then click **New Folder** to create subfolders. For example, you may want to create a subfolder for images.
    
4.  Upload files from your computer to you new folder.
    
    -   Click **Add File** to add individual files.
        
    -   Click **Advanced Add** to add multiple files in a .zip file. Check the Unzip files box to automatically unzip files when they are uploaded to the file cabinet.
        
5.  When you have added all of your site files and folders, go to _Commerce > Websites > Website List_.
    
6.  Click **Edit** next the name of the website.
    
7.  On the **Setup** subtab, in the **Default Hosting Root** field, select the top level folder in the file cabinet where your site is stored.
    
8.  In the **Web Site Home Page Type** field, select **Hosted Web Page**.
    
9.  In the **Web Site Home Page** field, select the file name of your home page.
    
10.  Click **Save**.
     

Now, when customers visit your NetSuite website, they see only your custom HTML website. If you need to edit an HTML file, make changes to the file on your computer, and then upload the modified file to the file cabinet. To preserve links and references to the file, do not change the file name.

For more information about setting up a domain name for your website, see [Domain Setup Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1521794882.html#section_1521797541).

For more information about optimizing your site for search engines, see [Site Builder Search Engine Optimization (SEO)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2635817.html).

## Moving an HTML Website to NetSuite {#bridgehead_N2598698}

If you are moving an existing HTML site to NetSuite, you may want to create a new hosting folder in the Web Site Hosting Files folder to keep your site structure and links intact.

#### To recreate the structure of an existing HTML website in NetSuite: {#procedure_N2598719}

1.  Go to _Commerce > Hosting > Website Hosting Files_.
    
2.  Click **New Folder** to create a new hosting folder based on the structure of your existing HTML website.
    
    You can create a new folder on the same level as the Live Hosting Files folder or create a subfolder in the Live Hosting Files folder. Your approach depends on how you want to structure your website. Later, you will select the folder you create as the Default Hosting Root for your website.
    
3.  Create subfolders as needed and add files. For more information about uploading files, see [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html).
    
4.  Go to _Commerce > Websites > Website List_
    
    If you use multiple websites, click **Edit** next to the site you want to modify, or click **New** to create a new website.
    
5.  On the **Setup** subtab, in the **Web Site Home Page Type** field, select **Hosted Web Page**.
    
6.  In the **Web Site Home Page** field, select the file name of your home page.
    
7.  In the **Default Hosting Root** field, select the top-level folder in the file cabinet where your site is stored. This is the folder you created in Step 2.
    
8.  Click **Save**.
    

To preview your site, go to _Commerce > Websites > Preview Website_. Click Preview Site.

### Related Topics

-   [Audience Permissions for Hosted Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598904.html)
-   [Creating an HTML Intranet Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599141.html)
-   [Displaying an HTML Site in a NetSuite Tab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599309.html)
-   [Website Staging Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599525.html)
-   [External Catalog Site (WSDK) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
