---
id: "section_N277674"
type: "section"
title: "Associate Subsidiaries With Shipping Items"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Associate Subsidiaries with Entities and Items > Associate Subsidiaries With Shipping Items"
parent: "section_N276477"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N277674.html"
anchors: ["bridgehead_N277883", "subsect_163007428057", "procedure_N277908"]
sha256: "39f7eae517e74255efa208958d1f0066dcfe397f5cdd813a175a3f5f195756d1"
---

In NetSuite OneWorld, you assign a shipping item to a subsidiary so that it can be used for transactions. You can associate only one subsidiary with a shipping item, but you can create multiple shipping items for the same shipping service. You can then use the shipping services across multiple subsidiaries. The shipping services respect currencies and post to the appropriate subsidiary accounts.

Shipping items for the same service have a unique Ship Name but share the same Display/Code name. Shipping items use real-time rates and shipping label integration features associated with the carrier.

For example, you have two subsidiaries, one for your operations in the United States and one for operations in Canada. You use UPS Ground service for shipping needs in both subsidiaries. Create a shipping item for each subsidiary with a Ship Name that identifies the subsidiary where it is to be used:

|  | US Subsidiary | Canada Subsidiary |
| --- | --- | --- |
| Ship Name | UPS Ground - US | UPS Ground - CA |
| Display Name /Code | UPS Ground | UPS Ground |
| Subsidiaries | US | Canada |

When you select a customer on a transaction, only shipping items for the subsidiary attached to that customer display in the list for Shipping Method.

In the Web store, an unregistered shopper without a customer record can choose shipping items associated with the subsidiary website being viewed. When a registered customer logs in to your Web store, the shopper can see only those shipping items associated with the customer's record. For example, a shopper in Canada sees only those shipping items associated with the Canadian subsidiary.

## Associate a Subsidiary With a Shipping Item {#bridgehead_N277883}

Follow the instructions for creating a shipping item at [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html). This procedure includes a step to select the subsidiary for the shipping item. You can select only one subsidiary for a shipping item.

## Creating Multiple Shipping Items for the Same Shipping Service {#subsect_163007428057}

Use the following procedure to create shipping items for the same shipping service.

#### To create multiple shipping items for the same shipping service: {#procedure_N277908}

1.  Edit an existing shipping item at _Lists > Accounting > Shipping Items_. Click **Edit** next to the shipping item you want to modify.
    
    Create a new shipping item at _Lists > Accounting > Shipping Items > New_.
    
2.  In the **Ship Name** field, enter an internal name for the shipping item. To identify the shipping item by subsidiary, include the subsidiary in the name, for example, **UPS Ground - U.S.**
    
3.  The **Display Name/Code** defaults from the shipping service you select as the real-time rate on the **Shipping Rate** subtab. This is the shipping method name as it appears to customers visiting your Web store. It also appears on printed invoices and in centers such as the Customer Center. You can't modify the **Display Name/Code**.
    
4.  In the **Subsidiaries** field, select the subsidiary you want to offer this shipping item in.
    
5.  Click **Save**.
    

For information about shipping items, see [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html).

### Related Topics

-   [Assigning a Subsidiary to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276604.html)
-   [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html)
-   [Assigning a Subsidiary to a Partner](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276702.html)
-   [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html)
-   [Associate Subsidiaries With Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276948.html)
-   [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
