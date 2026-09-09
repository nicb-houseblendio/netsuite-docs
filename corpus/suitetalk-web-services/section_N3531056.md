---
id: "section_N3531056"
type: "section"
title: "updateInviteeStatus"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > updateInviteeStatus"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3531056.html"
anchors: ["bridgehead_N3531219", "bridgehead_N3531405", "bridgehead_N3531522", "bridgehead_N3531597", "bridgehead_N27327031", "bridgehead_N27327091", "bridgehead_N3531627"]
sha256: "d7b337ecf28b0994e3b90f59331e4ce4b9acc059b0f5b848b9d4cdc940730dc7"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The updateInviteeStatus operation lets users respond to NetSuite events that have been sent to them. This operation takes both the internal ID of the event as well as a calendar event status as arguments.

After invitees have responded to the event invitation, the Event record is updated with their response. Possible responses include accepted, declined, tentative, and noResponse.

Note the following:

-   For information about the Event record in SOAP web services, see [Events (CalendarEvent)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650565.html). For general information about scheduling events in NetSuite, see [Scheduling Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501467.html).)
    
-   There is no async equivalent for the updateInviteeStatus operation.
    

Note the following when using this operation:

-   Users must have a valid session. This operation includes a **passport** header to support request level credentials. (For information about request level authentication, see [Request-Level Credentials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489690806.html#bridgehead_N3447228).)
    
-   To update other properties on the Event record, the event owner should still use the [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) operation. Note, however, event owners are not exempt from using updateInviteeStatus if they have to update their own event response status. There may be cases in which event owners must decline their own event and have another person run the event for them.
    
-   Unlike in the NetSuite UI, invitees will not be able to send a message back to the organizer. SOAP web services does not currently support messages attached to events. An event invitee's response can include only one of the following values: \_accepted, \_declined, \_tentative, \_noResponse.
    

## Request {#bridgehead_N3531219}

The UpdateInviteeStatusRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| eventId | RecordRef | References an existing instance of an Event record. |
| responseCode | CalendarEventAttendeeResponse | The CalendarEventAttendeeResponse type includes the following enums:
\_accepted

\_declined

\_tentative

\_noResponse



 |

## Response {#bridgehead_N3531405}

The UpdateInviteeStatusResponse type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse | Contains details on the status of the operation and a reference to the updated record. |

## Faults {#bridgehead_N3531522}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3531597}

## C# {#bridgehead_N27327031}

          `NetSuiteService nss = new NetSuiteService(); // login details omitted  UpdateInviteeStatusReference inviteeStatusRef = new UpdateInviteeStatusReference();  // Set the event id for the status update RecordRef eventIdRef  = new RecordRef(); eventIdRef.internalId = '100';   // Substitute this with your own event id inviteeStatusRef.eventId = eventIdRef;  // Set the event status inviteeStatusRef.responseCode = CalendarEventAttendeeResponse._accepted;  // Update invitee event status WriteResponse resp = nss.updateInviteeStatus(inviteeStatusRef);` 
        

## SOAP Request {#bridgehead_N27327091}

          `<updateInviteeStatus xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <updateInviteeStatusReference>                <eventId internalId="100" xmlns="urn:core_2017_1.platform.webservices.netsuite.com" />                <responseCode xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_accepted       </responseCode>             </updateInviteeStatusReference>          </updateInviteeStatus>` 
        

## SOAP Response {#bridgehead_N3531627}

          `<updateInviteeStatusResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true"                   xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef internalId="100" type="calendarEvent" xsi:type="platformCore:RecordRef"       xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>          </updateInviteeStatusResponse>` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
