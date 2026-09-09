---
id: "section_N2603891"
type: "section"
title: "Creating and Editing Site Themes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Creating and Editing Site Themes"
parent: "section_N2603624"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603891.html"
anchors: ["subsect_1554930072", "procedure_N2603959", "bridgehead_N2604236", "bridgehead_N2604358", "procedure_N2604442", "procedure_N2605981"]
sha256: "0f965da0ab22d1e87ab6beb30bb37ead2452331597ba3b49558b8b5684871e8a"
---

Customize and edit site themes from the Web Site Themes page on the Setup tab. You can edit the default site theme, or customize one of the basic site themes. After creating a custom site theme, it is displayed on the list, and you can go back to edit the custom site theme you created.

To customize or edit a site theme, first go to _Commerce > Site Builder > Appearance > Themes_.

To view a chart of NetSuite website tags, see [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html) and [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html).

## General Guidelines for Using SuiteScript in Site Builder Themes {#subsect_1554930072}

Customizations must not overwrite existing event listeners. Where a custom event listener is needed, it should be added to the event rather than replace existing listeners. Note the following examples:

Preferred:

            `window.addEventListener('load', function () { alert('load triggered'); });` 
          

Avoid:

            `window.onload = function () { alert('load triggered'); };` 
          

#### General subtab {#procedure_N2603959}

1.  In the **Page cellpadding** field, enter a value for the amount of space you want to appear outside the tables in your HTML.
    
    For example, to include no space between your tables, enter **0**.
    
2.  In the **Color Theme** field, select the color background scheme to use for this theme. You can override this theme by selecting a theme on the Set Up Web Site page.
    
    You can create your own color theme at _Commerce > Site Builder > Appearance > Color Themes > New_.
    
3.  In the **Site Font** field, select the default font to use for text in your site.
    
4.  In the field named **Addition to <head>**, enter any HTML you want to appear in the <head> section of your website.
    
    This section is useful for referencing script files, defining scripts your pages need or adding a message in the title of your window.
    
5.  In the **<body> tag attributes** field, you can control the attributes of the page <body> tag.
    
    For example, you can control the page background color, default text color, link color and margin width. Enter customized values to override the default values for the <body> tag of your site. Leave this field empty to use default body tag attributes.
    
    Use the following as an example for this field:
    
                    `bgcolor='#FFFFFF' link='#000000' vlink='#000000' alink='#000000' text='#000000'` 
                  
    
6.  In the **Default Item Drilldown Template** field, select the item/category template that should be used to display item detail pages.
    
    The item detail page is displayed when a site visitor clicks on an item on your website to see more information. You can override this default by selecting templates for individual items on item records.
    
    For more information about item templates, see [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).
    
    Note:
    
    Selecting a default item template on the Set Up Web Site page overrides this setting.
    
7.  In the **Default Info Item Drilldown Template** field, Select the item/category template that should be used to display information item detail pages.
    
    Your HTML template is applied when a site visitor clicks the name of the information item from a list to view more details. You can override this default by selecting templates on individual information item records.
    
    Note:
    
    Selecting a default information item template on the Set Up Web Site page overrides this setting.
    
8.  In the **Default Item List Layout** field, select the default layout for lists of items in your site. You can set list layouts on individual categories and tabs to override this default.
    
    For more information on layouts and list templates, see [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html) and [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html).
    
    Note:
    
    The Item List Layout set on the parent Tab overrides the setting on the Set Up Web Site page.
    
9.  In the **Default Category List Layout** field, select the default layout for lists of categories or subcategories in your site. You can set list layouts on individual categories and tabs to override this default.
    
    Note:
    
    Selecting a default category list layout on the Set Up Web Site page overrides this setting.
    
10.  In the **Default Related Items Layout** field, Select the default layout for lists of related items in your site. You can set list layouts on individual categories and tabs to override this default.
     
     Note:
     
     Selecting a default related items list layout on the Set Up Web Site page overrides this setting.
     
11.  In the **Welcome Page Item List Layout** field, select the list layout you want to use for items on your Welcome tab.
     
     Create new layouts at _Commerce > Site Builder > Appearance > Layouts > New_.
     

