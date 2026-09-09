---
id: "section_N2625840"
type: "section"
title: "Site Attributes"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Creating Attribute Tags > Creating Attribute Tags for Standard Records > Site Attributes"
parent: "section_N2616966"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2625840.html"
anchors: []
sha256: "d223d56b833326da5189ebb3c626468d03fc4b5614300125f600aa6b1bacc44d"
---

You can create attribute tags for elements of the site that do not exist on NetSuite records, such as the URL for the home page. For example:

          `<%=getCurrentAttribute('site','homepageurl')%>` 
        

| Site Properties | Attribute | Notes |
| --- | --- | --- |
| Consent to accept website cookies | cookieconsenthtml | Displays a black banner at the top of your website with a link to read your website cookies policy. |
| Copyright | copyrighthtml | Displays the copyright message with © symbol, year, and store display name |
| Display name of the store | name | Returns the display name from the Site Setup page. |
| Home page URL | homepageurl |  |
| HTML to publish the entire page | storepagehtml |  |
| Logo alignment | logoalignment | Returns left, right or center alignment. |
| Logo image | logoimagehtml |  |
| Logo image URL | logoimageurl | Returns the URL for use in an <img> tag. |
| Logo image link | logolinkurl |  |
| Tab name currently being viewed | currenttablabel |  |
| Welcome page image | welcomeimagehtml |  |
| Welcome page image/flash URL | welcomeimageurl | Returns URL for use in an <img> tag. |
| Related items list title | relateditemsdescription | Returns the contents in the Related Items field on the Upsell subtab of the website record (_Commerce > Websites > Website List_. |
| Upsell items list title | upsellitemsdescription | Returns the contents in the Upsell field on the Upsell subtab of the website record (_Commerce > Websites > Website List_). |

### Related Topics

-   [Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2617271.html)
-   [Information Item Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2620223.html)
-   [Color Theme Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622110.html)
-   [Category Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2622893.html)
-   [Customer Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2623719.html)
-   [Request Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627019.html)
-   [Checkout Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627341.html)
-   [Order Confirmation Attributes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2627572.html)
-   [Creating Attribute Tags for Standard Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2616966.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
