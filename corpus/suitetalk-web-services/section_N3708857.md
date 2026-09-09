---
id: "section_N3708857"
type: "section"
title: "Billing Rates Matrix List"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Shared Field Definitions for Items > Billing Rates Matrix List"
parent: "section_N3707811"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3708857.html"
anchors: ["bridgehead_N3708873", "bridgehead_N3709187"]
sha256: "add1cded91f57ea2ed388dd6f836111344070fc02a37b0d1e854df156497419f"
---

Use the Billing Rates list to set pricing for each billing class on service item records.

Because the Billing Classes feature is not compatible with the Quantity Pricing feature, you cannot use both features at the same time. If both are enabled, then billing classes replace quantity pricing on service item records.

## Billing Rates {#bridgehead_N3708873}

| Field Name | 
Type /

Field Length



 | Req. | Mapping | Notes |
| --- | --- | --- | --- | --- |
| billingClass | RecordRef | \- | Billing Rates / Billing Class | References a value in a user defined list at _Setup > Accounting > Setup Tasks > Accounting Lists > New > Billing Class_. |
| currency | RecordRef | \- | \- | References a value in a user-defined list at _Lists > Accounting > Currencies_. (Note that the Multiple Currencies feature must be enabled before you can set currency values.) This value sets the currency that all transactions involving this customer are conducted in. If defaults are OFF, this field is required. To retrieve a list of available values for this field, use the GetSelectValue operation. For more information, see [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) of the Platform Guide. |
| rateList | List | \- | Billing Rates | See [Rate](#bridgehead_N3709187). |

## Rate {#bridgehead_N3709187}

| Field Name | 
Type /

Field Length



 | Req. | Mapping | Notes |
| --- | --- | --- | --- | --- |
| priceLevel | RecordRef | \- | Billing Rates / \[Various Price Level\] | Sets the price Level this value is for. Price Levels are defined in a user defined list at _Setup > Accounting > Setup Tasks > Accounting Lists > New > Price Level_. For details on how to edit this list through SOAP web services, see [Price Level](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3765290.html). |
| value | double | \- | Billing Rates / Amount field for each price level | Sets the amount for the associated priceLevel. |

### Related Topics

-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
