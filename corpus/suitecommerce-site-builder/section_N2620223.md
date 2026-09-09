---
id: "section_N2620223"
type: "section"
title: "Information Item Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Information Item Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html"
anchors: []
sha256: "3453e898d6adc8c0677d8da0b8a612a01c746fad7e3c26511487dea58f438beb"
---

The following table includes the eligible fields for the information item record type and the corresponding attribute to use in your tag. Attributes are not case-sensitive. For example, the Attribute tag below would show the value in the Store Detailed Description field on an information item record.

          `<%=getCurrentAttribute('infoitem','storedetaileddescription')%>` 
        

| **Field Name** | **Attribute** | Notes |
| --- | --- | --- |
| Detailed Description | storedetaileddescription |  |
| Display in Site | isonline |  |
| Featured Description | featureddescription |  |
| Featured Item | bfeat |  |
| Featured Item (Opt 2) | welcomedescription | If the Featured Description is empty, this attribute returns the value in the Store Description field. |
| Inactive | binactive |  |
| Internal ID | internalid |  |
| Item/Category Display Image | storedisplayimagehtml |  |
| Item/Category Display Image (returns URL only) | storedisplayimage |  |
| Item/Category Display Thumbnail | storedisplaythumbnailhtml storeDisplayThumbnailHtml-URL | Use **storeDisplayThumbnailHtml-URL** to access the URL of the image file. |
| Item/Category Display Thumbnail | storedisplaythumbnail | Returns only the URL for the thumbnail image. |
| Item Name/Number | itemid | Returns the value in the Name field on information items. |
| Search Keywords | searchkeywords |  |
| Store Description | storedescription |  |
| Subsidiary | subsidiary |  |
| URL Component | urlcomponent |  |
| Meta Tag HTML | metataghtml |  |
| Page Title | pagetitle |  |
| Store page | storepagehtml | Returns HTML to publish the entire page. |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
