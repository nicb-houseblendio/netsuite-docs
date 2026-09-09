---
id: "section_N3449174"
type: "section"
title: "Operations and Their Internal ID Requirements"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Platform Features > Operations and Their Internal ID Requirements"
parent: "chapter_N3448700"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3449174.html"
anchors: ["bridgehead_N3451691", "bridgehead_3705126032", "bridgehead_3705126439", "bridgehead_N3451740", "bridgehead_3705126682", "bridgehead_3705126939", "bridgehead_N3451775", "bridgehead_3705180760", "bridgehead_3705180947", "bridgehead_N3451810", "bridgehead_3705431081", "bridgehead_3705181304", "bridgehead_N3451845", "bridgehead_3705181798", "bridgehead_3705182048"]
sha256: "d41c71fc27930d0d14d14408ff2038cd8b60d28f08c405ea8afab830f4585ae2"
---

The following table lists the ID requirements for each operation. Note that IDs are only required in calls where specific records corresponding to the call exist in the NetSuite database. For example, on an add operation, no ID is required in the request since the record does not yet exist.

An internal ID is created by the system and returned in the response. On search operations, because a specific record is not being called, an internal ID is not required in the request. However, an internal ID for each record found is returned in the response.

Note:

Since external IDs are provided by the client application, if an external ID is desired for a record, it can be submitted on an Add operation.

| Operation | Record ID Required in Request | Record ID Returned in Response |
| --- | --- | --- |
| login | \- | \- |
| logout | \- | \- |
| add/addList | No | Yes |
| update/updateList | Yes | Yes |
| delete/deleteList | Yes | Yes |
| getDeleted | No | Yes |
| get/getList | Yes | Yes |
| getAll | No | Yes |
| search/searchNext/searchMore/searchMoreWithId | No | Yes |
| getSavedSearch | No | Yes |

The following samples show the use of internal IDs as they pertain to operations. Click to see samples for any of the following:

