---
id: "section_N3643434"
type: "section"
title: "Contact"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Contact"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3643434.html"
anchors: ["bridgehead_N3643455", "bridgehead_N3643726", "bridgehead_N3643763", "bridgehead_N3643772", "bridgehead_N3643784"]
sha256: "6247c50d48a8c641d94c5dc09080a4c6e9c0364e96ad2f8f2c184110ca546a94"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Contact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159170320047.html).

Contacts represent people or companies that you deal with in the daily activity of your business. Use the contact record to create, modify, or delete contacts and associate a contact to a parent record. For information about working with this record in the UI, see [Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1075037.html).

The contact record is defined in the [listRel (relationship)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD.

## Supported Operations {#bridgehead_N3643455}

The following operations can be used to manipulate the contact record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3643726}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [contact](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/contact.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3643763}

## Working with Contact Sublists {#bridgehead_N3643772}

The SOAP Schema Browser includes all sublists (lists) associated with the contact record. See the following information for usage notes regarding specific contact lists. Note that usage notes are not provided for every list type.

## AddressbookList {#bridgehead_N3643784}

The addressBookList field is a list field that lets you provide multiple addresses for a contact. These fields are all mapped to the Address subtab in the UI.

When you work with the addressbookList in the 2009.2 endpoint and beyond, be sure to use **internalId** as the key. Do not use **label**. For the 2009.1 and lower endpoints, the addressbookList is not a keyed sublist, but you can use label to identify records.

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
