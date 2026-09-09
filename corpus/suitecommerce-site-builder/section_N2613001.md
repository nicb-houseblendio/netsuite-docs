---
id: "section_N2613001"
type: "section"
title: "Adding Multiple Items to the Shopping Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters > URL Parameters for Adding Items to the Cart > Adding Multiple Items to the Shopping Cart"
parent: "section_N2612472"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613001.html"
anchors: ["bridgehead_N2613029", "bridgehead_N2613060", "bridgehead_N2613089"]
sha256: "de1e64d03fd9d001933634555e1cc14223c0cb6e4fd191529eefefc1240299af"
---

You can add more than one item to the shopping cart in one request. First set the value of the **buyid** attribute to **'multi.'** Then add the item IDs and item quantities as values for the **multi** attribute.

## Adding Multiple Items to the Cart with a URL {#bridgehead_N2613029}

The sample URL below from account number 123456, adds one item (ID=51) with size and color options; and one of another item (ID=52) with different size and color options.

          `/app/site/backend/additemtocart.nl?c=123456&buyid=multi&multi=51,1,custcolsize|1|| custcolcolor|1;52,2,custcolsize|2||custcolcolor|2` 
        

You can use item ID and quantity, or item ID, quantity and options in a URL that adds multiple items to the shopping cart. Note the example of item options specified in the URL:

          `custcolsize|1||custcolcolor|1;` 
        

Note:

The vertical bar (|) separates option ID (custcolsize) from option value (1). The double vertical bar (||) separates option ID/value pairs from one another.

## Adding Multiple Items to the Cart Using HTML {#bridgehead_N2613060}

When you operate an external catalog site, use HTML to add multiple items to the shopping cart. The sample code below adds one each of item IDs 206, 207, 205 and 208 to the shopping cart.

For more information on internal IDs, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)

## Sample code snippet for adding multiple items to the shopping cart: {#bridgehead_N2613089}

          `<!-- START ITEM TEMPLATE --> <td> <!-- START MULTI ITEM ADD CODE --> <table border="0" cellpadding="0" cellspacing="0" width="100%"> <form method='post' action='http://www.wolfeelctronics.com/app/site/backend/additemtocart.nl'> <tr> <td> <p align="left"><input type="submit" value="Enter Store"></p> <input type='hidden' name='c' value='123456'> <input type=hidden name='qtyadd' value='1'> <input type=hidden name='buyid' value='multi'> <input type=hidden name='multi' value='206,1;207,1;205,1;208,1'> </td> </tr> </table> </form> <!-- END MULTI ITEM ADD CODE --> </td> <!-- END ITEM TEMPLATE -->` 
        

Note:

The code sample above also functions with the NetSuite shopping domain. Replace the URL in the <form> tag. For example: `<form method='post' action='http://shop.netsuite.com/app/site/backend/additemtocart.nl'>`

### Related Topics

-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html)
-   [Website URL Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
