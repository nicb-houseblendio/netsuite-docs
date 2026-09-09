---
id: "section_N2468468"
type: "section"
title: "Managing Website Customers in OneWorld with Site Builder"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Setting Up Your Site Builder Site > Site Builder and OneWorld > Managing Website Customers in OneWorld with Site Builder"
parent: "section_N2466850"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2468468.html"
anchors: ["bridgehead_4484810213"]
sha256: "c2fcd8a19010bc1103bc68ebc42843edb8c254f27f80df5fd43081831e9f84be"
---

Visitors to your website can use a list displayed on your Site Builder site to select the subsidiary information they want to view. After the visitor selects a subsidiary, that subsidiary is assigned to the customer record created after an order is submitted. If the visitor does not submit an order but signs up on your website, the subsidiary is assigned to the lead record created in NetSuite.

Customers returning to your website are automatically directed to the subsidiary on the customer record and the list of subsidiaries is not displayed in the site. An administrator can only reset the subsidiary on the customer record in NetSuite if no transactions have occurred.

## Setting the Default Customer Role {#bridgehead_4484810213}

New customers registering on your website are assigned a default customer role that you specify. In a OneWorld account, the corresponding subsidiary must be defined on the default customer role. If the subsidiary is not defined on the default customer role, then information such as shipping options may not be available to the customer.

#### To define a subsidiary on the default customer role:

1.  Go to _Setup > Company > General Preferences_.
    
2.  Find the **Default Role for New Customers** field. Remember the role selected here.
    
3.  Go to _Setup > Users/Roles > Manage Roles_.
    
4.  On the list of roles, find the role that is selected as the default role for new customers from Step 2. Click the link to view the values in the **Subsidiaries** list. All subsidiaries that have web stores should be selected. You can click **Customize** to update the role.
    
    Note:
    
    To complete this task, you need an administrator role, or permission to modify users and roles.
    

### Related Topics

-   [Setting Up Site Builder for Multiple Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2467073.html)
-   [Navigating Directly to a Subsidiary Website in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2467568.html)
-   [Subsidiary Management with Multiple Site Builder Sites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2467964.html)
-   [Selecting a Credit Card Gateway for a Subsidiary Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2468625.html)
-   [Displaying Items in Site Builder with OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2468868.html)
-   [OneWorld and SuiteCommerce](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282701.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
