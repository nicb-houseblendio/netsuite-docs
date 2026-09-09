---
id: "chapter_N2164525"
type: "chapter"
title: "Using Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Using Item Records"
parent: "book_N2164398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html"
anchors: ["subsect_161912132341", "subsect_161912136173", "subsect_161912138664", "subsect_161912141882"]
sha256: "1fa3d34bf681f478d7234dc53feddceedec37c6f184bc1889255361b0bc8017d"
---

Item record management begins with creating item records for all of the items you use on transactions. There are many item types available for creating records.

Important:

Don't use NetSuite special accounts when using item records. They may cause inventory errors.

Items are the goods and services you sell to customers, and the parts and raw materials you purchase from vendors. They can also include line items on sales and purchase forms. For example, discounts and miscellaneous charges. With item records, you can enter or define products and services you buy or sell and track their details.

After you have set up item records, you can maximize the item and inventory management in the following ways:

-   [Restricting Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2176374.html) - helps to limit the visibility of designated items for selected employees and partners. This enables you to work more efficiently by decreasing the possibility of entry errors.
    
-   [Setting Up Items for the Web Site](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585301.html#section_N2177433) - lets you define whether an item can be viewed or purchased in your web store, and how it should be displayed and sold.
    
-   [Working With Multi-Language Names and Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2178279.html)\- enables you to translate your web site. On printed transaction forms, customers see item names, descriptions, and expense categories in the language selected on the customer record.
    
-   [Related Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2179943.html) - help you to find transactions related to an item. To track updates to fields on the item record, refer to item user notes and NetSuite system notes.
    

## Item Pricing {#subsect_161912132341}

Item Pricing lets you set a single price for each item or different prices for the items you sell. The available options for creating different include Multiple Pricing, Quantity Pricing, or Pricing Groups

-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html) - lets you set different price levels for each item. Multiple price levels improves flexibility to set different pricing for different customers. For example, you can set up several pricing levels that sell items at one price for retail customers, another price for wholesale customers. You can alternatively give 5%, 10% or 15% discounts on retail pricing.
    
-   [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html) - lets you automatically apply different sales prices to items that depend on the quantity being sold. This enables you to offer discounts to customers who buy in bulk.
    
-   [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html) - enable you to assign customer-specific price levels for groups of items. For example, you could create a pricing group called Laptops and associate the pricing group with all of your laptop items.
    

Note:

In an account that has the Quantity Pricing Schedules feature enabled, only schedules with matching units type can be item.

When sales prices or purchase prices change, use [Updating Item Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184312.html) and [Updating Item Purchase Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184741.html) to keep records up to date. This results in more accurate data when you create transactions.

To exchange the prices of two existing price levels, use the [Swapping Prices Between Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185052.html) feature. For example, you have created Level One (retail pricing) and Level Two (retail less 5 percent). You can swap the prices for both price levels so that the price Level One reflects a 5% discount and Level Two reflects retail pricing.

When [Creating Item Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185383.html), you can offer coupon codes that apply to specific items when you enable the Promotion Codes feature.

## Multiple Units of Measure {#subsect_161912136173}

The Multiple Units of Measure feature enables you to define units used to stock, buy, and sell inventory items. Units of measure gives you more flexibility and accuracy when tracking and selling inventory. For example, you can purchase cable in pallets, stock the cable in spools, and sell the cable in feet.

## Item Costing {#subsect_161912138664}

If you use both the Accounting and Inventory features, you need to track the total value of your assets and calculate profits you make. Each time you buy and sell inventory items, track the cost of your items throughout the purchase and sale processes. The cost of an item you buy or sell affects general ledger accounts.

-   [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html) - enable you to track the costs associated with goods and services you sell.
    
-   [Standard Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2199708.html) - tracks standard costs for inventory.
    
-   [Setting a Default Inventory Costing Method](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345703007.html) - defines the costing method your items use. The cost of inventory is determined by your items' purchase prices and all costs incurred in acquiring these items. The costing method you choose determines how you handle the costs associated with buying the same items at different purchase prices over a certain period.
    
-   [Initial Average Cost](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html#subsect_0707085636) - enables you to specify and apply this cost per location, if you use the Multi-Location Inventory feature.
    
-   [Viewing Inventory Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197076.html) - determines the cause of an inventory costing problem.
    

## Bar Codes and Item Labels {#subsect_161912141882}

The Bar Codes and Item Labels feature lets you enter and track information by generating [Bar Codes and Item Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2215205.html) for each item and transaction. For example, you can:

-   Print labels to affix to the items that show the item price, and bar codes for item number and serial number.
    
-   Scan bar code labeled items to add to a sales transaction or receive them on a purchase transaction.
    
-   Scan transaction bar codes to bulk receive, fulfill, pick, pack, ship, bill or approve orders.
    

NetSuite automatically generates bar codes for items in UPC or Code 128 format based on Item Name/Number or Stock Keeping Unit (SKU).

### Related Topics

-   [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html)
-   [Viewing the Items List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2176664.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)
-   [Item Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2191369.html)
-   [Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2211898.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)
-   [Customer Part Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4575965810.html)
-   [Effective Date Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1536354469.html)
-   [Item Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2164398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
