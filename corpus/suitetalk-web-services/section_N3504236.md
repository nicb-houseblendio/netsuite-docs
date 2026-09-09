---
id: "section_N3504236"
type: "section"
title: "getSelectValue"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getSelectValue"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html"
anchors: ["bridgehead_N3504418", "bridgehead_N3504494", "bridgehead_N3504531", "bridgehead_N3506802", "bridgehead_N3506894", "bridgehead_N3507056", "bridgehead_N3507534", "bridgehead_N3507758", "bridgehead_N3507833", "bridgehead_N27161181", "bridgehead_N27161241"]
sha256: "645edd0d6eb0389b7ebc13a5a9272c82df102e9e8d2034b22d7f0be62b128faf"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Use the getSelectValue operation to retrieve valid select options for a particular [RecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3454730), [CustomRecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3454996), or enumerated static field. This is useful if you are writing an application UI that needs to mimic NetSuite UI logic, if the referenced record type is not yet exposed in SOAP web services, or when the logged-in user's role does not have permission to the instances of the referenced record type. A call to getSelectValue may return different results for the same field for different roles.

The getSelectValue operation can be used on standard body fields and custom body fields. It can also be used on sublist fields that appear on both standard and custom records.

Important:

The getSelectValue operation is not supported for record types which can't be created with SuiteScript, like for example Inventory Number or Period End Journal Entry.

These topics describe each aspect of the operation:

