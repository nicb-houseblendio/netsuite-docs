---
id: "section_N2591207"
type: "section"
title: "Search Forms"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Items, Forms, & Images > Publishing Forms > Search Forms"
parent: "section_N2590699"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591207.html"
anchors: ["procedure_N2591291", "procedure_N2591424"]
sha256: "8ffdd0ccf254c8ba6f8ffee3730d7d049244035d06871ed196c63fffe02250eb"
---

A search form lets you create a custom search that is displayed in your website or intranet site. Customers can select their own search criteria, and the search results show in a list on the site.

For example, when Wolfe Electronics publishes an item search to the Catalog page of its website, customers can search for items by their name or price.

To publish a search form on your website, you must first create a saved search for use with the search form. Then create the search form on the Publish Form page in NetSuite.

After you have created the search form, apply a custom layout template to present the items in the search results with a look and feel consistent with the rest of your site. For more information, see [Applying Layout Templates to Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635640.html).

You can also use the search form as the default search in your website. Go to _Commerce > Websites > Website List_ and click **Edit** next to the website name. On the Search subtab, select the name of the search form for either **Search Link Form, Search Portlet Form**, or both. Click Save. For more information, see [Web Site Search Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2572319.html).

Note:

You can create a search form and display it as a portlet on your NetSuite-generated web pages. To display a search form on hosted pages use Web Site Tags. For more information, see [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html).

#### To create a saved search for use with a search form: {#procedure_N2591291}

1.  Go to _Lists > Search > Saved Searches > New_.
    
2.  Select a type of record for the search.
    
    For example, if this search is for items available on your website, choose **Item**.
    
3.  Enter a name for this search in the **Search Title** field. This title is not seen by your customers.
    
4.  Check the **Public** box to make the search available to use on a Search Form.
    
5.  On the **Criteria** subtab, select criteria to **Filter** the items displayed in the search results.
    
    For example, if this search is for items available on your website, choose the filter, Display in Web Site, then select Yes. Only items that are marked to display online are included in the search results.
    
6.  On the **Results** subtab, select the columns you want to show in the search results.
    
    In the example above, Wolfe Electronics shows Name, Description, and Online Price.
    
    Important:
    
    In the Custom Label column, you can change the names of the columns in the search results.
    
7.  Click **Add**.
    
8.  (Required) On the **Available Filters** subtab, choose the criteria your customers can select when using the search form on your site.
    
    Note:
    
    Only searches with Available Filters appear in the list of Saved Searches available to be published. Also, when creating a saved search to publish as a search portlet on your website, keep the number of available filters at a minimum to prevent slow performance.
    
    For example, customers on the Wolfe Electronics website can search by Name and Online Customer Price.
    
9.  Click **Add**.
    
10.  Click **Save**.
     

Next, create a search form to publish to a tab or category in your website.

#### To create the search form: {#procedure_N2591424}

1.  Go to _Commerce > Site Builder > Content Management > Publish Forms > New_.
    
2.  Click **Search Form**.
    
3.  In the **Name** field, enter a title for this search form. Customers can see this title.
    
    For example, if this is a custom search that will appear with your Specials category, you could enter **Search Our Specials**.
    
4.  In the **Saved Search** field, select the search this form is based on.
    
5.  Check the **Disallow Drilldown** box if you do not want customers to click on the link to each item in the search results to see the item page.
    
6.  Check the **Display in Web Site** box, so that the search form appears on your site.
    
7.  The fields on the Basic subtab are optional.
    
    -   Enter any descriptions you want to appear with this search form in the **Brief Form Description** and **Detailed Form Description** fields.
        
    -   The **Featured Description** appears below the store display name on the Home page of your site. Enter a description here, if you plan to publish the form to the Home page of your site.
        
    -   In the **Search Keywords** field, enter alternative search keywords that customers might use to find this search form using your web store's internal search.
        
    -   Check the **Exclude form Sitemap** box to exclude the search form from the Sitemap.
        
    -   **Sitemap Priority** is used for the Sitemap Generator. NetSuite uses the value you set here when you generate the Sitemap.
        
8.  At the bottom of the page, in the **Site Category** column, choose one or more categories where you want this search form to appear.
    
    Also, choose the **Site** in which the search form should appear.
    
9.  On the **Media** subtab, choose a thumbnail image to appear with this search form in lists.
    
    For more information, see [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html).
    
10.  If you use the Multi-Language feature, see [Working With Multi-Language Names and Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2178279.html) for more information about using the **Translations** subtab.
     
11.  Click **Save**.
     

Your search form is now available in the categories you chose in Step 8 above.

### Related Topics

-   [Email Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591004.html)
-   [Case and Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html)
-   [File Download with Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592134.html)
-   [Publishing Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2590699.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
