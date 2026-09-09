---
id: "section_N3481947"
type: "section"
title: "attach / detach"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > attach / detach"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html"
anchors: ["bridgehead_N3483603", "bridgehead_N3483718", "bridgehead_N3483834", "bridgehead_N3483949", "bridgehead_N3484064", "bridgehead_N3484140", "bridgehead_3705185967", "bridgehead_3705186254", "bridgehead_3705186602", "bridgehead_3705186925", "bridgehead_3705187153", "bridgehead_N3484226"]
sha256: "f6fbdc23cf2aea681cccbaa905d27bfe655faab7fcdf86e9b5557a852632e155"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The attach and detach operations can be used to define or remove a relationship between two records. For example, a Contact record can be associated with a Partner record, or an Opportunity record can be associated with a Customer record.

Important:

A user error is thrown if you attempt to attach files or records that do not exist.

You can also use the attach / detach operations to attach or detach a file to or from a record. Any file that is in the NetSuite File Cabinet, for example an MS Word or Excel file or a PDF can be attached to any record other than a custom record.

Note that when attaching Contacts to other entity records, the Contact's role can also be specified during the request. Contact Roles are roles available in a user defined list at _List > Relationships > Contacts_. This list has been exposed as ContactRole in accounting.xsd.

Note that to prevent duplicate records, you should use the alternate upsert and upsertList operations along with external ids to add records to NetSuite.

Note:

Contact records can be attached to all entity records expect for other Contact or Group records.

The following table lists all records that support the attach/detach operations. It also lists which records can accept file attachments as well as which records can accept Contact records as attachments.

| Record Type | Accepts File Attachments | Accepts Contact Record Attachments |
| --- | --- | --- |
| **Transactions** |
| Check | X | X |
| Custom Transaction | X |  |
| Expense Report | X |  |
| Inventory Adjustment | X | X |
| Item Fulfillment | X | X |
| Intercompany Transfer Order | X | X |
| Opportunity | X | X |
| Transfer Order | X | X |
| Sales Order | X | X |
| Customer Payment | X | X |
| Return Authorization | X | X |
| Credit Memo | X | X |
| Cash Refund | X | X |
| Estimate | X | X |
| Invoice | X | X |
| Cash Sale | X | X |
| Purchase Order | X | X |
| Requisition | X | X |
| Customer Payment | X | X |
| Customer Refund | X | X |
| Customer Deposit | X | X |
| Vendor Bill | X | X |
| Vendor Credit | X | X |
| Vendor Return Authorization | X | X |
| Work Order | X |  |
| Work Order Issue | X |  |
| Work Order Close | X |  |
| Work Order Completion | X |  |
| **Entities** |
| Customer | X | X |
| Contact | X |  |
| Employee | X |  |
| Partner | X | X |
| Vendor | X | X |
| Project | X | X |
| Group | X | Note: Although you cannot currently attach Contact records to Group, you can attach members to create a static group. |
| **Activities** |
| Task | X |  |
| Event | X |  |
| Phone Call | X |  |
| Project Task | X |  |
| **Support** |
| SupportCase | X |  |
| Issue | X |  |
| **Marketing** |
| Campaign | X |  |

## Request (attach) {#bridgehead_N3483603}

The AttachRequest type is used for this request. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| attachReference | AttachReference |  |

## Request (detach) {#bridgehead_N3483718}

The DetachRequest type is used for this request. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| detachReference | DetachReference |  |

## Response (attach) {#bridgehead_N3483834}

The AttachResponse type is used for this response. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse |  |

## Response (detach) {#bridgehead_N3483949}

The DetachResponse type is used for this response. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| response | WriteResponse |  |

## Faults {#bridgehead_N3484064}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3484140}

## SOAP Request (attach) {#bridgehead_3705185967}

          `<attach xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">      <attachReferece xsi:type="ns1:AttachContactReference"       xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com">           <ns1:attachTo internalId="176" type="customer" xsi:type="ns1:RecordRef">              <ns1:name xsi:type="xsd:string">Adelina Shonkwiler</ns1:name>               </ns1:attachTo>            <ns1:contact internalId="1467" xsi:type="ns1:RecordRef"/>              <ns1:contactRole internalId="-10" xsi:type="ns1:RecordRef">                  <ns1:name xsi:type="xsd:string">Primary Contact</ns1:name>               </ns1:contactRole>       </attachReferece>    </attach>` 
        

## SOAP Request (detach) {#bridgehead_3705186254}

          `<detach xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <detachReferece xsi:type="ns1:DetachBasicReference"          xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com">               <ns1:detachFrom internalId="176" type="customer" xsi:type="ns1:RecordRef">                 <ns1:name xsi:type="xsd:string">Adelina Shonkwiler</ns1:name>                    </ns1:detachFrom>        <ns1:detachedRecord internalId="1467" type="contact" xsi:type="ns1:RecordRef"/>         </detachReferece>    </detach>` 
        

## SOAP Response (attach) {#bridgehead_3705186602}

          `<attachResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">     <writeResponse>       <ns1:status isSuccess="true"             xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>            <baseRef internalId="176" type="customer" xsi:type="ns2:RecordRef"                   xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">                <ns2:name>Adelina Shonkwiler</ns2:name>             </baseRef>      </writeResponse>  </attachResponse>` 
        

## SOAP Response (detach) {#bridgehead_3705186925}

          `<detachResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <writeResponse>      <ns1:status isSuccess="true"          xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>         <baseRef internalId="176" type="customer" xsi:type="ns2:RecordRef"                xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">              <ns2:name>Adelina Shonkwiler</ns2:name>           </baseRef>    </writeResponse> </detachResponse>` 
        

## Java (attach operation) {#bridgehead_3705187153}

          `public void attach() throws Exception     {         RecordRef contactRef = new RecordRef();         contactRef.setInternalId("1467");         contactRef.setType(RecordType.contact);           RecordRef contactRoleRef = new RecordRef();         contactRoleRef.setInternalId("-10");         contactRoleRef.setName("Primary Contact");           RecordRef customerRef = new RecordRef();         customerRef.setInternalId("176");         customerRef.setType(RecordType.customer);           AttachContactReference attachRef = new AttachContactReference();         attachRef.setContact(contactRef);         attachRef.setAttachTo(customerRef);         attachRef.setContactRole(contactRoleRef);           WriteResponse attachResponse = sessMgr.getPort().attach(attachRef);     }` 
        

## Java (detach operation) {#bridgehead_N3484226}

          `public void detach() throws Exception     {         RecordRef contactRef = new RecordRef();         contactRef.setInternalId("1467");         contactRef.setType(RecordType.contact);           RecordRef customerRef = new RecordRef();         customerRef.setInternalId("176");         customerRef.setType(RecordType.customer);           AttachContactReference detachRef = new AttachContactReference();         detachRef.setContact(contactRef);         detachRef.setAttachTo(customerRef);           WriteResponse detachResponse = sessMgr.getPort().detach(detachRef);     }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
