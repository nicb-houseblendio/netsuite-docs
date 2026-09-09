---
id: "section_N3485424"
type: "section"
title: "changePassword"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > changePassword"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3485424.html"
anchors: ["bridgehead_N3485486", "bridgehead_N3485638", "bridgehead_N3485650", "bridgehead_N3485725", "bridgehead_3705189319", "bridgehead_3705431690", "bridgehead_3705189546"]
sha256: "413b1586637e489b87366056324f0e08ee6fe0ce441037094ed4baa39d0ed0bf"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Use the changePassword operation to change a user's NetSuite password.

This topic provides details about how to change a user's password with SOAP web services code. For details about how to make this change in the NetSuite user interface, see [Change Password Link](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N487604.html) and [Your User Credentials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N485109.html).

## Request {#bridgehead_N3485486}

The ChangePasswordRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| changePassword | ChangePassword |  |

The ChangePassword type takes the following fields:

-   currentPassword
    
-   newPassword
    
-   newPassword2
    

## Response {#bridgehead_N3485638}

The ChangePasswordResponse type is used for the response. It does not contain any fields.

## Faults {#bridgehead_N3485650}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InsufficientPermissionFault
    
-   InvalidAccountFault
    
-   InvalidCredentialsFault
    
-   InvalidVersionFault
    
-   ExceededRequestLimitFault
    
-   UnexpectedErrorFault
    
-   UserError
    

## Sample Code {#bridgehead_N3485725}

## SOAP Request {#bridgehead_3705189319}

          `<soapenv:Body>            <changePassword xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <changePassword>                    <ns6:currentPassword xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">password1</ns6:currentPassword>                    <ns7:newPassword xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">password2</ns7:newPassword>                    <ns8:newPassword2 xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">password2</ns8:newPassword2>                </changePassword>            </changePassword>        </soapenv:Body>` 
        

## SOAP Response {#bridgehead_3705431690}

          `<soapenv:Body>          <changePasswordResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <sessionResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </sessionResponse>          </changePasswordResponse>       </soapenv:Body>` 
        

## Java {#bridgehead_3705189546}

          `ChangePassword changePW = new ChangePassword(); changePW.setCurrentPassword("password1"); changePW.setNewPassword("password2"); changePW.setNewPassword2("password2");   c.getPort().changePassword(changePW);` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
