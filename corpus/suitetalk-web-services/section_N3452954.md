---
id: "section_N3452954"
type: "section"
title: "Complex Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Types > Complex Types"
parent: "chapter_N3452524"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html"
anchors: ["bridgehead_N3453226", "bridgehead_1488965347", "bridgehead_N3453509", "bridgehead_N3454445", "bridgehead_N3454588", "bridgehead_N3454730", "bridgehead_N3454996", "bridgehead_N3455299", "bridgehead_N3455609", "bridgehead_N3455809", "bridgehead_N3456068", "bridgehead_N3456218", "bridgehead_N3457524", "bridgehead_N3457683", "bridgehead_N3457857"]
sha256: "a68fb5c47916550b3bab3d56ed31736c0cdabe577c74fa59324ba01a8d74ea5f"
---

Complex types are structured types built by aggregating elements of simple or previously defined complex types. NetSuite complex types are defined in the platform core and platform core types XSDs. All NetSuite record types ultimately reference one of these complex types.

NetSuite complex types include the following:

-   [Passport](#bridgehead_N3453226)
    
-   [TokenPassport](#bridgehead_1488965347)
    
-   [Record](#bridgehead_N3453509)
    
-   [RecordList](#bridgehead_N3454445)
    
-   [BaseRef](#bridgehead_N3454588)
    
-   [RecordRef](#bridgehead_N3454730)
    
-   [CustomRecordRef](#bridgehead_N3454996)
    
-   [ListOrRecordRef](#bridgehead_N3455299)
    
-   [Status](#bridgehead_N3455609)
    
-   [StatusDetail](#bridgehead_N3455809)
    
-   [NullField](#bridgehead_N3456068)
    
-   [ReadResponse](#bridgehead_N3456218)
    
-   [ListReadResponse](#bridgehead_N3457524)
    
-   [ListWriteResponse](#bridgehead_N3457683)
    
-   [WriteResponse](#bridgehead_N3457857)
    

## Passport {#bridgehead_N3453226}

Important:

As of the 2020.2 SOAP web services endpoint, authentication through request-level credentials is not supported. The Passport complex type is not supported. If you attempt to authenticate through request-level credentials in SOAP web services 2020.2 and later endpoints, the web services request is not processed, and an error message is returned. You must ensure that SOAP web services integrations created with 2020.2 and later SOAP web services endpoints use TBA. Authentication through user credentials continues to be supported in integrations that use SOAP web services 2020.1 and earlier endpoints. For more information, see [Token-based Authentication and Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4381113277.html).

The Passport type is used by the login operation to encapsulate the security credentials required for authentication. The passport type is defined in the core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| email | xsd:string | Y |  |
| password | xsd:string | Y |  |
| account | xsd:string | Y | Must correspond to a valid NetSuite account number |
| role | RecordRef | Y | A role is a set of permissions that lets a user access specific areas of data. If not set, NetSuite uses the default Web Services role set for this user. |

The default web services role for a specific user is dependent on the values set when setting the permissions for a particular role. These are set through the UI in _Setup > Users/Roles > Manage Roles_.

## TokenPassport {#bridgehead_1488965347}

The TokenPassport type is used by SOAP web services requests that use token-based authentication. The TokenPassport type is defined in the core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| account | xsd:string | Y |  |
| consumerKey | xsd:string | Y |  |
| token | xsd:string | Y |  |
| nonce | xsd:string | Y |  |
| timestamp | xsd:long | Y |  |
| signature | xsd:string | Y |  |

Note:

For information about the TokenPassport type, see [TokenPassport Complex Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4395630653.html).

## Record {#bridgehead_N3453509}

The Record type is an abstract type used as the parameter for the add, addList, delete, deleteList, update and updateList operations. It is also returned in the get, getList, search, searchMore and searchNext operations. All business object types extend the Record type. The record type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| id | xsd:string (attribute) | N |  |
| xsi:type | xsi:type (attribute) | N | This is a field (attribute) that is automatically implemented by the XML Schema. The value should represent the concrete Record type such as Customer or Event. |
| nullFieldList | NullFields\[\] | N | A list of fields that are to be set to null explicitly in the update operation. Note: You cannot set the Custom Form field to NULL. Any request to set this field to NULL is ignored. |

## RecordList {#bridgehead_N3454445}

The RecordList type is an array of the Record type. The recordList type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| record | Record \[\] | N |  |

## BaseRef {#bridgehead_N3454588}

The BaseRef type is an abstract type used to reference any existing record in NetSuite including other business records and custom records. The BaseRef type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| name | BaseRef | N |  |

## RecordRef {#bridgehead_N3454730}

The RecordRef type is used to reference an existing record in NetSuite in get operations. Typically, a RecordRef references one of the following:

-   Another business object such as a customer or sales order
    
-   An entry in a user defined list such as the category list for contacts or sales tax items
    

The recordRef type descends from BaseRef and is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | See [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html). |
| type | xsd:string (attribute) | N | Reference to a value in a SOAP web services only system list. If the type is known by context, the type is NOT required. |
| name | xsd:string | N | This is a read-only field that is populated by NetSuite when it's a part of a get or search response. If this field is populated during a write operation, it will be ignored. |

## CustomRecordRef {#bridgehead_N3454996}

The CustomRecordRef type is used to reference any existing custom record in NetSuite. The CustomRecordRef type descends from BaseRef and is defined in core.xsd.

Important:

Setting the RecordRef.type to **customRecord** on an add does NOT return a CustomRecord. You must use CustomRecordRef. The CustomRecordRef has a typeId to indicate which kind of CustomRecord it is.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | References the primary record internal Id. This Id corresponds to the type of custom record. For a list of possible values, see [ListOrRecordRef](#bridgehead_N3455299). |
| typeId | xsd:string | Y | References the custom record type Id. |
| type | xsd:string (attribute) | N | Reference to a value in a SOAP web services only system list. |
| name | xsd:string | N |  |

## ListOrRecordRef {#bridgehead_N3455299}

The listOrRecordRef type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | See [Using Internal IDs, External IDs, and References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html). |
| externalId | xsd:string (attribute) | N | Use to reference records by their external ID in select and multi-select custom fields. |
| typeId | xsd:string (attribute) | N | Reference to a value in a SOAP web services only system list. |
| name | xsd:string | N | This is a read-only field that is populated by NetSuite when it's a part of a get or search response. If this field is populated during a write operation, it is ignored. |

Each record type in NetSuite has a corresponding internal ID (or typeId). This internal ID is required when using ListOrRecordRef since the type of record being referenced needs to be specified.

Note:

To update a ListOrRecordRef object, you must use either the internal ID or the external ID in your request. Using the name field only does not update the object.

For example, in the following code a new ListOrRecordRef object is created. The list references a specific Entity record as designated by the internalId of **1011** and specifies that the record is of the type **customer (-2)**. Note that customer records have an internal ID of -2 as shown in the table below.

          `ListOrRecordRef[] fieldNameEntity = new ListOrRecordRef[1]; fieldNameEntity[0] = new ListOrRecordRef(); fieldNameEntity[0].setInternalId("1011");  fieldNameEntity[0].setTypeId("-2");` 
        

## Status {#bridgehead_N3455609}

The Status type contains an array of objects of type StatusDetail. The status type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| statusDetail | StatusDetail \[\] | N | Used to capture the specific details for the status. See [StatusDetail](#bridgehead_N3455809). |
| isSuccesss | xsd:Boolean (attribute) | Y | Indicates whether the status is successful or not. If false, one or more statusDetail objects are populated. |

## StatusDetail {#bridgehead_N3455809}

The StatusDetail type is used to capture the specific details for the status. The statusDetail type is defined in core.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| code | xsd:string | Y | The status code. See [SOAP Web Services Error Handling and Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3536378.html) for a listing of codes. |
| message | xsd:string | Y | The detailed message for this status. See [SOAP Web Services Error Handling and Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3536378.html) for details. |
| type | xsd:string |  | Reference to a value in a SOAP web services only system list. Values: error, warning See [SOAP Web Services Error Handling and Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3536378.html) for details. |

## NullField {#bridgehead_N3456068}

The NullField type is defined in core.xsd. It contains the following fields.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| name | xsd:string | Y | Name of the field to be null. The specified name must exactly match an existing field name. |

Note:

You cannot set the Custom Form field to NULL. Any request to set this field to NULL is ignored.

## ReadResponse {#bridgehead_N3456218}

The ReadResponse type is used by the following read operations.

-   The getResponse output message for the get operation.
    
-   The searchResponse output message for the search operations.
    

These types have a field named readResponse of the type ReadResponse. The ReadResponse type is defined in message.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| status | Status | Y |  |
| recordRef | RecordRef | N |  |

## ListReadResponse {#bridgehead_N3457524}

The ListReadResponse type is used by the following operations.

-   The GetListResponse output message for the getList operation.
    

These types have a field named response of type ListReadResponse. The ListReadResponse type is defined in message.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| response | ReadResponse\[\] | Y | An array of ReadResponse types. |

## ListWriteResponse {#bridgehead_N3457683}

The ListWriteResponse type is used by the following operations.

-   The AddListResponse output message for the addList operation.
    
-   The UpdateListResponse output message for the updateList operation.
    
-   The DeleteListResponse output message for the deleteList operation.
    

These types have a field named response of type ListWriteResponse. The ListWriteResponse type is defined in message.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| response | WriteResponse\[\] | Y | An array of WriteResponse types. |

## WriteResponse {#bridgehead_N3457857}

The WriteResponse type is used by the following operations:

-   The AddResponse output message for the add operation
    
-   The UpdateResponse output message for the update operation
    
-   The DeleteResponse output message for the delete operation
    

These types have a field named writeResponse of type WriteResponse. The WriteResponse type is defined in message.xsd.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| status | Status | Y |  |
| recordRef | RecordRef | N |  |

### Related Topics

-   [Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html)
-   [Built-in Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452691.html)
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html)
-   [Search Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html)
-   [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
