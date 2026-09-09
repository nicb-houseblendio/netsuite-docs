---
id: "section_N3493817"
type: "section"
title: "getCustomizationId"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getCustomizationId"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3493817.html"
anchors: ["bridgehead_N3493985", "bridgehead_N3494036", "bridgehead_N3494223", "bridgehead_N3494410", "bridgehead_N3494486", "bridgehead_3705199163", "bridgehead_3705199430", "bridgehead_3705200038", "bridgehead_3705199704", "bridgehead_3705200385", "bridgehead_1535368250", "bridgehead_1535368448", "bridgehead_1520864992"]
sha256: "b5ef7d15c7d84df115f8c0651503401c9a0fdc1a7b3e9aefb94840e73432a64e"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

When integrating with NetSuite through SOAP web services, in many cases, you will want to know which custom objects exist in an account. You may also want to obtain metadata for these custom objects so that your application can handle any business logic that is specific to the account.

To learn which custom objects exist in an account, use the getCustomizationId operation to retrieve the internalIds, externalIds, and scriptIds of all custom objects of a specified type. These types, enumerated in CustomizationType, include the following:

-   crmCustomField
    
-   customList
    
-   customRecordType
    
-   customRecordCustomField
    
-   customSegment
    
-   entityCustomField
    
-   itemCustomField
    
-   itemOptionCustomField
    
-   otherCustomField
    
-   transactionBodyCustomField
    
-   transactionColumnCustomField
    

Note:

The CustomizationType object is defined in the [coreTypes XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd).

