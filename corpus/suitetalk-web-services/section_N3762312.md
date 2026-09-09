---
id: "section_N3762312"
type: "section"
title: "Lead Source"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Other Lists > Lead Source"
parent: "chapter_N3757146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3762312.html"
anchors: ["bridgehead_N3762332", "bridgehead_N3762490"]
sha256: "58cb2c01c82a1a344ecd445b35877ee40c0e68a220445e8568e24cea4a486940"
---

LeadSource defines a list of values that are used by the customer record to set the source of the lead for this customer - such as an ad or website referral (see [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html)).

If you use the Marketing Automation feature, the list of possible lead sources matches the titles of your marketing campaigns. Administrators can enable this feature at _Setup > Company > Enable Features > CRM_.

If you do not use the Marketing Automation feature, in the UI, a user-defined lead source list is defined at _Setup > Sales > Setup Tasks > CRM Lists > New > Lead Source_. Note the Marketing Automation feature must be turned off before you can create a user-defined lead source list.

For information about working with this record in the UI, see [Lead Sources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N975884.html).

## Supported Operations {#bridgehead_N3762332}

The following operations can be used with the lead source record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [getAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

Note:

The getAll operation should be used to retrieve values of a list since the search operation does NOT exist for this record.

## Field Definitions {#bridgehead_N3762490}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [lead source](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/leadsource.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

### Related Topics

-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
