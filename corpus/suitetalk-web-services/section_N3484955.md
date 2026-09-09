---
id: "section_N3484955"
type: "section"
title: "changeEmail"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > changeEmail"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3484955.html"
anchors: ["bridgehead_N3485020", "bridgehead_N3485171", "bridgehead_N3485183", "bridgehead_N3485258", "bridgehead_3705188573", "bridgehead_3705188794", "bridgehead_3705189037"]
sha256: "65e0b314fe46b3382cccbb3cecd08f344a48bd8e86ed3745f0fdb522e72ad0db"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Use the changeEmail operation to change a user's email address.

This topic provides details about how to change a user's email address with SOAP web services code. For details about how to make this change in the NetSuite user interface, see [Change Email Link](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N487532.html) and [Your User Credentials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N485109.html).

Important:

This operation is supported as of the 2012.2 endpoint. The 2012.2 and later endpoints support changeEmail and [changePassword](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3485424.html) operations.

Important:

Be aware that a user's email address is not changed immediately. The old email address remains in effect until the new email address is validated by the user, through a validation link sent to the new address. A notification is also sent to the old address. This behavior is the same as when users change their email addresses through the user interface.

## Request {#bridgehead_N3485020}

The ChangeEmailRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| changeEmail | ChangeEmail |  |

The ChangeEmail type takes the following fields:

-   currentPassword
    
-   newEmail
    
-   newEmail2
    
-   justThisAccount
    

## Response {#bridgehead_N3485171}

The ChangeEmailResponse type is used for the response. It does not contain any fields.

## Faults {#bridgehead_N3485183}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InsufficientPermissionFault
    
-   InvalidAccountFault
    
-   InvalidCredentialsFault
    
-   InvalidVersionFault
    
-   ExceededRequestLimitFault
    
-   UnexpectedErrorFault
    
-   UserError
    

## Sample Code {#bridgehead_N3485258}

## SOAP Request {#bridgehead_3705188573}

          `<changeEmail xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <changeEmail>           <ns6:currentPassword xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">xxxxxxx</   ns6:currentPassword>           <ns7:newEmail xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">newEmail@tester.com</ns7:newEmail>           <ns8:newEmail2 xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"> newEmail @tester.com</ns8:newEmail2>           <ns9:justThisAccount xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">true</ns9:justThisAccount>       </changeEmail>   </changeEmail>` 
        

## SOAP Response {#bridgehead_3705188794}

          `<changeEmailResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">               <sessionResponse>                      <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </sessionResponse> </changeEmailResponse>` 
        

## Java {#bridgehead_3705189037}

          `public void test_ChangeEmail() throws Exception {    sessMgr.loginWithEmail("oldEmail@ws.com");    ChangeEmail c = new ChangeEmail();    c.setCurrentPassword("xxxxxx");    c.setNewEmail("newEmail@ws.com");    c.setNewEmail2("newEmail@ws.com");    c.setJustThisAccount(true);    sessMgr.getPort().changeEmail(c);    sessMgr.loginWithEmail("newEmail@ws.com"); }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
