---
id: "section_N3438708"
type: "section"
title: "User Defined Lists"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > User Defined Lists"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438708.html"
anchors: []
sha256: "25d786dfa54ea0177663d1c4116106e2f70dfe2407e14d23e80025cb5a5b9604"
---

In SOAP web services, many fields require internal ID values that correspond to an item in a user-defined list. To locate the internal ID of a specific value in a user-defined list, you must have the **Show Internal IDs** preference enabled in your account. For details, see [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html).

After enabling the **Show Internal IDs** preference, you can then go to the appropriate list within NetSuite. The internal ID values (also referred to as nsKeys) are displayed for each list item.

For example, the Status (_entityStatus_) field on the customer record takes an internal ID value from the Customer Status list, which is a user-defined list located at Setup > Sales > Customer Statuses. If you go to this page in NetSuite, you can see the internal ID values for each item in the column called **Internal ID**

Note:

Some user-defined lists can also be edited through SOAP web services to modify the values for the list. For details, see [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html).

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
