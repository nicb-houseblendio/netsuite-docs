---
id: "section_N2607165"
type: "section"
title: "Sample HTML for Item/Category Templates"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Advanced Site Customization > Item and Category Templates > Sample HTML for Item/Category Templates"
parent: "section_N2606158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607165.html"
anchors: ["bridgehead_N2607274", "bridgehead_N2607291", "bridgehead_N2607307", "bridgehead_N2607324", "bridgehead_N2607341", "bridgehead_N2607358"]
sha256: "b44424e2ee0f0f2edcbfb3eabd0a6454e0d924626347d8abf960c8c296931857"
---

Use the HTML code samples provided below to create a set of item/category templates for your website:

-   [Example of a Category List Template](#bridgehead_N2607274)
    
-   [Example of an Item List Template](#bridgehead_N2607291)
    
-   [Example of a Category in a List](#bridgehead_N2607307)
    
-   [Example of an Item in a List](#bridgehead_N2607324)
    
-   [Example of an Item Page](#bridgehead_N2607341)
    
-   [Example of an Information Item Page](#bridgehead_N2607358)
    

## Example of a Category List Template {#bridgehead_N2607274}

This example displays the name, description, and image for the category being viewed and lists its subcategories below. List templates must include the <NLITEMLIST> tag to display the list of subcategories.

          `<td width='100%'> <table width=100%> <tr> <td colspan=2 align='center'> <h1> <%=getCurrentAttribute('sitecategory','itemid')%> </h1> <%=getCurrentAttribute('sitecategory','storedetaileddescription')%> <br> <br> <img src='<%=getCurrentAttribute('sitecategory','storedisplaythumbnail')%>' border=0> </td> </tr> <tr> <NLITEMLIST> </tr> </table> </td>` 
        

## Example of an Item List Template {#bridgehead_N2607291}

This example lists the category name before listing the items in the category. List template must include the <NLITEMLIST> tag to display the list of items in a category.

          `<td width='100%'> <table width=100%> <tr> <td> <h1> <%=getCurrentAttribute('sitecategory','itemid')%> Items </h1> </td> </tr> <tr> <NLITEMLIST> </tr> </table> </td>` 
        

## Example of a Category in a List {#bridgehead_N2607307}

This example is a category cell template for categories in a list. The category name, description, and image are included in the list, and the name and image act as links to go to the category page.

          `<td> <h2> <a href='<%=getCurrentAttribute('sitecategory','storeURL')%>'> <%=getCurrentAttribute('sitecategory','itemID')%></a> </h2> <%=getCurrentAttribute('sitecategory','storeDetailedDescription')%> <br><br> <a href='<%=getCurrentAttribute('sitecategory','storeURL')%>'> <img src='<%=getCurrentAttribute('sitecategory','storeDisplayThumbnail')%>' border=0></a> </td>` 
        

## Example of an Item in a List {#bridgehead_N2607324}

This example is an item cell template for items in a list. The item name, stock status, description, price, weight, image, and related items are displayed along with an Add to Cart button. The item name and image act as links to the item page.

          `<td> <h2> <a href='<%=getCurrentAttribute('item','storeURL')%>'> <%=getCurrentAttribute('item','itemID')%> <%=getCurrentAttribute('item','stockStatusMessageHTML')%></a> </h2> <!--%=getCurrentAttribute('item','salesPrice')%><br>--> Only <%=getCurrentAttribute('item','salesPriceHTML')%> <br><br> <table> <%=getCurrentAttribute('item','addToCartListHTML')%> </table> <a href='<%=getCurrentAttribute('item','storeURL')%>'> <%=getCurrentAttribute('item','storeDisplayImageHTML')%></a> </td>` 
        

## Example of an Item Page {#bridgehead_N2607341}

This example is for an item drilldown page that shows when a visitor clicks the name of an item to view details. This example includes the item's name, detailed description, price, weight, and full size image with an Add to Cart button.

          `<td> <h2> <%=getCurrentAttribute('item','itemID')%> </h2><br> <%=getCurrentAttribute('item','storeDetailedDescription')%> <br><br> <h3> <!--%=getCurrentAttribute('item','salesPrice')%> <br>--> Only <%=getCurrentAttribute('item','salesPriceHTML')%> </h3> Weight <%=getCurrentAttribute('item','weight')%> <br><br> <%=getCurrentAttribute('item','storeDisplayImageHTML')%> <table> <%=getCurrentAttribute('item','addToCartHTML')%> </table><br> <table> <tr> <%=getCurrentAttribute('item','relatedItemsHTML')%> </tr> </table> </td>` 
        

## Example of an Information Item Page {#bridgehead_N2607358}

This example is for a text and image information item page that shows when a visitor clicks the name of the information item. This example includes the information item title, brief description, full size image and detailed description.

          `<td> <h2> <%=getCurrentAttribute('infoitem','itemID')%> </h2> <br> <%=getCurrentAttribute('infoitem','storeDescription')%> <br> <%=getCurrentAttribute('infoitem','storeDisplayImageHTML')%> <br> <%=getCurrentAttribute('infoitem','storeDetailedDescription')%> </td>` 
        

### Related Topics

-   [Creating Item/Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606465.html)
-   [Applying Templates to Lists of Categories and Lists of Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606825.html)
-   [Placing Multiple Images in an Item/Category Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2607454.html)
-   [Item and Category Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2606158.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