-   [GetSelectValue Overview](#bridgehead_N3504418)
    
-   [Paginating Select Values](#bridgehead_N3504494)
    
-   [Filtering Select Value Text](#bridgehead_N3504531)
    
-   [Getting Dependent Select Values](#bridgehead_N3506802)
    
-   [Sample Code](#bridgehead_N3507833)
    

Important:

If you reference a field or a select value that is renamed in future versions of NetSuite, your requests will still be handled, however, a warning will be returned. Also, when working with this operation be aware of any special permissions applied to a field. For example, a permission error will be thrown if you attempt to get select values on a field that has been disabled on a form.

Note:

The getSelectValue operation will not return the following values: "" , (blank), -1,

\-New-, -2, -Custom-.

## GetSelectValue Overview {#bridgehead_N3504418}

You can use getSelectValue to return the entire list of values or a subset of values.

In accounts where there are levels of field dependencies, such as OneWorld accounts, you can use getSelectValue to get select values for field 'B' based on the value of field 'A'. For example, select values associated with the Department field are based on the value specified in the Subsidiary field. In this scenario, you can use getSelectValue to get the values on the Department field by specifying the internal ID of its filterBy ('primary') field, which is Subsidiary (internal ID - **subsidiary**). For more information, see [Getting Dependent Select Values](#bridgehead_N3506802).

Running getSelectValue against records that are created from other records may result in an INSUFFICIENT\_PERMISSION error.

Important:

The getSelectValue operation is not supported for record types which can't be created with SuiteScript, like for example Inventory Number or Period End Journal Entry.

## Paginating Select Values {#bridgehead_N3504494}

The first call to getSelectValue returns the total number of select values for the specified field. If you choose, you can return a subset of those values by specifying a pageIndex number in the request.

          `<complexType name="getSelectValueRequest">         <sequence>             <element name="fieldDescription" type="platformCore:GetSelectValueFieldDescription"       minOccurs="1" maxOccurs="1"/>       <element name=" pageIndex " type="xsd:int" minOccurs="1" maxOccurs="1"/>       </sequence>     </complexType>` 
        

Note:

To define a page size, set the pageSize element in the SearchPreference type. The value must be greater than 10 and less than the system-defined maximum of 1,000. If the number of select values exceeds the page size, the remaining results must be retrieved in subsequent calls getSelectValue with a new pageIndex value.

## Filtering Select Value Text {#bridgehead_N3504531}

To help end users pick from a long list of select values, you can use the **contains, startsWith**, or **is** search operators to filter the results returned by getSelectValue. The **filter** element in the GetSelectValueFieldDescription object lets you set the operator type in your request.

          `<complexType name=" GetSelectValueFieldDescription ">    <sequence>       <element name="recordType" type="platformCoreTyp:RecordType" minOccurs="0" maxOccurs="1"/>       <element name="customRecordType" type="platformCore:RecordRef" minOccurs="0"       maxOccurs="1"/>                   <element name="sublist" type="xsd:string" minOccurs="0" maxOccurs="1"/>          <element name="field" type="xsd:string" minOccurs="1" maxOccurs="1"/>          <element name="customForm" type="platformCore:RecordRef" minOccurs="0" maxOccurs="1"/>          <element name=" filter " type="platformCore: GetSelectValueFilter " minOccurs="0" maxOccurs="1"/>          <element name="filterByValueList" type="platformCore:GetSelectFilterByFieldValueList"       minOccurs="0" maxOccurs="1"/>         </sequence> </complexType>` 
        

## Getting Dependent Select Values {#bridgehead_N3506802}

The getSelectValue operation can also be used to get select values that are available on the condition of other field values. For example, in OneWorld accounts the values that appear in many dropdown fields are based on the values specified for either Customer or Subsidiary. As another example, on the Item sublist of a Sales Order, the values for the Tax Code field depend on both customer and item values.

In your getSelectValue call, you will use the **GetSelectFilterByFieldValueList** and **GetSelectFilterByFieldValue** objects to specify the filterBy field of a dependent field. (The dependent field is the field you want to get the values for. The filterBy field is the field that controls which values are available for the dependent field.)

          `<complexType name=" GetSelectFilterByFieldValueList ">       <sequence>         <element name="filterBy" type="platformCore:GetSelectFilterByFieldValue" minOccurs="1"          maxOccurs="unbounded"/>       </sequence>    </complexType>    <complexType name=" GetSelectFilterByFieldValue ">       <sequence>         <element name=" sublist " type="xsd:string" minOccurs="0" maxOccurs="1"/>         <element name=" field " type="xsd:string" minOccurs="1" maxOccurs="1"/>         <element name=" internalId " type="xsd:string" minOccurs="1" maxOccurs="1"/>       </sequence>    </complexType>` 
        

The sublist, field, and internalId arguments will contain:

-   the name of the sublist the filterBy field appears on (_if_ it appears on a sublist)
    
-   the schema name of the filterBy field (for example, 'entity')
    
-   the internalId of the specific entity record (for example, '87')
    

A getSelectValue call for a dependent field with no filterBy ('primay') field specified returns 0 records. This type of call also returns a warning that notes the filterBy field, so the call can be corrected.

Important:

Currently there is no programmatic way to discover what the filterBy field is for another field. Note, however, on transaction records the Customer ( **entity** ) field is always the filterBy field for any dependent RecordRef field. For all other record types, you must use the UI to see which field is the filterBy field.

## Request {#bridgehead_N3506894}

The getSelectValueRequest type is used for the request. It contains the following elements.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| fieldDescription | [GetSelectValueFieldDescription](#bridgehead_N3507056) | Use to specify all characteristics of the field containing the select values. For example, depending on the field and the values you want returned, you will specify the names or internalIds for the record type, sublist, and field. You may also specify filtering criteria to refine the select options returned in the response. |
| pageIndex | xsd: int | For select values that span multiple pages, use this argument to specify which page to return in your response. |

## GetSelectValueFieldDescription {#bridgehead_N3507056}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| recordType | RecordType | Specify a record defined in [coreTypes.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd) |
| customRecordType | RecordRef | If you are getting select values for a field appearing on a custom record, specify the internal or external ID of the custom record, as well as the custom record type. |
| sublist | xsd:string | If getting select values for a field on a sublist, you must specify the sublist name (as it is defined in the schema). Sublist names are those names that appear toward the bottom of a record schema and are appended with **List**, for example itemList, saleTeamList, timeList. |
| field | xsd:string | Specify a field name, as defined in the schema for that record. The field value can represent either a body field or a sublist field. |
| customForm | RecordRef | If the RecordRef or CustomRecordRef field is associated with a custom form, specify the internal or external ID of the custom form, as well as the custom form type. |
| filter | GetSelectValueFilter | If you choose, you can filter select options using the **contains, is**, or **startsWith** operator. Use any of these operators to return a subset of the options associated with the RecordRef or CustomRecordRef field. For example, to get a specific list of customers on an opportunity record, you can search for 'Adam' with the **contains** operator to get only customers whose name contains Adam. See also [Filtering Select Value Text](#bridgehead_N3504531). |
| filterByValueList | GetSelectFilterByFieldValueList | This will contain a reference to the filterBy field (or fields) in which you specify the following:
-   **sublist** - If the filterBy field is on a sublist, you will specify the name of the sublist containing this field. Sublist names are appended with List (for example item **List** ).
-   **field** - The name of the filterBy field (for example, _entity_ or _subsidiary_ ).
-   **internalId** - The internalId value of the filterBy field (for example, '87' or '112'). If the filterBy field on an Opportunity record is Customer, you would specify:
    
    sublist = null
    
    field = 'entity'
    
    internalId = '87' (87 being the internalId of a specific customer record, such as the Abe Simpson customer record)
    

See also [Getting Dependent Select Values](#bridgehead_N3506802). If a getSelectValue call does not return a warning, but also does not return any values, make sure you have specified all required filterByValueList values. To better understand which filterByValueList values are required in a record, go to a new record form in the UI. On the form you can see what other fields you must fill in, before your target field can get a value. The values in these fields are the required filterByValueList values you must specify. |

## Response {#bridgehead_N3507534}

The getSelectValueResponse type is used for the response. It contains the following elements.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| totalRecords | xsd:int | The total number of record references for this search. Depending on the pageSize value, some or all the references may be returned in the response. |
| totalPages | xsd:int | The total number of pages for this search. Depending on the pageSize value, some or all the pages may be returned in this response. |
| baseRefList | BaseRef\[\] | An array of baseRefs that references existing NetSuite records, including custom records. These baseRefs represent the valid values available for the current field. |

## Faults {#bridgehead_N3507758}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3507833}

## SOAP Request {#bridgehead_N27161181}

          `<?xml version="1.0" encoding="UTF-8"?><soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001 XMLSchema-instance">  <soapenv:Header>   <ns1:passport soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" soapenv:mustUnderstand="0"      xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">   <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">kwolfe@netsuite.com<     ns2:email>  <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com"><SOAP web services password><    ns3:password> <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">000071</ns4:account <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>   </ns1:passport>  </soapenv:Header>  <soapenv:Body>   <getSelectValue xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <fieldDescription>     <ns6:recordType xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">salesOrder<        ns6:recordType> <ns7:sublist xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">itemList</ns7:sublist> <ns8:field xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">item</ns8:field> <ns9:filterByValueList xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">      <ns9:filterBy>       <ns9:field>entity</ns9:field>       <ns9:internalId>8</ns9:internalId>      </ns9:filterBy>     </ns9:filterByValueList>    </fieldDescription>    <pageIndex>1</pageIndex>   </getSelectValue>  </soapenv:Body> </soapenv:Envelope>` 
        

## Java {#bridgehead_N27161241}

This sample shows how to get select values for the Item field that appears on the Item sublist of a Sales Order record.

In this sample the variable 'c' is a shortcut for the application that needs to communicate with NetSuite through SOAP Web Services. For more information about building an application, see [SOAP Web Services Quick Start](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419782.html).

          `GetSelectFilterByFieldValueList myFilterByList = new GetSelectFilterByFieldValueList(new      GetSelectFilterByFieldValue[]{new GetSelectFilterByFieldValue(null,"entity","8")});   GetSelectValueFieldDescription myGSVField = new GetSelectValueFieldDescription(RecordType.salesOrder,          null, "itemList", "item", null, null, myFilterByList);   BaseRef[] br = c.getSelectValue(myGSVField);` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
