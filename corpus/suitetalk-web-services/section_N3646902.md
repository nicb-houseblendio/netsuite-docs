---
id: "section_N3646902"
type: "section"
title: "Vendor"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Vendor"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3646902.html"
anchors: ["bridgehead_N3646922", "bridgehead_N3647195", "bridgehead_N3647232", "bridgehead_N3647240", "bridgehead_N3647268", "bridgehead_1544450629", "bridgehead_N3647280"]
sha256: "9d0dba71b420e215caf58c024a520b9ed9626f291989e557a036e25e0ed9e1ab"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_164337045826.html).

A vendor is a company or person you purchase goods and services from. Vendor records track information about your vendors and enable you to view past transactions and communications with them. For information about working with vendor records in the UI, see [Vendor Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2360495.html).

The vendor record is defined in the [listsRel (relationships)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD.

## Supported Operations {#bridgehead_N3646922}

The following operations can be used to modify vendor records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3647195}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [vendor](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendor.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3647232}

## Working with Vendor Lists {#bridgehead_N3647240}

The SOAP Schema Browser includes all lists (sublists) associated with the vendor record. However, see the following information for usage notes regarding specific vendor lists. Note that usage notes are not provided for every list type.

Note:

As of the 2011.2 endpoint, the VendorContactList sublist is no longer supported. You can add or update contacts through the attach/detach operations, and you can retrieve contact names and roles for an entity through an advanced search on the entity record and its associated contacts. This advanced search technique is described in [Returning a Contact List for a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html#bridgehead_N3641393).

## VendorPricingScheduleList {#bridgehead_N3647268}

This list can only be edited on an update. It defines the quantity pricing schedules to use for the vendor. The Quantity Pricing feature must be enabled to access this list.

## Working with the Tax Registration Sublist {#bridgehead_1544450629}

The tax registrations sublist is available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab.

Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services.

For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html).

## Note about Multiple Currencies and Vendors {#bridgehead_N3647280}

When the Multiple Currencies feature is enabled, the label for the Currency field on the vendor record changes to Primary Currency (internal id of the field is still currency) and a Currency sublist is added to the vendor record. Also, the purchasePrice field in ItemVendorList becomes hidden but this field's values can still be saved through SOAP web services.

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
