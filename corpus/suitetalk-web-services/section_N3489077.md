---
id: "section_N3489077"
type: "section"
title: "getAll"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getAll"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html"
anchors: ["bridgehead_N3489096", "bridgehead_N3489212", "bridgehead_N3489363", "bridgehead_1520951604", "bridgehead_1520951659", "bridgehead_1520951707", "bridgehead_1520951737"]
sha256: "214311cdf854e80e3a588cff32caf4caf1518b8f0938f9f047063c984aaf369d"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The getAll operation is used to retrieve a list of all records of the specified type. Records that support the getAll operation are listed in the GetAllRecordType, as defined in the platformCoreType system constants XSD file.

Note:

You cannot use the search operation to retrieve state values. You must use the getAll operation. The getAll operation will return all states, not the legal ones for your default country. Also note that the country and state must match on the address.

## Request {#bridgehead_N3489096}

The getAllRequest type is used for the request. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| recordType | GetAllRecordType | Specify the record type. |

## Response {#bridgehead_N3489212}

The getList response type is used for the response. It contains the following fields.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| recordList | Record\[\] | A list of records that correspond to the specified ids. The records returned need to be of a type that extends the abstract type Record. |

## Faults {#bridgehead_N3489363}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_1520951604}

The following sample shows how to retrieve the list of all Currency records.

## Java {#bridgehead_1520951659}

          `public void getAll() throws Exception {          c.getAll(GetAllRecordType.currency);     }` 
        

## SOAP Request {#bridgehead_1520951707}

          `<soapenv:Body>            <getAll xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record recordType="currency"/>            </getAll>        </soapenv:Body>` 
        

## SOAP Response {#bridgehead_1520951737}

          `<soapenv:Body>          <getAllResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformCore:getAllResult xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:totalRecords>2</platformCore:totalRecords>                <platformCore:recordList>                   <platformCore:record internalId="1" xsi:type="listAcct:Currency" xmlns:listAcct="urn:accounting_2017_1.lists.webservices.netsuite.com">                      <listAcct:name>US USD</listAcct:name>                      <listAcct:symbol>USD</listAcct:symbol>                      <listAcct:isBaseCurrency>true</listAcct:isBaseCurrency>                      <listAcct:isInactive>false</listAcct:isInactive>                      <listAcct:overrideCurrencyFormat>false</listAcct:overrideCurrencyFormat>                      <listAcct:displaySymbol>$</listAcct:displaySymbol>                      <listAcct:symbolPlacement>_beforeNumber</listAcct:symbolPlacement>                      <listAcct:locale>_unitedStatesEnglish</listAcct:locale>                      <listAcct:formatSample>$1,234.56</listAcct:formatSample>                      <listAcct:exchangeRate>1.0</listAcct:exchangeRate>                      <listAcct:currencyPrecision>_two</listAcct:currencyPrecision>                   </platformCore:record>                   <platformCore:record internalId="2" xsi:type="listAcct:Currency" xmlns:listAcct="urn:accounting_2017_1.lists.webservices.netsuite.com">                      <listAcct:name>UK GBP</listAcct:name>                      <listAcct:symbol>GBP</listAcct:symbol>                      <listAcct:isBaseCurrency>true</listAcct:isBaseCurrency>                      <listAcct:isInactive>false</listAcct:isInactive>                      <listAcct:overrideCurrencyFormat>false</listAcct:overrideCurrencyFormat>                      <listAcct:displaySymbol>&#xA3;</listAcct:displaySymbol>                      <listAcct:symbolPlacement>_beforeNumber</listAcct:symbolPlacement>                      <listAcct:locale>_unitedKingdomEnglish</listAcct:locale>                      <listAcct:formatSample>&#xA3;1,234.56</listAcct:formatSample>                      <listAcct:exchangeRate>0.6</listAcct:exchangeRate>                      <listAcct:currencyPrecision>_two</listAcct:currencyPrecision>                   </platformCore:record>                </platformCore:recordList>             </platformCore:getAllResult>          </getAllResponse>       </soapenv:Body>` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
