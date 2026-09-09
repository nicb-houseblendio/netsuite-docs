---
id: "section_N3531763"
type: "section"
title: "updateInviteeStatusList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > updateInviteeStatusList"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3531763.html"
anchors: ["bridgehead_N3531786", "bridgehead_N3532106", "bridgehead_N3532221", "bridgehead_N3532297", "bridgehead_N27332681", "bridgehead_N27332741", "bridgehead_N3532327"]
sha256: "de7161884afbfc5cd025f4f657c961558e81db896a8de4349fe195b042c9d31f"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The updateInviteeStatusList operation is used to update one or more NetSuite events. For general details on the updateInviteeStatus operation, see [updateInviteeStatus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3531056.html).

## Request {#bridgehead_N3531786}

The UpdateInviteeStatusListRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| updateInviteeStatusReference\[\] | UpdateInviteeStatusReference | UpdateInviteeStatusReference uniquely identifies the event and the status you want to update the event with. |

The UpdateInviteeStatusReference type includes the following elements:

-   eventId
    
-   responseCode
    

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| eventId | RecordRef | References an existing instance of an Event record. |
| responseCode | CalendarEventAttendeeResponse | The CalendarEventAttendeeResponse type includes the following enums:
\_accepted

\_declined

\_tentative

\_noResponse



 |

## Response {#bridgehead_N3532106}

The UpdateInviteeStatusListResponse type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response\[\] | WriteResponse | Contains an array of WriteResponse objects, each of which contains details on the status of that updateInviteeStatusList operation and a reference to each event record. |

## Faults {#bridgehead_N3532221}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3532297}

## C# {#bridgehead_N27332681}

          `UpdateInviteeStatusReference [] inviteeStatusRefList = new UpdateInviteeStatusReference[2];                   for (int i=0; i<2; i++)                      {                         RecordRef eventIdRef = new RecordRef();                          if (i==0)                            eventIdRef.internalId = '100';                          else                            eventIdRef.internalId = '101';                            UpdateInviteeStatusReference statusRef = new UpdateInviteeStatusReference();                             statusRef.eventId = eventIdRef;                             statusRef.responseCode = CalendarEventAttendeeResponse._accepted;                             inviteeStatusRefList[i] = statusRef;                      }                               nss.updateInviteeStatusList(inviteeStatusRefList);` 
        

## SOAP Request {#bridgehead_N27332741}

          `<updateInviteeStatusList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <updateInviteeStatusReference>                <eventId internalId="100" xmlns="urn:core_2017_1.platform.webservices.netsuite.com" />                <responseCode xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_accepted       </responseCode>             </updateInviteeStatusReference>             <updateInviteeStatusReference>                <eventId internalId="101" xmlns="urn:core_2017_1.platform.webservices.netsuite.com" />                <responseCode xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_accepted       </responseCode>             </updateInviteeStatusReference>          </updateInviteeStatusList>` 
        

## SOAP Response {#bridgehead_N3532327}

          `<updateInviteeStatusListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponseList>                <writeResponse>                   <platformCore:status isSuccess="true"           xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <baseRef internalId="100" type="calendarEvent" xsi:type="platformCore:RecordRef"           xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                </writeResponse>                <writeResponse>                   <platformCore:status isSuccess="true"            xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                   <baseRef internalId="101" type="calendarEvent" xsi:type="platformCore:RecordRef"          xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                </writeResponse>             </writeResponseList>          </updateInviteeStatusListResponse>` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
