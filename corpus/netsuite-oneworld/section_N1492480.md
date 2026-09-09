---
id: "section_N1492480"
type: "section"
title: "Manage Intercompany Orders"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Intercompany Sales and Billing Transactions Overview > Manage Intercompany Orders"
parent: "section_N1492389"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492480.html"
anchors: []
sha256: "c33bedda54966321724d872aa8affd9ee679596ffa5f765bcf174f075b8f038e"
---

The Manage Intercompany Sales Order page shows intercompany purchase orders that have an intercompany transaction status of Pending or Rejected.

Intercompany orders can have the following statuses:

-   **Pending** indicates that the intercompany order has not been paired with a corresponding order in another subsidiary. Order pairs are Sales Order/Purchase Order and Vendor Return Authorization/Return Authorization.
    
    Note:
    
    Intercompany orders that are pending approval do not appear on this page.
    
-   **Rejected** indicates that the intercompany purchase order or vendor return authorization can't be paired with a sales order or return authorization. Usually this is because it contains incorrect information such as subsidiary, currency, amount, or other detail.
    
-   **Linked** indicates that the intercompany order has been paired with an intercompany order in another subsidiary. Order pairs are Sales Order/Purchase Order and Vendor Return Authorization/Return Authorization. The Manage Intercompany Sales Order page doesn't display linked orders.
    

Intercompany Order Status appears only on intercompany sales orders, intercompany purchase orders, intercompany return authorizations, and intercompany vendor return authorizations.

Select a customer and a currency on the Manage Sales Order page to filter the list of displayed purchase orders. This is the list of intercompany purchase orders not paired with intercompany sales orders. Setting the filter also determines the customer, subsidiary, and currency for the sales order to be created.

Access to subsidiary data is controlled by your user role. If you are not an administrator, you can use the Manage Intercompany Sales Order page if you have been granted the required permission. To view a Purchase Order in another subsidiary, your user role must have the **Allow Cross-Subsidiary Record Viewing** option set. Your user role also must have view access to Purchase Order. To automatically generate and create a Sales Order, you must have create or full permissions to Sales Order. For more information, see [Control Employee Access to Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278097.html).

From the Manage Intercompany Sales Orders page, you can:

-   Generate sales orders for select purchase orders
    
-   Manually create a sales order for a purchase order
    
-   Reject intercompany purchase orders
    
-   View rejected intercompany purchase orders
    

### Related Topics:

-   [Generating an Intercompany Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159249226797.html)
-   [Manually Creating a Paired Intercompany Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159249207006.html)
-   [Rejecting an Intercompany Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159249066244.html)
-   [Pairing Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158989895273.html)
-   [Intercompany Sales and Billing Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492389.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