After the IDs are returned, you can then pass the ID value(s) to either the [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) or [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) operation to obtain metadata for specific custom objects (see [Using get and getList with getCustomizationId](#bridgehead_N3493985) for more details).

Note the following:

-   To see the UI equivalent of a NetSuite custom object, go to Customization > Lists, Records, & Fields > \[custom object type\]. For information about working with each object type in SOAP web services, see [Customization Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html) . For a more general understanding of the NetSuite customization model, see [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html#bridgehead_1491845409).
    
-   Normally, you cannot add or update the internalId of a NetSuite object. Custom objects, however, are an exception to this rule. You can specify the ID on add, but you cannot update the ID thereafter. Also note that internalIds for custom objects can be set to any unique alphanumeric string up to 30 characters long. This string cannot include any spaces, but it can include underscores ( \_ ).
    
-   The getCustomizationId operation also returns fields generated from custom segments. See the SOAP samples at [SOAP Request for Returning Custom Segments](#bridgehead_1535368250).
    

## Using get and getList with getCustomizationId {#bridgehead_N3493985}

If you want only the internalIds, externalIds, and scriptIds for custom objects of a specific type, you can call getCustomizationId on that custom type (for example, crmCustomField). However, if you also want the metadata for any or all of the custom objects referenced in the getCustomizationId response, you must invoke a get or getList request and specify each object's ID.

When using either the get or getList operations in conjunction with getCustomizationId, be aware of the following:

-   If you specify more than one ID in a get | getList call, the IDs you pass are read in the following order: internalId, externalId, scriptId.
    
-   If an invalid scriptId is specified but the internalId or externalId is correct, the scriptId is ignored.
    
-   NetSuite will reject get | getList requests if only a scriptId is passed for record types that do not support scriptIds.
    

## Request {#bridgehead_N3494036}

The getCustomizationIdRequest type is used for this request. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| customizationType | CustomizationType | Any of the custom object types enumerated in CustomizationType. |
| includeInactives | boolean | A value of true or false is required. A value of false means no inactive custom objects are returned in the response. A value of true means that both active and inactive custom objects are returned in the response.
-   To determine which of the returned custom objects are inactive, you must perform either a get or getList operation to obtain the metadata for the custom object type(s). For custom records and custom lists, the value is specified in the **isInactive** element.
-   Although the includeInactives argument is required, the value you set applies to custom record and custom list objects only. In NetSuite, custom fields cannot be set to active or inactive. Therefore, when using getCustomizationId on a custom field type, the value you specify for includeInactives will be ignored. Whether you specify true or false, all custom field objects (of the type specified in your request) will be returned.

 |

## Response {#bridgehead_N3494223}

The getCustomizationIdResult type is used for the response. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| totalRecords | xsd:int | The total number of records for this request. Depending on the pageSize value, some or all the records may be returned in the response. |
| customizationRefList | CustomizationRef | A list of custom objects that correspond to the specified customization type. Also returns the internalId, externalId, and scriptId of each object. |

## Faults {#bridgehead_N3494410}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3494486}

The following sample is a two-part sample. The first part of the sample shows how to construct a getCustomizationId request so that the IDs for all custom record type objects in a NetSuite account are returned. Notice that in the getCustomizationId request, the value of the includeInactives parameter is set to false, meaning that only custom records marked as 'active' in the account will be returned.

The second part of the sample shows how to take internalIds that are returned, and make a getList request to return the metadata for each custom record type.

## C# Sample {#bridgehead_3705199163}

          `NetSuiteService nss = new NetSuiteService();  // credential code ignored here in this sample ...  // Perform getCustomizationId on custom record type CustomizationType ct = new CustomizationType(); ct.getCustomizationTypeSpecified=true; ct.getCustomizationType = GetCustomizationType.customRecordType;  // Retrieve active custom record type IDs. The includeInactives param is set to false. GetCustomizationIdResult getCustIdResult = nss.getCustomizationId(ct, false);  // Retrieve the metadata of the returned custom record types ReadResponse [] readResp = nss.getList(getCustIdResult.customizationRefList);` 
        

## SOAP Request (getCustomizationId) {#bridgehead_3705199430}

          `<soapenv:Body>                     <getCustomizationId xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                            <customizationType getCustomizationType="customRecordType"/>                            <includeInactives>false</includeInactives>                     </getCustomizationId>              </soapenv:Body>` 
        

## SOAP Response (getCustomizationId) {#bridgehead_3705200038}

          `<getCustomizationIdResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformCore:getCustomizationIdResult       xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:totalRecords>1</platformCore:totalRecords>                <platformCore:customizationRefList>                   <platformCore:customizationRef internalId="15" scriptId="customrecord15"          type="customRecordType">                      <platformCore:name>Customer Satisfaction Survey</platformCore:name>                   </platformCore:customizationRef>                </platformCore:customizationRefList>             </platformCore:getCustomizationIdResult>          </getCustomizationIdResponse>` 
        

## SOAP Request (getList) {#bridgehead_3705199704}

          `<getList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <baseRef xmlns:q1="urn:core_2017_1.platform.webservices.netsuite.com"       xsi:type="q1:CustomizationRef" internalId="15" scriptId="customrecord15"          type="customRecordType">                   <q1:name>Customer Satisfaction Survey</q1:name>                </baseRef>             </getList>` 
        

## SOAP Response (getList) {#bridgehead_3705200385}

          `<getListResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <readResponseList>                   <readResponse>                      <platformCore:status isSuccess="true"          xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <record internalId="15" xsi:type="setupCustom:CustomRecordType"          xmlns:setupCustom="urn:customization_2017_1.setup.webservices.netsuite.com">                         <setupCustom:recordName>Customer Satisfaction Survey</setupCustom:recordName>                         <setupCustom:includeName>true</setupCustom:includeName>                         <setupCustom:showId>true</setupCustom:showId>                         <setupCustom:showCreationDate>true</setupCustom:showCreationDate>                         <setupCustom:showCreationDateOnList>true</setupCustom:showCreationDateOnList>                         <setupCustom:isAvailableOffline>false</setupCustom:isAvailableOffline>                         <setupCustom:allowQuickSearch>false</setupCustom:allowQuickSearch>                         <setupCustom:isInactive>false</setupCustom:isInactive>                         <setupCustom:disclaimer><b>Record numbers cannot be reverted back to names after being             updated.<br/></setupCustom:disclaimer>                         <setupCustom:enableNumbering>false</setupCustom:enableNumbering>                         <setupCustom:numberingCurrentNumber>413</setupCustom:numberingCurrentNumber>                         <setupCustom:allowNumberingOverride>false</setupCustom:allowNumberingOverride>                         <setupCustom:isNumberingUpdateable>false</setupCustom:isNumberingUpdateable>                         <setupCustom:scriptId>customrecord15</setupCustom:scriptId>                         <setupCustom:fieldList>                            <setupCustom:customField scriptId="customrecord_CONTACT_TYPE">                               <setupCustom:label>Contact type</setupCustom:label>                               <setupCustom:fieldType>_listRecord</setupCustom:fieldType>                               <setupCustom:selectRecordType internalId="16"             xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                                  <platformCore:name>Customer contact type</platformCore:name>                               </setupCustom:selectRecordType>                               <setupCustom:storeValue>true</setupCustom:storeValue>                               <setupCustom:showInList>false</setupCustom:showInList>                               <setupCustom:globalSearch>false</setupCustom:globalSearch>                               <setupCustom:isParent>false</setupCustom:isParent>                               <setupCustom:displayType>_normal</setupCustom:displayType>                               <setupCustom:isMandatory>true</setupCustom:isMandatory>                               <setupCustom:checkSpelling>false</setupCustom:checkSpelling>                               <setupCustom:defaultChecked>false</setupCustom:defaultChecked>                               <setupCustom:isFormula>false</setupCustom:isFormula>                               <setupCustom:recType>15</setupCustom:recType>                               <setupCustom:roleRestrict>false</setupCustom:roleRestrict>                               <setupCustom:accessLevel>_edit</setupCustom:accessLevel>                               <setupCustom:searchLevel>_edit</setupCustom:searchLevel>                            </setupCustom:customField>                            <setupCustom:customField scriptId="customrecord_IF_OTHER">                               <setupCustom:label>Other contact type</setupCustom:label>                               <setupCustom:fieldType>_freeFormText</setupCustom:fieldType>                               <setupCustom:storeValue>true</setupCustom:storeValue>                               <setupCustom:showInList>false</setupCustom:showInList>                               <setupCustom:globalSearch>false</setupCustom:globalSearch>                               <setupCustom:isParent>false</setupCustom:isParent>                               <setupCustom:displayType>_normal</setupCustom:displayType>                               <setupCustom:displayWidth>42</setupCustom:displayWidth>                               <setupCustom:isMandatory>false</setupCustom:isMandatory>                               <setupCustom:checkSpelling>false</setupCustom:checkSpelling>                               <setupCustom:defaultChecked>false</setupCustom:defaultChecked>                               <setupCustom:isFormula>false</setupCustom:isFormula>                               <setupCustom:recType>15</setupCustom:recType>                               <setupCustom:roleRestrict>false</setupCustom:roleRestrict>                               <setupCustom:accessLevel>_edit</setupCustom:accessLevel>                               <setupCustom:searchLevel>_edit</setupCustom:searchLevel>                            </setupCustom:customField>               // custom field list continues ...                       </setupCustom:fieldList>                      <setupCustom:formsList>                            <setupCustom:forms>                               <setupCustom:formName>Standard Customer Satisfaction Survey             Form<setupCustom:formName>                               <setupCustom:formPref>false</setupCustom:formPref>                            </setupCustom:forms>                         </setupCustom:formsList>                         <setupCustom:parentsList>                            <setupCustom:parents>                               <setupCustom:childDescr>Customer</setupCustom:childDescr>                            </setupCustom:parents>                         </setupCustom:parentsList>                      </record>                   </readResponse>                </readResponseList>             </getListResponse>` 
        

## SOAP Request for Returning Custom Segments {#bridgehead_1535368250}

          `<soapenv:Body>                              <getCustomizationId xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">                                        <customizationType getCustomizationType="customSegment"/>                                        <includeInactives>false</includeInactives>                              </getCustomizationId>                    </soapenv:Body` 
        

## SOAP Response with Unified Script ID Used on the Custom Segment {#bridgehead_1535368448}

          `<soapenv:Body>          <getCustomizationIdResponse xmlns="urn:messages_2019_1.platform.webservices.netsuite.com">             <platformCore:getCustomizationIdResult xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:totalRecords>1</platformCore:totalRecords>                <platformCore:customizationRefList>                   <platformCore:customizationRef scriptId="cseg_testws" internalId="1" type="customSegment">                      <platformCore:name>TestWS</platformCore:name>                   </platformCore:customizationRef>                </platformCore:customizationRefList>             </platformCore:getCustomizationIdResult>          </getCustomizationIdResponse>       </soapenv:Body>` 
        

## Java Sample {#bridgehead_1520864992}

The following Java sample show how to construct a getCustomizationId request so that the IDs for all custom record type objects are returned. In this example, inactive custom record type objects are not returned.

          `// Perform getCustomizationId operation on the custom record type      public void getCustomizationId () throws Exception {         CustomizationType ct = new CustomizationType();         ct.setGetCustomizationType(GetCustomizationType.entityCustomField);         ct.getGetCustomizationType();          c.getCustomizationId(GetCustomizationType.customRecordType, false);` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
