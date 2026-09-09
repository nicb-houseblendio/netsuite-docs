---
id: "section_N2599702"
type: "section"
title: "Example for Building a Combination Site"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Website Hosting with Site Builder > Example for Building a Combination Site"
parent: "chapter_N2598224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599702.html"
anchors: ["bridgehead_N2599835", "procedure_N2599848", "bridgehead_N2599954", "procedure_N2599967", "bridgehead_N2600182", "bridgehead_N2600224", "bridgehead_N2600266", "bridgehead_N2600291"]
sha256: "462492a87e167a6b0b89d56ed90fa152fefafc4de3035ea4ae60263588816a76"
---

This section offers sample HTML and GIF files for a site that mixes a hosted home page with NetSuite tabs, shopping cart and checkout. You can experiment with this example to best serve your needs.

Click [here](https://system.netsuite.com/core/media/media.nl?id=2034678&c=NLCORP&h=175661f5a9d8dba82a67&_xt=.zip) to download a ZIP file that includes the sample home page and images. When the dialog opens, choose Save, and then save the media file as **NetSuite\_examples.zip** in a location where you can find it again.

Follow the steps below to start using the sample files:

1.  [Add the Sample Files to the File Cabinet](#bridgehead_N2599835)
    
2.  [Set Preferences for the Sample Web Store](#bridgehead_N2599954)
    
3.  [Create a Tab for Your Website](#bridgehead_N2600182)
    
4.  [Create a Category for Your Website](#bridgehead_N2600224)
    
5.  [Create an Item Record to Publish on Your Website](#bridgehead_N2600266)
    

## Add the Sample Files to the File Cabinet {#bridgehead_N2599835}

Because you will display these files in your web store, you must upload them in the Web Site Hosting Files folder in the NetSuite file cabinet.

#### To upload website files in the file cabinet: {#procedure_N2599848}

1.  Go to _Commerce > Hosting > Website Hosting Files_.
    
2.  Click the **Live Hosting Files** folder.
    
3.  Click the **Site** folder.
    
4.  At the bottom of the page, click **Advanced Add**.
    
5.  In the **Zip Archive to Add** field, click **Browse**.
    
6.  Select the **NetSuite\_examples.zip** file from your hard drive, and click **Open**.
    
7.  Check the **Make All Files Available Without Login** box.
    
8.  Click **Add**. All files are automatically unzipped in the site folder.
    
9.  Click **Edit** next to **logo\_wolfe\_electronics.gif**.
    
10.  In the **Folder** field, select **Images**.
     
11.  Click **Save**.
     

Next, set preferences for your site including the hosted home page.

## Set Preferences for the Sample Web Store {#bridgehead_N2599954}

Set preferences to determine how your site appears and interacts with your NetSuite account. In the steps below, you will set the look and feel of your site by choosing a color theme, logo, and site theme.

#### To set web store preferences: {#procedure_N2599967}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next the website name.
    
3.  On the **Setup** subtab, in the **Web Site Home Page Type** field, choose **Hosted Web Page**.
    
4.  In the **Web Site Home Page** field, choose **Live Hosting Files : /site/index.html**.
    
5.  Click the **Appearance** subtab.
    
6.  In the **Web Site Color Theme** field, you can choose your own company colors or choose **\-From Theme-** to use the color theme provided with the site theme.
    
7.  In the **Web Site Logo** field, choose **logo\_wolfe\_electronics**.
    
8.  In the **Web Site Logo Alignment** field, choose **Left**.
    
9.  In the **Web Site Theme** field, select one of the Basic site themes.
    
    If you use the Advanced Site Customization feature, you can customize the templates for these themes or use them as guides to make your own at _Commerce > Site Builder > Appearance > Themes_. For more information, see [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html).
    
10.  In each of the **Drilldown Template** and the **Layout** fields, choose **\-From Theme-** to use the templates associated with the site theme you selected in Step 8. You can mix and match site templates by selecting different templates for Drilldown and Layout.
     
     The Advanced Site Customization feature is required to customize the basic item/category templates or to create your own. For more information on creating item/category templates, see _Commerce > Site Builder > Appearance > Item/Category Templates_.
     
11.  Click **Save**.
     

For more information on the other optional settings on the Site Builder Web Site Setup page, see [Site Builder Web Site Record Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2561820.html).

Next, create a website tab and a category for your site.

## Create a Tab for Your Website {#bridgehead_N2600182}

To create a Web site Tab, go to _Commerce > Site Builder > Content Management > Tabs_.

You will use tabs as the pages of your web store, to organize and display categories of similar items and information. You can also use a hosted tab to display an HTML page or link to a different website. For more information, see [Creating Website Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2595492.html).

After creating a tab for your website, you can create a category and display it on a tab.

## Create a Category for Your Website {#bridgehead_N2600224}

To create categories for your site, go to _Commerce > Site Builder > Content Management > Categories_.

Categories organize the items you sell in your web store. On the Web Site subtab of item records, you select the category where you want to display the item. To learn more about setting up categories, see [Creating Site Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2596427.html).

After you have created a category, and assigned it to the tab you created, next create an item record.

## Create an Item Record to Publish on Your Website {#bridgehead_N2600266}

You can create item records of virtually any type for display on your website. Note that to display an item in your web store, it must have a value for price, it must be assigned to a category, and the Display in Web Site box must be checked. For more information, see [Setting Up Items for the Web Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585301.html#section_N2177433).

Your web store is now ready to preview.

## Preview Your Website {#bridgehead_N2600291}

To preview your website, go to _Commerce > Websites > Preview Website_. Click Preview Site. Your site opens in a new window.

The website home page displays the sample hosted HTML page you uploaded in the file cabinet. The other tabs display categories and items you have set up in your account. The Shopping Cart, Checkout and My Account tabs display by default in all NetSuite websites. You can choose not to display any tab in your website by clearing the Display in Web Site box.

Note:

If you choose to build your website with HTML pages, you can use Attribute tags in the HTML to display items and categories. For more information, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html). You can also use attribute tags to display information from category and item records in site templates. For more information, see [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html).

### Related Topics

-   [Hosting HTML Websites with NetSuite Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598355.html)
-   [Audience Permissions for Hosted Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2598904.html)
-   [Website Staging Environment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2599525.html)
-   [External Catalog Site (WSDK) Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2600392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
