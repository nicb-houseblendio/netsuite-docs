---
id: "section_N3712676"
type: "section"
title: "Item Vendor List"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Shared Field Definitions for Items > Item Vendor List"
parent: "section_N3707811"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3712676.html"
anchors: []
sha256: "b1282df15212cafbbdd10264f253c2035c24c503cab4e440cf545ac9877605d2"
---

Use the Vendors List to add a list of vendors that can be used for this item. This information can then be accessed from the item record and from the corresponding vendor record.

The Multiple Vendors feature must be enabled to define item codes and purchase prices for multiple vendors on each item record. To enable this feature, go to _Setup > Company > Setup Tasks > Enable Features_. On the Items & Inventory subtab, in the Items section, check the Multiple Vendors box.

| Field Name | 
Type /

Field Length



 | Req. | Mapping | Notes |
| --- | --- | --- | --- | --- |
| preferredVendor | boolean | N | Basic / Preferred | You can only set one vendor in the list as preferred. If this is set true for multiple vendors, then the last vendor in the list is set as true and all others revert to false. |
| purchasePrice | double | N | Basic / Purchase Price | Sets the purchase price for this item when purchased from this vendor. |
| schedule | RecordRef | \- | \- | This field points to the quantity pricing schedule record, but is unique to the vendor and can only be created from the vendor record. In the UI go to Financial > Schedules > New Pricing Schedule. |
| subsidiary | string | N | Subsidiary | \- |
| vendor | RecordRef | Y | Basic / Vendor | References an existing vendor record. This is required for each vendor being defined. To retrieve a list of available values for this field, use the GetSelectValue operation. For more information, see [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) of the Platform Guide. |
| vendorCode | string / 15 | N | Basic / Vendor | Sets the vendor's item code. |
| vendorCurrencyName | string | \- | \- | \- |

### Related Topics

-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
