---
id: "section_N3645002"
type: "section"
title: "Partner"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Partner"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3645002.html"
anchors: ["bridgehead_N3645034", "bridgehead_N3645307", "bridgehead_N3645344", "bridgehead_N3645353", "bridgehead_N3645365", "bridgehead_1544450568"]
sha256: "3d13844137bef24ae5088e8e83108e801b4e186400887c17466746c2e3a22d2a"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Partner](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0815024527.html).

A partner is a company you have a business agreement with who is not a customer or a vendor. To use partner records the Partner Relationship Management feature must be enabled at _Setup > Company > Enable Features > CRM_. For more details, see [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html).

The partner record is defined in the [listsRel (relationships)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD.

## Supported Operations {#bridgehead_N3645034}

The following operations can be used with partner records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3645307}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [partner](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/partner.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3645344}

## Setting a Partner as an Individual or a Company {#bridgehead_N3645353}

When creating a partner record, you can specify that partner as either an individual or a company by setting the isPerson field to TRUE or FALSE respectively. The available required and non-required fields vary depending on the setting of this field as detailed in the field definitions table.

## Giving Partners NetSuite Access {#bridgehead_N3645365}

You can update the PartnerContactRole sublist to provide Partner Center access to contacts. You can give this access to contacts attached to partners. This sublist is available for updates of Partner records only. Partners and contacts must already exist in NetSuite and contacts must already be attached to partners. You cannot use this sublist to attach new contacts. The workflow is as follows: 1) Add partner. 2) Add contacts. 3) Attach contacts to partner. 4) Update partner with contact access information from this sublist.

The fields in this sublist map to the fields on the Access subtab in the UI. These fields include:

-   A Boolean field that indicates whether a contact has access to NetSuite
    
-   A field that indicates whether new notification emails are sent when access changes are made
    
-   A field that indicates whether the password is manually assigned or changed
    
-   A contact name key field
    
-   The email address and password used to log in to NetSuite
    
-   The NetSuite role (Partner Center)
    

Operations on this sublist do not preserve row order. In some cases, rows added to the sublist will not be returned in the same order.

Note:

As of the 2011.2 endpoint, the PartnerContactList sublist is no longer supported. You can use the partnerContactRoleList instead. In addition, you can add or update contacts through the attach/detach operations, and you can retrieve contact names and roles for an entity through an advanced search on the entity record and its associated contacts. This advanced search technique is described in [Returning a Contact List for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html#bridgehead_N3641393).

## Working with the Tax Registration Sublist {#bridgehead_1544450568}

The tax registrations sublist is available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab.

Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services.

For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html).

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
