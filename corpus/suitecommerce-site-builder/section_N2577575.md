---
id: "section_N2577575"
type: "section"
title: "Registration-Free Shopping"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Customizing Registration for Your Site Builder Web Store > Registration-Free Shopping"
parent: "section_N2576937"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577575.html"
anchors: ["procedure_N2577602"]
sha256: "73a6e47704478237a7cff959148568f68021dfc317df3cfd5f44b58db80ddb5c"
---

You can allow customers to shop and purchase items in your web store without having to create a login and password.

When a customer purchases items without creating a login and password, a customer record is created using the information provided during checkout. Each time the customer returns and purchases items, a new customer record is created. If you do not use Auto-generated numbers, a number is added to the end of the customer name for each additional customer record created.

You can use the Duplicate Detection feature to merge duplicate records that may result from registration-free shopping.

#### To allow registration-free shopping: {#procedure_N2577602}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to your website.
    
3.  Click the **Shopping** subtab.
    
4.  In the **Type of Customer Registration** field, select **optional**.
    
5.  Click **Save**.
    

Customers can now shop in your store without entering registration information. A new customer record is created each time a shopper submits an order in your web store. Any duplicate customer records appear in the list of customers with a number appended to the name. For example, if Jane Smith already exists as a customer in the system, the next customer who places an order with the same name displays in NetSuite as Jane Smith 2.

You can manage duplicate records by enabling the feature, Duplicate Detection & Merge from _Setup > Company > Setup Tasks > Enable Features_ > Company. After that feature is enabled, you can periodically run the duplicate merge operation from the Search menu.

Note:

Customers who choose not to register will not have a My Account tab and therefore cannot download items, check order status or make payments from your site. They will need to enter personal information every time they purchase from your store.

### Related Topics

-   [Secure Login Access to Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577046.html)
-   [Displaying Login Fields on Your Web Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577156.html)
-   [Customizing Login and Logout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577359.html)
-   [Restricting Access to Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2577753.html)
-   [Customizing the Website Registration Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2578016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
