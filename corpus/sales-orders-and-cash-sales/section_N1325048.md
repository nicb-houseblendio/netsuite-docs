---
id: "section_N1325048"
type: "section"
title: "Setting Up Items for Contract Renewals"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Setting Up Items for Contract Renewals"
parent: "section_N1320628"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325048.html"
anchors: []
sha256: "33222b414fc9b7d6a8de92e2d4ae558b4c73f41df0ae42243736b1f07c3f7e33"
---

Item records define how renewal transactions and contracts are generated. If an item is set up for automated renewal, it is automatically included in contracts and renewal transactions.

Typically, contract items are defined with an item type of Non-inventory Item for Sale in NetSuite. The renewal behavior is determined by the fields under the Vertical Classification section on item records.

#### To set up items for Contract Renewals

1.  Go to Lists > Accounting > Items > New.
    
2.  Select the item type for the contract item that you want to create. Most contract items are defined with an item type of Non-inventory Item for Sale. For more information about NetSuite item types, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
3.  On the Item form, make sure that a Contract Renewal custom form is selected in the **Custom Form** field. For more information about setting preferred forms, see [Setting Preferred Forms for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321283.html).
    
4.  Enter values in the fields on the Primary Information and Classification sections as you would in a standard item form. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
5.  On the Vertical Classifications section, specify values for the fields that will determine the renewal behavior of the item. Refer to [Fields for Configuring Renewal of Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1229081902.html).
    
6.  Specify the item price on the **Pricing** subtab.
    
    Note:
    
    When you enter pricing for percentage based maintenance and support items, you must set the base price to zero so that pricing is calculated correctly.
    
    If you use the Project Management feature, be sure to enter a base price on the service item record or enter zero (instead of leaving the Base Price field blank) if the service item doesn't have a base price. For information about setting the base price of a service item see, [Setting Up Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181018.html). For more information about the Project Management feature, see [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html).
    
7.  Enter values in the fields on the other subtabs as you would in a standard item form. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
    If you use the Advanced Billing and Advanced Shipping features and you don't want to fulfill orders, be sure to clear the **Can be Fulfilled/Received** box on the **Preferences** subtab for items that you include in contracts.
    

You shouldn't use kits or assemblies for renewable software items because these item types don't include the derived information required to generate contract items. You can, however, use item groups to make entering transaction line renewable items easier. For more information about item groups, see [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html#bridgehead_N2318108).

### Related Topics

-   [Software Vertical Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1319596.html)
-   [Contract Renewals Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4442063121.html)
-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html)
-   [Setting Up Maintenance/Support for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1324612.html)
-   [Setting Up Product Lines for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1324952.html)
-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)
-   [Software Vertical Contract Renewals References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4581932984.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
