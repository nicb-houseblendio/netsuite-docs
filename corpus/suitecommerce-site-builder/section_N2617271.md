---
id: "section_N2617271"
type: "section"
title: "Item Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Item Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html"
anchors: []
sha256: "41ef294beb9e2d563a6fcdba351259319e6a60c4bfcf1ec5923bd2d0df65b5c2"
---

The following table includes the eligible fields for the item record type and the corresponding attribute to use in your tag. Attributes are not case-sensitive. For example, use the attribute tag below, to show a list of upsell items on your site.

          `<%=getCurrentAttribute('item','correlateditemshtml')%>` 
        

| **Field Name** | **Attribute** | Notes |
| --- | --- | --- |
| Available To Adv. Partners | availabletopartners |  |
| Canonical URL | canonicalurl |  |
| Class | class |  |
| Correlated Items | correlateditemshtml | Returns the list of automated upsell items. |
| Department | department |  |
| Detailed Description | storedetaileddescription |  |
| Display in Site | isonline |  |
| Display Name/Code | displayname |  |
| Drop Ship Item | isdropshipitem |  |
| Featured Description | featureddescription |  |
| Featured Item | isfeatured | See also [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html). Note: This attribute is different from the **Featured Item** attribute for information items. |
| Featured Item (Opt 2) | welcomedescription | If the Featured Description field is empty, this attribute returns the value in the Store Description field. |
| Handling Cost | handlingcost |  |
| Inactive | isinactive | See also [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html). Note: This attribute is different from the **Inactive** attribute for information items. |
| Internal ID | internalid |  |
| Item/Category Display Image | storedisplayimagehtml |  |
| Item/Category Display Image | storedisplayimage | Returns the URL only. |
| Item/Category Display Thumbnail | storedisplaythumbnailhtml storeDisplayThumbnailHtml-URL | Use **storeDisplayThumbnailHtml-URL** to access the URL of the image file. |
| Item/Category Display Thumbnail | storedisplaythumbnail | Returns the URL for use in an <img> tag. |
| Related Item Thumbnail Image | relateditemthumbnailhtml | Returns the image at the size you set for Related Item Thumbnails on Image Resizing page (_Commerce > Site Builder > Content > Image Resizing_). |
| Featured Item Thumbnail Image | featureditemthumbnailhtml | Returns the image at the size you set for Featured Item Thumbnails on Image Resizing page (_Commerce > Site Builder > Content > Image Resizing_). |
| Item Options | denselistitemoptionshtml | Returns HTML for the item options select list in a dense list format. |
| Item Name/Number | itemid |  |
| Item Weight | weight |  |
| Item Weight Unit | weightunit | Shows the unit of measure for item weight, such as lb, oz, kg, or g. |
| Lead Time | leadtime storeleadtime | Both attributes return the value for lead time from the Inventory subtab. |
| Location | location |  |
| Manufacturer | manufacturer |  |
| Maximum Variable Amount | maxdonationamount |  |
| Minimum Quantity | minimumquantity |  |
| Offer Support | offersupport |  |
| On Special | onspecial |  |
| Online Price | salespricehtml |  |
| Online Price | salespricelisthtml | Returns HTML for how it appears on an item list page. |
| 
Online Price

(For dense list layout)



 | denselistsalespricehtml | Returns HTML for how it appears on a dense list layout. |
| Price Level | pricelevel pricelevel1, pricelevel2, etc. | Use **pricelevel** to return the price for the customer who is logged in. For more information, see [Displaying Price Levels and Sale Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2608509.html). |
| Quantity Available | quantityavailable |  |
| Quantity On Hand | quantityonhand |  |
| Related Items | relateditemshtml | Returns the items you add to the Related Items subtab of Item records. Note: For upsell items, see 'Correlated Items' at the beginning of this table. |
| Related Items Description | relateditemsdescription | Returns contents in the Related Items Description field on the item record. |
| Related Item Name | relateditemsdescription2 | Returns the contents in the Related Items Description field on the item record if present. If the field on the item record is blank, then this attribute defaults to the item's name. |
| Related items description | relateditemsdescription3 | Returns the contents in the Related Items Description field on the item record if present. If the field on the item record is blank, then this attribute defaults to the value in the Related Items field on the Upsell subtab at _Commerce > Websites > Website List_. |
| Sale Unit | saleunit |  |
| Sales Description | salesdescription |  |
| Search Keywords | searchkeywords |  |
| Shipping Cost | shippingcost |  |
| Special Order Item | isspecialorderitem |  |
| Specials Description | specialsdescription |  |
| Stock Description | stockdescription |  |
| Store Description | storedescription |  |
| Store Display Name | storedisplayname |  |
| Store Display Name | storedisplaynamehtml | Displays as a link to the item detail page or as a link shoppers can use to transfer data in the case of a download item hosted in the file cabinet. |
| Subsidiary | subsidiary |  |
| Type | type | Defines the type of the item in use on the website. For example: an item for sale, or an information item. |
| Units Type | unitstype |  |
| URL Component | urlcomponent |  |
| Varialble Amount | isdonationitem |  |
| Vendor Name/Code | vendorname |  |
| **Attributes for Elements not Available on the Item Record** |
| Add to Cart button with item name | addtocartitemid | Lists the item name on the Add to Cart button. |
| Add to Cart button | addtocarthtml | 

Returns HTML for the Add to Cart button. Use between <table> and

</table> tags.



 |
| Quantity field | addtocartquantityhtml | Returns HTML for the quantity field as it appears with the Add to Cart button. |
| 

Add to Cart button

(Item detail page)



 | addtocartdrilldownhtml | Returns HTML for the Add To Cart button as it appears on an item detail page. |
| 

Add to Cart button

(Item list page)



 | addtocartlisthtml | Returns HTML for the Add To Cart button as it appears on an item list page. |
| 

Add to Cart button

(Dense list layout)



 | denselistaddtocartbuttonhtml | Returns HTML for the Add To Cart button as it appears in dense lists. |
| 

Add to Cart quantity

(Dense list layout)



 | denselistaddtocartquantityhtml | Returns HTML for the quantity field as it appears with the Add to Cart button on dense lists. |
| Add to Cart button with options | addtocartoptionshtml |  |
| HTML to publish the entire page | storepagehtml |  |
| Out of Stock message | stockstatusmessagehtml | See the note below. |
| 'Tell A Friend' link | tellafriendlinkhtml |  |
| Upsell related items together with item you add to the Related Items subtab on item records. | allrelateditemshtml |  |
| URL Address of the item referenced | storeurl |  |

Note:

To include the stock status message with an Add to Cart button, you must use the stock status message attribute in a tag that appears before the attribute tag for the add to cart button. For example:

          `<%=getCurrentAttribute('item','stockstatusmessagehtml')%><%=getCurrentAttribute('item', 'addtocartdrilldownhtml')` 
        

### Related Topics

-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
