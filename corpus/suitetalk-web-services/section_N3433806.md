---
id: "section_N3433806"
type: "section"
title: "External IDs Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services > External IDs Overview"
parent: "section_N3428663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html"
anchors: ["bridgehead_4757704997"]
sha256: "425d1ea36e8d1e8efe9f0bb8b9dc1629ac5b97e17b6899f82ac7e2faae5980a6"
---

The externalId attribute of a RecordRef provides a means to reference an object by its foreign key in an external database.

You can set the externalID attribute during an add or update operation. External IDs are useful in the following situations:

-   **Maintaining client ID relationships**
    
    In cases where a client application already maintains references between records, set the externalId attribute for each record during imports. In subsequent API calls, you can then reference associated records by the known external ID. Note that SuiteScript does not support external IDs.
    
-   **Establishing relationships during a single import operation**
    
    For example, suppose you want to import customer records with references to sales reps into NetSuite. If no external ID is used, you would need to import the customer records, determine the IDs of the related sales reps' employee records, and then re-import the customer records with the sales reps ID references. By providing an external ID, you can import the customer records in a single API call using the external ID references to the sales reps.
    

To prevent duplicate records, you should use external IDs and the upsert and upsertList operations to add records to NetSuite.

Most NetSuite record types support the use of external ID, but not all do. The following list identifies the record types that do not support external ID. For all other records, you should assume that external ID is supported. When in doubt, refer to the appropriate page in the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html). On each page describing a record type, view the Attributes table to see whether external ID is supported.

Important:

External IDs are not displayed on records by default. However, you can search for external IDs, or you can add a custom field to the record types where you want to the external ID to be displayed in the UI. For information about searching in SOAP web services, see [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html). For information about working with custom fields, see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html).

The record types that do not support external ID are:

-   Accounting Period
    
-   Budget Category
    
-   CRM Custom Field
    
-   Custom List
    
-   Custom Record Custom Field
    
-   Custom Record Type
    
-   Entity Custom Field
    
-   Gift Certificate
    
-   Item Custom Field
    
-   Item Number Custom Field
    
-   Item Option Custom Field
    
-   Landed Cost
    
-   Other Custom Field
    
-   State
    
-   Transaction Body Custom Field
    
-   Transaction Column Custom Field
    

## Guidelines for External IDs {#bridgehead_4757704997}

Consider the following guidelines for external IDs:

-   External IDs must be unique not only within a single record type, but also within certain record groups. For details about record types and record groups, see [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html).
    
-   External IDs can be updated through CSV import, user event scripts, or web services. Therefore, your organization should use a single approach for maintaining external IDs, so that external IDs are not unknowingly updated using separate methods.
    
    Although records of a particular type may be used in multiple integration scenarios, each record instance can only have a single external ID value. To maintain data integrity, only a single integrated application can set and update external ID values for each record type. External ID values for all records of a particular type must all be from the same external application.
    
-   External IDs are case insensitive in web services references. For details, see [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html).
    

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
-   [Search Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html)
-   [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
