---
id: "section_N2635180"
type: "section"
title: "Publishing Saved Search Results on Your Website"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Website Search with Site Builder > Publishing Saved Search Results on Your Website"
parent: "chapter_N2634719"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635180.html"
anchors: ["procedure_N2635210", "procedure_N2635338"]
sha256: "c6bf5923f02de4c23de5911247d39af7332f6e50b76a2e4553600b5defdd456c"
---

Create a saved search for items that might appeal to certain interests, and publish the saved search on your web store. When shoppers click a link, they can see the search results on your site.

For example, the Wolfe Electronics website has a saved search for cordless phones. This search updated on a regular basis, so the list is up to date.

To publish the search results on your website, you need to enable the Website feature first.

#### To enable the Website feature:

1.  Go to _Setup > Company > Enabled Features_.
    
2.  Under the **Web Presence** tab, check the **Website** box.
    
3.  Click **Save**.
    

#### To create a saved search for use with a Published Saved Search: {#procedure_N2635210}

1.  Go to _Lists > Search > Saved Searches_.
    
2.  Click **New**.
    
3.  Click **Item**.
    
4.  Enter a name for this search in the **Search Title** field. This title is not seen by your customers.
    
5.  Check the **Available for Publishing on a Website** box to make the search available to use on a Search Form.
    
6.  On the **Criteria** subtab, select criteria to filter the records displayed in the search results.
    
    For example, if this search is for items available on your website, choose the filter, Display in Web Site, then select Yes. Only items that are marked to display online are included in the search results.
    
    Important:
    
    Use these criteria to restrict search results, such as transaction records, from displaying on your website to all customers.
    
7.  On the **Results** subtab, select the columns you want to show in the search results. For example, use: Name, Description, and Online Price.
    
    Note:
    
    In the **Custom Label** column, you can change the names of the columns in the search results.
    
8.  Click **Add**.
    
9.  Click **Save**.
    

Next, publish this saved search to your web store. Customers will be able to view an up-to-date list of items. Note that only search forms allow customers to change the criteria of a search. For more information, see [Search Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591207.html).

#### To publish the search results: {#procedure_N2635338}

1.  Go to _Commerce > Site Builder > Content Management > Publish Saved Search > New_.
    
2.  Enter a title for the link shoppers click to view your search results.
    
3.  In the **Search** field, select the name of the search you created.
    
4.  In the **Subcategory of** field, choose the page in your site where you want to display the link to your search results.
    
5.  In the Item List Layout field, you can select a layout created at _Commerce > Site Builder > Appearance > Layouts_. Choose an option in the list to customize the look of your search results.
    
6.  Check the **Display in Web Site** box.
    
7.  On the **Basic** and **Media** subtabs, enter descriptions and choose images to appear next to the link for this **Published Saved Search**.
    
8.  On the **Audience** subtab, you have the option of displaying search results only to registered customers who log in instead of all site visitors.
    
    To publish only to specific customers or to registered customers who log in, first clear the Display in Web Site box. Then, on the Audience subtab, choose from the following:
    
    -   To display these results to all registered customers when they log in, check **Select All** next to Customers.
        
    -   To publish to specific customers, select customer names in the **Customers** field.
        
    -   To publish to a group of customers, select the group name in the **Groups** field.
        
        To create groups of customers using search criteria, go to _Contacts > Contacts > Groups > New_. Select Dynamic or Static based on the type of group you want to create.
        
9.  Click **Save**.
    

Shoppers in your web store can now click the link to your published saved search and see the list of search results.

You can also apply a layout template to the published saved search. This lets you better merchandise your items by presenting them in a list that has a look and feel consistent with the rest of your website. For more information, see [Applying Layout Templates to Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635640.html).

Note:

Published saved search results are updated every four hours at the database level, adding or removing content, to meet the criteria for the search. Consequently, changes in the saved search results may not display immediately on the web store.

By default, all items marked Display in Web Site can be returned in web search results, even if they are not assigned to a tab or category in the website. To only have items assigned to tabs or categories appear in search results, go to _Commerce > Websites > Website List_ and click Edit next to your website name. Clear the Show Items Not in Categories in Search Results box.

Warning:

CSV Import of Published Saved Searches is not supported.

### Related Topics

-   [Helping Customers Find Items on Your Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2634841.html)
-   [Setting Up Alternate Search Keywords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635042.html)
-   [Applying Layout Templates to Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2635640.html)
-   [Creating and Publishing an Employee Directory for a Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N916548.html)
-   [Website Search with Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2634719.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
