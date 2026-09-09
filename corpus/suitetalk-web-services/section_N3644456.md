---
id: "section_N3644456"
type: "section"
title: "Group (Entity Group)"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Group (Entity Group)"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3644456.html"
anchors: ["bridgehead_N3644482", "bridgehead_N3644741", "bridgehead_N3644778", "bridgehead_N3644795", "bridgehead_4791382461"]
sha256: "e48e9730966e8305af1f51d09a58cce491d00af46f5e700f0cf8e6f9b606c763"
---

The group record is defined in [listRel (relationships)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD.

Specify the group type (contact, customer, employee, partner, or vendor) by setting the type element on an add operation. Note that the group record cannot be customized. Also note that in NetSuite, groups can be dynamic or static. To create a dynamic group, on the group record you must set the group type to dynamic. You can then reference a saved search when adding the group record. The members will change based on the results of the saved search. To create a static group, first add the group record to NetSuite. Then use the **attach** operation to associate members with it. For more information and for examples of using the attach operation, see [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html).

For information about working with groups in the UI, and about adding and removing members, see [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html).

## Supported Operations {#bridgehead_N3644482}

The following operations can be used with the group record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3644741}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [entity group](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/entitygroup.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3644778}

When searching for members of a **dynamic** group, you must use the GroupMemberSearchBasic search interface; you cannot use the group's corresponding entity search. The GroupMemberSearch interface retrieves members of a dynamic group by referencing the groupId.

## GroupMemberSearchBasic {#bridgehead_N3644795}

| Field Name | Type |
| --- | --- |
| groupId | platformCore:RecordRef |

| Field Name | Type |
| --- | --- |
| groupId | platformCore:SearchMultiSelectField |

The following code snippet shows GroupMemberSearchBasic in a SOAP request.

## SOAP Request {#bridgehead_4791382461}

          `<soapenv:Body>    <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <searchRecord xsi:type="ns7:GroupMemberSearchBasic" xmlns:ns7="urn:common_2017_1.platform.webservices.netsuite.com">          <ns7:groupId internalId="163" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>       </searchRecord>    </search> </soapenv:Body>` 
        

If the entity group is not dynamic, you can use the standard EntityGroupSearch interface to execute a search against the group.

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
