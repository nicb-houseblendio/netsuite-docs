---
id: "section_N3539420"
type: "section"
title: "SOAP Fault Status Codes"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Error Handling and Error Codes > SOAP Fault Status Codes"
parent: "chapter_N3536378"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html"
anchors: []
sha256: "fbe955628fc15973235d53095767102bfe0de337c0816956cfe0a2d84187d98f"
---

The following table defines SOAP fault types and their corresponding codes. For a complete description of faults and how they differ from errors and warnings, refer to [SOAP Web Services Warnings, Errors, and Faults](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536574.html).

| Fault Name | Description |
| --- | --- |
| InsufficientPermissionFault | This fault is thrown when the client does not have the appropriate permissions to perform an action based on the role under which they are currently logged in. If the client (user) has more than one role, they may need to login again supplying a different role with more permissions. |
| InvalidAccountFault | This fault is thrown when the client attempts to login with an invalid account id. |
| InvalidPartnerCredentials | Partner ID or password submitted with this request is invalid. |
| InvalidRequestIP | Originating IP is not one of the registered IPs from which this Partner request may arrive. |
| InvalidSessionFault | This fault can be thrown when the client's session has timed out or was terminated as the result of a second SOAP web services client establishing another session. The fault message occurs on the first request attempted after the session is terminated/timed out. For more details on how NetSuite handles sessions, see [Session Management for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html). |
| InvalidVersionFault | This fault is thrown in the event that the request message contains an unsupported version of the schema. |
| ExceededConcurrentRequestLimitFault | This fault is thrown in the event that the maximum number of concurrent requests has been reached. |
| ExceededRecordCountFault | This fault is thrown in the event the maximum number of records allowed for an operation has been exceeded. For more information, see [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html). |
| ExceededRequestLimitFault | This fault is thrown if the allowed number of concurrent requests is exceeded. For more information, see [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html). |
| ExceededRequestSizeFault |  |
| ExceededUsageLimitFault |  |
| UnexpectedErrorFault | This fault is thrown in the event of an occurrence of an unexpected exception. |
| InvalidCredentialsFault | This fault is thrown in the event of an invalid username (e-mail), password, role, or application ID. This fault is also thrown if two-factor authentication is required but is missing. |
| AsyncFault |  |

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Warnings, Errors, and Faults](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536574.html)
-   [SOAP Faults for Each Operation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536956.html)
-   [Error Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539978.html)
-   [Warning Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3599699.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
