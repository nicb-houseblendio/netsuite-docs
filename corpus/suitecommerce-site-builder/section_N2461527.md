---
id: "section_N2461527"
type: "section"
title: "Best Practices for Website Performance"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Best Practices for Website Performance"
parent: "chapter_N2576231"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2461527.html"
anchors: []
sha256: "f4b2ac030fe3902e1852b163d734edbe4305cd1bdcb242c54b0ec3e476a7c01a"
---

This topic describes ways in which you can improve performance on your website and create pages that load quickly.

-   **Limit the number of items displayed on a page to 25 items or fewer.**
    
    Restrict the number of rows and columns on the page layout. NetSuite imposes a limit of 50 items per page, but pages with 25 or fewer items load faster.
    
    For more information about creating layouts for your website pages, see [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html).
    
-   **Avoid hosted pages that display more than 25 items.**
    
    Because hosted pages use Web Site Tags to display items, NetSuite is unable to limit the number of items on hosted pages. You can create performance problems by making hosted HTML pages that display hundreds of items.
    
-   **Display no more than 250 items in your web store categories.**
    
    NetSuite generates a warning when you add more than 1000 items to a category. Items beyond the 1000th are displayed on pages in your web store, but performance on your site will be degraded. If you have categories with thousands of items, consider breaking those up into smaller categories.
    
-   **Avoid using an excessive number of tabs.**
    
    Having more than 20-50 tabs on your site, even if published to different people, can cause performance problems. Avoid the practice of creating a tab published to each one of your users.
    
-   **Whenever possible, use categories and tabs to organize items on your website instead of published saved searches.**
    
    Public saved search pages do not perform as well as pages with lists of items that you define, especially searches with complex search criteria. For that reason, published search results pages are cached for up to 4 hours so the underlying search does not run more than one time every 4 hours despite potentially heavy page demand.
    
-   **Reuse JavaScript if you create custom site theme templates for your website.** Rework scripts in cell templates to share code.
    
-   **Simplify your JavaScript code**.
    
    For example, note that the code sample below is reused elsewhere in the website, so only one copy is needed.
    
                  `<script language="JavaScript" type="text/javascript"> function checkForSpecialDisplay(itemName, itemID, itemBlockString) {         if ( (( itemName== "" )  && ( itemID== ""))  ||  ( itemName.indexOf('Error') == 1 )  ) {               // undesirable item leave span off - do nothing           }           else {               // show span               document.getElementById(itemBlockString).style.display = "";           } } </script>` 
                
    
    This is the code sample that will be repeated for each item on page.
    

          `<script language="JavaScript" type="text/javascript">         checkForSpecialDisplay(<%=getCurrentAttribute('item','storeDisplayName')%>, <%=getCurrentAttribute('infoitem', 'itemid')%>, item-block<%=getCurrentAttribute('item', 'internalid')%>); </script>` 
        

### Related Topics

-   [Site Builder Web Site Content Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576424.html)
-   [Previewing Your Site Builder Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2576788.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
