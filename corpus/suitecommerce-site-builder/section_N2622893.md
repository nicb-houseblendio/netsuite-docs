---
id: "section_N2622893"
type: "section"
title: "Category Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Category Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html"
anchors: []
sha256: "593cb2adf642b9a52fbbd2c41467a924da244ccdac8cd6c70ef468a0d9fc0350"
---

The following table includes the eligible fields for the category record type and the corresponding attribute to use in your tag. Attributes are not case-sensitive. For example, you could use the Attribute tag to expose the canonical URL for a particular category:

          `<%=getAttribute('sitecategory',7,'canonicalurl')%>` 
        

| **Field Name** | **Attribute** | Notes |
| --- | --- | --- |
| Canonical URL | canonicalurl |  |
| Category Image | categorythumbnailhtml | Returns the image at the size you set for Category Thumbnails on the Image Resizing Page. |
| Detailed Description | storedetaileddescription |  |
| Inactive | 
isinactive

binactive (information item)



 |  |
| Internal ID | internalid |  |
| Item/Category Display Image | storedisplayimagehtml |  |
| Item/Category Display Image (returns URL only) | storedisplayimage |  |
| Item/Category Display Thumbnail | storedisplaythumbnailhtml storeDisplayThumbnailHtml-URL | Use **storeDisplayThumbnailHtml-URL** to access the URL of the image file. |
| Item/Category Display Thumbnail (returns URL only)' | storedisplaythumbnail |  |
| Item Name/Number | itemid | Returns the value in the Category field on category records. |
| Search Keywords | searchkeywords |  |
| URL Component | urlcomponent |  |
| Description | description |  |
| Description (Opt 2) | description2 | If the Category Description is empty, this attribute returns the value for Category Name. |
| Meta Tag HTML | metataghtml |  |
| Page Title | pagetitle |  |
| Parent Category | parentcategory |  |
| store page | storepagehtml | HTML to for the entire page |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Site Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
