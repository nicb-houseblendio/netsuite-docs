---
id: "section_N3428663"
type: "section"
title: "Records in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services"
parent: "chapter_N3428523"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html"
anchors: []
sha256: "c0ef15ef20b346db2e4b407c3ca88607b0ebb72b6dad1eb36bd8ea1111a79555"
---

Most standard NetSuite records are supported by SOAP web services. The list of supported records spans all areas of the NetSuite application from ERP to CRM to customization. For a list of records that are supported in SOAP web services, see [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html).

In the SOAP API, the Record class is the abstract super-class of all supported records. A supported record is always a concrete sub-class of Record. Due to the neutrality required to be language agnostic, the SOAP web services classes inheritance chain remains simplistic and does not implement language-specific object-oriented concepts such as multiple inheritance and interfaces.

NetSuite records are divided into the following broad categories:

-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
    
-   [Search Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html)
    
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
    

A record's standard body fields are its attributes, for example: `Customer.email, SalesOrder.salesRep`. Composite attributes such as line items or sublists are structured as complex objects that contain arrays, for example: `SalesOrder.itemList, CalendarEvent.attendeeList`. Custom fields within a record (if available) are also structured as composite attributes, for example: `Contact.customFieldList`.

Note:

A record element that ends with **List** is generally a sublist. (The exception is the customFieldList element, which represents custom fields on the record.) For information about working with sublists in SOAP web services, see [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html). For more general information about sublists and other form elements in NetSuite, see [Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2824615.html).

In addition to standard records, SOAP web services also supports custom objects and their metadata (see [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html) for more details). Using the [getCustomizationId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html) SOAP API, an application external to NetSuite can query a NetSuite account to obtain metadata about the custom objects that have been implemented in the account. This lets you build and ship generic applications that will work with any account. For example, a SOAP web services point-of-sale application can be designed to determine (during runtime) all the custom fields applied to a NetSuite CashSale record, so that it can then import CashSale records with the necessary custom fields set.

### Related Topics

-   [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html)
-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Forms in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439676.html)
-   [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