-   [add operation](#bridgehead_N3451691)
    
-   [update operation](#bridgehead_N3451740)
    
-   [deleteList operation](#bridgehead_N3451775)
    
-   [getList operation](#bridgehead_N3451810)
    
-   [search operation](#bridgehead_N3451845)
    

## add operation {#bridgehead_N3451691}

For an add operation, an internal ID is _not_ required in the request since the record does not yet exist. The internal ID (in this case 100101) is returned in the response.

Note:

There are internal IDs listed in the request, but these internal IDs are _embedded_ in the request and do not correspond to the record being added (an event) but to other existing records associated with the event record being added.

## Request {#bridgehead_3705126032}

          `<soap:Body> <platformMsgs:add>    <platformMsgs:record xsi:type="actSched:CalendarEvent">       <actSched:title>Web Services Meeting</actSched:title>       <actSched:organizer internalId="-5" type="calendarEvent" xsi:type="platformCore:RecordRef">          <platformCore:name>Mr. Wolfe</platformCore:name>       </actSched:organizer>       <actSched:location>Main Conference Room</actSched:location>       <actSched:attendeeList replaceAll="true" xsi:type="actSched:CalendarEventAttendeeList">          <actSched:attendee xsi:type="actSched:CalendarEventAttendee">             <actSched:sendEmail>false</actSched:sendEmail>             <actSched:attendee internalId="21" type="calendarEvent"              xsi:type="platformCore:RecordRef"/>             <actSched:response>_accepted</actSched:response>             <actSched:attendance>_optional</actSched:attendance>          </actSched:attendee>          <actSched:attendee xsi:type="actSched:CalendarEventAttendee">             <actSched:sendEmail>false</actSched:sendEmail>             <actSched:attendee internalId="27" type="calendarEvent"              xsi:type="platformCore:RecordRef"/>             <actSched:response>_accepted</actSched:response>             <actSched:attendance>_optional</actSched:attendance>          </actSched:attendee>       </actSched:attendeeList>    </platformMsgs:record> </platformMsgs:add> </soap:Body>` 
        

## Response {#bridgehead_3705126439}

          `<soapenv:Body>    <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="100101" type="calendarEvent" xsi:type="ns2:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </addResponse> </soapenv:Body>` 
        

## update operation {#bridgehead_N3451740}

In this example the record added above is being updated - since the internal ID matches the one created in the add operation (100101). Here, the internal ID and the record type are required in the request and both are also returned in the response.

## Request {#bridgehead_3705126682}

          `<soap:Body>    <platformMsgs:update>       <platformMsgs:record internalId="100101" xsi:type="actSched:CalendarEvent">          <actSched:title>Web Services Meeting (Platform)</actSched:title>       </platformMsgs:record>    </platformMsgs:update> </soap:Body>` 
        

## Response {#bridgehead_3705126939}

          `<soapenv:Body>    <updateResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef internalId="100101" type="calendarEvent" xsi:type="ns2:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </updateResponse> </soapenv:Body>` 
        

## deleteList operation {#bridgehead_N3451775}

In the following delete request, the internal IDs are required for the request and returned in the response. In this case, three event records are deleted (100101, 100102, and 100103).

## Request {#bridgehead_3705180760}

          `<soap:Body> <platformMsgs:deleteList>    <platformMsgs:baseRef internalId="100101" type="calendarEvent" xsi:type="platformCore:RecordRef"/>    <platformMsgs:baseRef internalId="100102" type="calendarEvent" xsi:type="platformCore:RecordRef"/>    <platformMsgs:baseRef internalId="100103" type="calendarEvent" xsi:type="platformCore:RecordRef"/> </platformMsgs:deleteList> </soap:Body>` 
        

## Response {#bridgehead_3705180947}

          `<soapenv:Body> <deleteListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponseList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <writeResponse>       <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="100101" type="calendarEvent" xsi:type="ns2:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse>    <writeResponse>       <ns3:status isSuccess="true" xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="100102" type="calendarEvent" xsi:type="ns4:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse>    <writeResponse>       <ns5:status isSuccess="true" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>       <baseRef internalId="100103" type="calendarEvent" xsi:type="ns6:RecordRef"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com"/>    </writeResponse> </writeResponseList> </deleteListResponse> </soapenv:Body>` 
        

## getList operation {#bridgehead_N3451810}

In this example, an internal ID is called for each record to be retrieved - in this case, three different event records. Again, the internal ID is required for the request and returned in the response.

## Request {#bridgehead_3705431081}

          `<soap:Body> <platformMsgs:getList>    <platformMsgs:baseRef internalId="100104" type="calendarEvent" xsi:type="platformCore:RecordRef"/>    <platformMsgs:baseRef internalId="100105" type="calendarEvent" xsi:type="platformCore:RecordRef"/>    <platformMsgs:baseRef internalId="100106" type="calendarEvent" xsi:type="platformCore:RecordRef"/> </platformMsgs:getList> </soap:Body>` 
        

## Response {#bridgehead_3705181304}

          `<soapenv:Body> <getListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <readResponseList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <readResponse>    <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>    <record internalId="100104" xsi:type="ns2:CalendarEvent"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"     xmlns:ns2="urn:scheduling_2017_1.activities.webservices.netsuite.com">       <ns2:title>Customization Meeting</ns2:title>       <ns2:organizer internalId="-5">       .........[more fields]    </record> </readResponse> <readResponse>    <ns8:status isSuccess="true" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>    <record internalId="100105" xsi:type="ns9:CalendarEvent"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"     xmlns:ns9="urn:scheduling_2017_1.activities.webservices.netsuite.com">       <ns9:title>Web Services Meeting (Records)</ns9:title>       <ns9:organizer internalId="-5">       .........[more fields]    </record> </readResponse> <readResponse>    <ns15:status isSuccess="true" xmlns:ns15="urn:core_2017_1.platform.webservices.netsuite.com"/>    <record internalId="100106" xsi:type="ns16:CalendarEvent"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"     xmlns:ns16="urn:scheduling_2017_1.activities.webservices.netsuite.com">       <ns16:title>Web Services Meeting</ns16:title>       <ns16:organizer internalId="-5">       .........[more fields]    </record> </readResponse> </readResponseList> </getListResponse> </soapenv:Body>` 
        

## search operation {#bridgehead_N3451845}

For the search operation, an internal ID is not required for the request but is returned for each record found that matches the specified criteria. In this case, two event records are returned for a search request calling for each event record that contains **web services** in the title field.

## (Request) {#bridgehead_3705181798}

          `<soap:Body> <platformMsgs:search>    <platformMsgs:searchRecord xsi:type="actSched:CalendarEventSearch">       <actSched:title operator="contains" xsi:type="platformCore:SearchStringField">          <platformCore:searchValue>web services</platformCore:searchValue>       </actSched:title>    </platformMsgs:searchRecord> </platformMsgs:search> </soap:Body>` 
        

## (Response) {#bridgehead_3705182048}

          `<soapenv:Body> <searchResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <searchResult xmlns="urn:core_2017_1.platform.webservices.netsuite.com">    <status isSuccess="true"/>    <totalRecords>2</totalRecords>    <pageSize>10</pageSize>    <totalPages>1</totalPages>    <pageIndex>1</pageIndex>    <recordList>       <record internalId="100105" xsi:type="ns1:CalendarEvent"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns1="urn:scheduling_2017_1.activities.webservices.netsuite.com">          <ns1:title>Web Services Meeting (Records)</ns1:title>          <ns1:organizer internalId="-5">          .....[more fields]       </record>       <record internalId="100106" xsi:type="ns2:CalendarEvent"        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"        xmlns:ns2="urn:scheduling_2017_1.activities.webservices.netsuite.com">          <ns2:title>Web Services Meeting</ns2:title>          <ns2:organizer internalId="-5">          .....[more fields]       </record>    </recordList> </searchResult> </searchResponse> </soapenv:Body>` 
        

### Related Topics

-   [Platform Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3448700.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [Enabling Web Services Concurrent Users with SuiteCloud Plus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448861.html)
-   [Using SOAP web services to Send Data from a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4488980213.html)
-   [Searching for SOAP Web Services Log Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738049812.html)
-   [SOAP Web Services Operations Search Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738050787.html)
-   [SOAP Web Services Record Processing Search Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738051114.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
