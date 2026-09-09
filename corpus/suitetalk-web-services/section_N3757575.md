---
id: "section_N3757575"
type: "section"
title: "Usage Notes for Other List Record Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Other Lists > Usage Notes for Other List Record Types"
parent: "chapter_N3757146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3757575.html"
anchors: ["bridgehead_N3757606"]
sha256: "54fce8795b936c214177be158283d2f7252e0b523dfc8e741fd13af032960ac4"
---

Other list records represent user-defined lists that define items that can be selected for a specific field.

For example, in the contact record, you can set the type of contact in the _category_ field. The _category_ field references the ContactCategory record, which contains a predefined list of different contact types.

All other list record types are defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Permissions {#bridgehead_N3757606}

In cases where the logged in user's role does NOT have permissions for the specified other list record, the get() operation will return only the key/name information instead of the whole record. This is to ensure that these lists can be manipulated when they are included as select or multiselect fields within another record.

### Related Topics

-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