#### Body subtab {#bridgehead_N2604236}

1.  In the **Logo and Tabs Template** field, enter the HTML that defines the top of the page, including your logo and tab bar.
    
    This example displays your logo, the Register and Log In links, the tab bar and the code that recognizes a customer that has logged in or prompts a returning customer to Log In. Replace **YOUR LOGO URL** with the URL of the image you use for your logo.
    
                    `<tr>       <td>          <table width="100%" border=0>             <tr>                <td align="left"><img src="https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/YOUR%20LOGO%20URL" border=0>                </td>                <NLPAGELINKS>             </tr>          </table>          <br>          <table border=0 cellspacing=0 cellpadding=0>             <tr><NLPAGETABS>             </tr>          </table>          <table border=0 cellspacing=0 cellpadding=0 width=100%>             <tr>                <td align="right"><NLUSERINFO>                </td>             </tr>          </table>       </td>    </tr>` 
                  
    
2.  In the **Content Area Template** field, you can customize the central content area where your categories and items are displayed. This example inserts lists of items available on the tab you are viewing.
    
                    `<td valign="top" width="100%">       <table width="100%">          <NLCOLUMNCONTENTS>       </table>    </td>` 
                  
    
3.  In the **Left Sidebar Width** field, enter a width in pixels for the size of the left column in your website.
    
4.  In the **Left Side Navigation Template** field, enter HTML for the table on the left side navigation of all pages. For example, you can enter the following:
    
                    `<td valign="top" width="<NLSIDEBARWIDTH>">       <table>          <NLCOLUMNCONTENTS>       </table>    </td>` 
                  
    
5.  In the **Right Sidebar Width** field, enter a width in pixels for the size of the right column in your website.
    
6.  In the **Right Side Navigation Template** field, enter HTML for the table on the right side navigation column on the Home page, and My Account tab on your web store. For example, you can enter the following:
    
                    `<td valign="top" width="<NLSIDEBARWIDTH>">       <table>          <NLCOLUMNCONTENTS>       </table>    </td>` 
                  
    
7.  In the **Footer Template** field, you can customize the footer of your site pages. This example places a copyright statement in the footer.
    

          `<table border="0" cellspacing="0" cellpadding="0" width="100%">       <tr>          <td align='right'>             Copyright © 2004 Your Company Name.          </td>       </tr>    </table>` 
        

#### Tabs and Buttons {#bridgehead_N2604358}

1.  In the **Active Tab Template** and **Inactive Tab Template** fields, you define how the active tab (the tab a customer is viewing) and the inactive tabs appear. If you create an active tab template, you must also create an inactive tab template.
    
    This example creates a tab bar with a dark blue active tab and light blue inactive tabs. The color of the text on the tabs in defined by the color theme selected on your website record at _Commerce > Websites > Website List_.
    
    **Active Tab Template** :
    
                    `<td width="2"></td>    <td bgcolor="darkblue">          <a href='<NLTABLINKURL>' <NLTABLINKATTRIBS>>       <NLTABLABEL></a>   </td>    <td width="2"></td>` 
                  
    
    **Inactive Tab Template** :
    
                    `<td width="2"></td>    <td bgcolor="lightblue">   <a href='<NLTABLINKURL>'        <NLTABLINKATTRIBS>><NLTABLABEL></a>       </td>    <td width="2"></td>` 
                  
    
2.  In the **Add to Cart Button** field, you can customize the button that customers click if they want to buy an item. This example creates a button with text 'Buy Now!'.
    
                    `<NLADDTOCARTOPTIONS>    <tr align='left'>       <td width='1%'>          <NLADDTOCARTITEMID><NLADDTOCARTQUANTITY>       </td>       <td>          <INPUT type='button' value='Buy Now!'                   name='addtocart'          onkeypress="window.event.cancelBubble=true;"          onclick="<NLADDTOCARTCLICKSCRIPT>">       </td>    </tr>` 
                  
    
