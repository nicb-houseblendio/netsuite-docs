---
id: "section_N3707950"
type: "section"
title: "Pricing Matrix List"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Shared Field Definitions for Items > Pricing Matrix List"
parent: "section_N3707811"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707950.html"
anchors: ["bridgehead_N3708345", "bridgehead_N3708589"]
sha256: "f0187646908a025613aeae52af1e310e6793db08370d3e38b72eaba226ab2367"
---

The Pricing Matrix List provides various pricings for a specific item. This list is supported when one or more of the following features are enabled: Multiple Currencies, Multiple Prices, and Quantity Pricing. For each item, you can set multiple pricings based on the following:

-   Currency the item is offered in
    
-   Price levels available for the item - as defined in the price level user defined list
    
-   The quantity of items being sold - when the Quantity Pricing feature is enabled
    

| Field Name | 
Type /

Field Length



 | Req. | Mapping | Notes |
| --- | --- | --- | --- | --- |
| currency | RecordRef | Y/N | \- | References the currency the price level will be set for. This field is required when the multi-currency preference is ON. Otherwise, the default currency is sourced for this field and it is NOT required. |
| discount | double | Y | Pricing / Default Discount % | This is a read-only field that returns the discount rate associated with the priceLevel. |
| priceLevel | RecordRef | Y | Pricing / Price Level | This is a read-only field that references values in a user-definable list at _Setup > Accounting > Setup Tasks > Accounting Lists > New > Price Level_. For details on how to edit this list, see [Price List](#bridgehead_N3708345). |
| pricelist | List | N | \- | See [Price List](#bridgehead_N3708345). |

## Price List {#bridgehead_N3708345}

To provide multiple entries in the Price List, the Quantity Pricing feature must be enabled. Otherwise, only one Price List entry should be submitted. Notice that in the UI, the quantity for multiple pricings is entered only one time. In SOAP web services, however, you must submit the quantity for **each** pricing. The quantity values for each price submitted in the same list **must match**. If they do NOT match, an error is returned.

| Field Name | 
Type /

Field Length



 | Req. | Mapping | Notes |
| --- | --- | --- | --- | --- |
| quantity | double | \- | Qty | Sets the quantity required to receive this price. |
| value | double | \- | Pricing / amount text box | This is calculated based on the Base Price level and discount rate for the specified priceLevel but can be overwritten. |

## Pricing Matrix Keys {#bridgehead_N3708589}

The key for the Pricing Matrix List varies according to the related features that are enabled. The key is the field or combination of fields with values that are used to uniquely identify each line in the list. The following table describes possible key combinations.

| **Enabled Feature(s)** | Key Field(s) |
| --- | --- |
| Multiple Currencies only | currency |
| Multiple Currencies, Multiple Prices | combination of currency, priceLevel |
| Multiple Currencies, Quantity Pricing | combination of currency, quantity |
| Multiple Currencies, Multiple Prices, Quantity Pricing | combination of Currency,priceLevel, quantity |
| Multiple Prices only | priceLevel |
| Multiple Prices, Quantity Pricing | combination of priceLevel, quantity |
| Quantity Pricing Only | quantity |

Important:

In endpoints prior to 2012.1, pricingMatrixList updates ignore the replaceAll attribute and all requests behave as if it is set to TRUE. For the 2012.1 and later endpoints, replaceAll is respected. If you upgrade to one of these later endpoints, you need to carefully evaluate which replaceAll setting to use for pricing updates. For details about how replaceAll works with matrix sublists, see [Matrix Sublists and replaceAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html#bridgehead_N3443249).

### Related Topics

-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
