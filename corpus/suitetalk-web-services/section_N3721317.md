---
id: "section_N3721317"
type: "section"
title: "Noninventory Purchase Item"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Noninventory Purchase Item"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3721317.html"
anchors: ["bridgehead_N3721329", "bridgehead_N3721553", "subsect_161485804039"]
sha256: "fbd4ccbbf1e8779fd365611c1343fc533053d6595218090ce25ef42006e4a09c"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Non-Inventory Purchase Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0120113247.html).

Noninventory purchase item records are used to track something you buy but do not stock.

For more information, see [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html).

## Supported Operations {#bridgehead_N3721329}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3721553}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [noninventory purchase item](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/noninventorypurchaseitem.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#subsect_161485804039}

See the following code sample of the get operation:

            `RecordRef item = new RecordRef();         item.setInternalId("249");         item.setType(RecordType.nonInventoryPurchaseItem);         c.getPort().get(item);  [SOAP request] <soapenv:Body>       <get xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">          <baseRef internalId="249" type="nonInventoryPurchaseItem" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2019_1.platform.webservices.netsuite.com"/>       </get> </soapenv:Body>  [SOAP response] <soapenv:Body>       <getResponse xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">          <readResponse>             <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com"/>             <record internalId="249" xsi:type="listAcct:NonInventoryPurchaseItem" xmlns:listAcct="urn:accounting_2019_1.lists.webservices.netsuite.com">                <listAcct:createdDate>2021-03-03T00:52:12.000-08:00</listAcct:createdDate>                <listAcct:lastModifiedDate>2021-03-03T00:52:12.000-08:00</listAcct:lastModifiedDate>                <listAcct:cost>10.43</listAcct:cost>                <listAcct:expenseAccount internalId="78" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:name>Miscellaneous Expense</platformCore:name>                </listAcct:expenseAccount>                <listAcct:customForm internalId="-210" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:name>Standard Non-Inventory Part Form</platformCore:name>                </listAcct:customForm>                <listAcct:itemId>Sample Non-inventory Item for purchase</listAcct:itemId>                <listAcct:upcCode>49378210</listAcct:upcCode>                <listAcct:displayName>Some display name</listAcct:displayName>                <listAcct:includeChildren>false</listAcct:includeChildren>                <listAcct:isInactive>false</listAcct:isInactive>                <listAcct:availableToPartners>false</listAcct:availableToPartners>                <listAcct:department internalId="1" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:name>Department  US</platformCore:name>                </listAcct:department>                <listAcct:location internalId="7" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:name>Location US 2</platformCore:name>                </listAcct:location>                <listAcct:subsidiaryList xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:recordRef internalId="1">                      <platformCore:name>Parent Company</platformCore:name>                   </platformCore:recordRef>                </listAcct:subsidiaryList>                <listAcct:taxSchedule internalId="1" xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                   <platformCore:name>S2</platformCore:name>                </listAcct:taxSchedule>                <listAcct:isFulfillable>true</listAcct:isFulfillable>                <listAcct:generateAccruals>false</listAcct:generateAccruals>                <listAcct:currency>1</listAcct:currency>                <listAcct:translationsList>                   <listAcct:translation>                      <listAcct:locale>_frenchFrance</listAcct:locale>                      <listAcct:language>French (France)</listAcct:language>                   </listAcct:translation>                   <listAcct:translation>                      <listAcct:locale>_russian</listAcct:locale>                      <listAcct:language>Russian</listAcct:language>                   </listAcct:translation>                   <listAcct:translation>                      <listAcct:locale>_chineseSimplified</listAcct:locale>                      <listAcct:language>Chinese (Simplified)</listAcct:language>                   </listAcct:translation>                </listAcct:translationsList>             </record>          </readResponse>       </getResponse> </soapenv:Body>` 
          

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
