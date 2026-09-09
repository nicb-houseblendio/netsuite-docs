---
id: "section_N2687230"
type: "section"
title: "Product Merchandising Overview"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Marketing > Storefront Merchandising Tools > Product Merchandising > Product Merchandising Overview"
parent: "section_N2687121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687230.html"
anchors: []
sha256: "69d34d88a565fe807a46a7253db1c510f291171cd57c5379d7ef077a24098306"
---

When using the Product Merchandising SuiteApp, a product merchandiser or marketing manager must work with a web developer to set up site templates with merchandising zones. After the initial setup is complete, these zones can be targeted with different content defined within merchandising rules without the need to rely on a developer for further customization.

Note:

Good initial planning in the types of merchandising zones required simplifies maintenance of sites and reduces the need for development costs.

The workflow for how a merchandising zone is implemented is as follows:

-   First, the product merchandiser works with a developer to define the selection criteria that would result in certain products to display. Selection criteria is based on available facets and sort options defined during the SuiteCommerce Advanced Web Site Setup.
    
-   The developer adds merchandising zones to website template files or creates new templates as needed to accommodate the desired display. These templates call the merchandising rule that initiates a query to the item search API, which then returns item data as requested by the rule.
    
    Note:
    
    If Content Delivery pages are used for the display of the Merchandising Rules, these pages must be defined after the Product Merchandising rules are defined. See [Content Delivery Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2688958.html) for details on using the Content Delivery SuiteApp.
    
-   The developer provides the product merchandiser with the Merchandising IDs to be used when setting up merchandising rules.
    
-   The product merchandiser defines the Product Merchandising rules based on the information used from the developer.
    

### Related Topics

-   [Create a Product Merchandising Rule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687488.html)
-   [Prepare Pages for Product Merchandising Zones](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687979.html)
-   [Storefront Merchandising Tools](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1531814631.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
