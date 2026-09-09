---
id: "section_N2182221"
type: "section"
title: "Setting Up Items for Multiple Price Levels"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Using Multiple Pricing > Setting Up Items for Multiple Price Levels"
parent: "section_N2181607"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182221.html"
anchors: ["procedure_N2182229"]
sha256: "ddae4df00063e80142905d4c18995ba9b4e7d4f74f607913ab2434370be29b8e"
---

Here's how you can set up multiple prices on item records. You can create up to 1,000 different price levels to select on the sales order.

#### To set up multiple prices on item records: {#procedure_N2182229}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the item.
    
3.  Click the **Sales/Pricing** subtab.
    
4.  Enter up to four prices in the **Base Price**, **Alternate Price 1**, **Alternate Price 2**, **Alternate Price 3** and **Online Price** fields.
    
    To add more price levels, go to _Setup > Accounting > Setup Tasks > Accounting Lists > New_. Click **Price Level**.
    
    To get a rate on a specific Price Level in a formula through Saved Search or a Custom Field, use this mapping:
    
    **Base Price** - use the format `price`
    
    **Other price levels** - use the format pricelevel<_price level ID_\>. For example, `pricelevel4`
    
    Important:
    
    When customers order online, the online price overrides all other prices.
    
    If your customers can order online and you don't enter an online sales price, the Base Price shows as the online price.
    
5.  Click **Save**.
    

The multiple sales prices you set show up on sales transactions in the Price Levels list.

Tip:

To improve performance, inactivate price levels you're not using right now.

### Related Topics

-   [Editing Multiple Prices on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2182345.html)
-   [Creating Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181938.html)
-   [Setting Up Price Levels for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182485.html)
-   [Editing Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2182796.html)
-   [Assigning a Foreign Currency Price to a Sales Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183023.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
