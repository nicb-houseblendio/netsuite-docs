---
id: "section_N3497592"
type: "section"
title: "getDeleted"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getDeleted"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html"
anchors: ["bridgehead_4253085370", "bridgehead_4256588742", "bridgehead_N3497624", "bridgehead_N3497747", "bridgehead_N3497904", "bridgehead_N3498056", "bridgehead_N3498131", "bridgehead_3705203445"]
sha256: "14642deb0c73d5e07620dc90eaa7482cda8613bdc06ea644300c87ff06ee09e6"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

You use the getDeleted operation to retrieve a list of deleted records. When you use this operation, you can filter by record type, by script ID, and by the date of record deletion. For each record that matches the filter criteria, the system returns the following data:

-   The record's type
    
-   The record's name
    
-   The record's internal ID
    
-   The record's external ID (if avalaible)
    
-   The date the record was deleted
    

The getDeleted operation can be useful when you want to synchronize information in a client application with NetSuite. For example, an Outlook client application plug-in maintains a list of contacts and synchronizes that list with NetSuite. The getDeleted operation can be used to determine contact deletions since the last synchronization with NetSuite.

## Permissions {#bridgehead_4253085370}

By default, only account administrators and users with the Full Access role have permission to use the getDeleted operation. However, you can grant permission to other roles. To use the getDeleted operation, the role has to have the Deleted Records permission (and the Web Services permission).

Users who have the Deleted Records permission can access results about any type of record that was deleted, even if they do not have permission to create or modify that record type. They also have permission to use the Deleted Record search type in the user interface, unless the Web Services Only option has been selected for the role.

You can give a role the Deleted Records permission by going to _Setup > Users/Roles > Manage Roles_. Go to the Permissions > Setup subtab, and add a line for the permission.

## Usage Notes {#bridgehead_4256588742}

Note the following:

-   Not all record types support the getDeleted operation. For a complete list of supported record types for this operation, refer to the DeletedRecordType enumeration in the [coreTypes](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd) xsd.
    
-   Data about deleted records remains available indefinitely.
    
-   The getDeleted response does not differentiate between records deleted through SOAP web services and through the UI.
    
-   Even though it is not a search, the getDeleted operation respects the pageSize search preference.
    
-   The getDeleted operation changed in 2015.1. If you are using the 2014.2 endpoint or earlier, refer to the Platform Guide for your WSDL version. To obtain an older version of the platform guide, see [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html).
    

## Request {#bridgehead_N3497624}

The GetDeletedRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| getDeletedFilter | GetDeletedFilter | See [GetDeletedFilter](#bridgehead_N3497747). |
| pageIndex | xsd: int | Use this argument to specify which page of results to return in your response. If there is only one page of results, enter 1. |

## GetDeletedFilter {#bridgehead_N3497747}

The GetDeletedFilter lets you retrieve data based on the date, record type, and script ID of the deleted records.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| deletedDate | SearchDateField | The date that the record was deleted. For example, you can search for records that were deleted since a particular date or between two dates. |
| type | SearchEnumMultiSelectField | The type of the record that was deleted. For a complete list of all of the values currently supported by the getDeleted operation, refer to the DeletedRecordType enumerations in the [coreTypes XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd). |
| scriptID | SearchStringField | The scriptID identifying the specific custom record or custom transaction type. Use this field to narrow the results to custom records (or custom transactions) **only** of that particular type. If you do not specify a script ID, and rely only on the type field, the operation returns details on all instances that were deleted, regardless of type. |

## Response {#bridgehead_N3497904}

The DeletedRecord type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| totalRecords | xsd: int | The total number of records that meet the filter criteria. |
| pageSize | xsd: int | The total number of records listed on each page of the results. |
| totalPages | xsd: int | The total number of available pages. |
| pageIndex | xsd: int | The number identifying the current page of results. |
| deletedRecordList | deletedRecordList | A list of records that meet the filter criteria |

## Faults {#bridgehead_N3498056}

This operation can throw any of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3498131}

The following sample shows how to retrieve details about deleted instances of a custom record type with the script ID customrecord1. It specifies that 10 results should be returned per page, and it includes logic to retrieve all pages.

## Java {#bridgehead_3705203445}

          `{    c.setSearchPrefsPageSize(10);     GetDeletedFilter filter = new GetDeletedFilter();    filter.setType(new SearchEnumMultiSelectField(new String[] {DeletedRecordType._customRecord}, SearchEnumMultiSelectFieldOperator.anyOf));    filter.setScriptId(new SearchStringField("customrecord1", SearchStringFieldOperator.is));     GetDeletedResult result;       int i = 1;       do       {          result = c.m_port.getDeleted(filter, i);          if (i == 1)          {             System.out.println(String.format("Page Size : %d, Total Pages : %d, Total Records : %d", result.getPageSize(), result.getTotalPages(), result.getTotalRecords()));          }          processDeletedRecordList(result.getDeletedRecordList());          System.out.println(String.format("Current Page Index : %d", result.getPageIndex()));          i++;       }       while (i <= result.getTotalPages()); }` 
        

### Related Topics

-   [Searching for Deleted Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4031815869.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