3.  In the **Add to Cart Button on Dense Lists** field, you can customize the button that customers click if they want to buy an item. This example creates a button with text 'Buy Now!'.
    

          `<NLADDTOCARTOPTIONS>    <tr align='left'>       <td width='1%'>          <NLADDTOCARTITEMID><NLADDTOCARTQUANTITY>       </td>       <td>          <INPUT type='button' value='Buy Now!'              name='addtocart' onkeypress="window.event.cancelBubble=true;"        onclick="<NLADDTOCARTCLICKSCRIPT>">       </td>    </tr>` 
        

#### Sidebars subtab {#procedure_N2604442}

1.  In the **Default Portlet Template field**, enter the HTML to define the framing around any portlets displayed on your site that you do not define in step 2 below.
    
    This HTML must start with <td> and end with </td>. For example, you can enter the following:
    
                    `<td>       <table width="<NLSIDEBARWIDTH>">          <tr>             <td><NLPORTLETTITLE>             </td>          </tr>          <tr><NLPORTLETCONTENTS>          </tr>       </table>    </td>` 
                  
    
2.  Using the same format as the Default Portlet Template, enter HTML between <td> and </td> tags for the following portlets:
    
    -   Cart Summary
        
    -   Currency Selector
        
    -   Language Selector
        
    -   Search
        
    -   Search Form
        
    -   Site Navigation
        
    
    To apply these templates, you must set these portlets to display on your website record at _Commerce > Websites > Website List_.
    
3.  In the **Navigation Show Top-level Links** field, choose the type of menu you want to display in your navigation portlet:
    
    -   **All Tabs** - Shows contents of all tabs
        
    -   **Current Tab** - Shows contents of the tab being viewed
        
    -   **Categories** - Shows contents of the category being viewed
        
    
    To use this preference you must enable the Show Navigation Portlet preference on the Set Up Web Site page.
    
    The contents in the site navigation list depend on your decision to show items or categories in the navigation portlet.
    
4.  Check the **Navigation Show Subcategories** box to show subcategories in the navigation menu portlet.
    
    -   If you select **All Tabs** as your top level navigation, subcategories under all tabs are shown.
        
    -   If you select **Current Tab** as your top level, subcategories of the tab being viewed are shown.
        
    -   If you select **Categories** as your top level, subcategories of the category being viewed are shown.
        
5.  Check the **Navigation Show Items** box to show item links in your navigation menu portlet.
    
    You must check the Show Navigation Portlet box on the Set Up Web Site page to use this preference.
    
    -   If you select **All Tabs** as the top-level navigation, item links are shown for all tabs.
        
    -   If you select **Current Tab** as the top level, item links are shown for the items on the tab being viewed.
        
    -   If you select **Categories** as the top level, item links are shown for the items in the category being viewed.
        

#### Misc subtab {#procedure_N2605981}

1.  For each of the following, you can enter custom HTML or select an image for the different kinds of bullets in your website:
    
    -   **Bullets** - This replaces the bullets next to login links or any bullets that are not part of a hierarchical list.
        
    -   **Item Bullets** - This replaces the bullets next to items in the left-column, navigational portlet.
        
    -   **Open Category Bullets** - This replaces the bullets next to categories that are open and showing subcategories or items in the left-column, navigational portlet.
        
    -   **Closed Category Bullets** - This replaces the bullets next to categories that are not open in the left-column, navigational portlet.
        
2.  In the **Separator HTML** field, enter the HTML you would like to appear between items in item lists.
    
    Note:
    
    Separator HTML only appears when you are viewing pages with layouts where the Show Separators Between Items box is checked.
    

You can override your site theme's appearance (color theme, tab style, portlet style, etc.) based on appearance settings on your website record at _Commerce > Websites > Website List_.

To further control your site, you can create custom HTML tags. These tags will be replaced based on your default settings and tag substitution definitions. This lets you customize your page templates to look different when individual tabs of your site are viewed.

To enter custom tag definitions, go to _Commerce > Site Builder > Content > Tags > New_, enter your custom tags. When you have finished, click Save.

### Related Topics

-   [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html)
-   [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html)
-   [Adding a Style Sheet to Your Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2608851.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html)
-   [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
