---
id: "section_N3489718"
type: "section"
title: "getBudgetExchangeRate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getBudgetExchangeRate"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489718.html"
anchors: ["bridgehead_N3489778", "bridgehead_N3489894", "bridgehead_N3490080", "bridgehead_N3490233", "bridgehead_N3490344", "bridgehead_N3490837", "bridgehead_N3490913", "bridgehead_3705193829", "bridgehead_3705194115", "bridgehead_N3490944"]
sha256: "b06dbe850b72b42ad8232547e3a5ef68179df58759acddb4c42f3b2260440db9"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

On the Budget Exchange Rates table, you can maintain exchange rates between the root-parent and child subsidiaries for use in the budgeting process. Use the getBudgetExchangeRate operation to get and filter all data related to this table.

Important:

This operation can be used only in NetSuite OneWorld accounts.

In the UI, you can see the Budget Exchange Rates table by going to List > Accounting > Budget Exchange Rates. Note that in SOAP web services, this table is read-only.

For general information about the Budget Exchange Rate table, see [Budget Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1508302.html).

## Request {#bridgehead_N3489778}

The GetBudgetExchangeRateRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| budgetExchangeRateFilter | BudgetExchageRateFilter | You can filter the returned exchange rates for a budget using this filter. |

## BudgetExchangeRateFilter {#bridgehead_N3489894}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | References an existing period. This argument is required. |
| fromSubsidiary | RecordRef | References the receiving subsidiary. This argument is optional. |
| toSubsidiary | RecordRef | References the originating subsidiary. This argument is optional. |

## Response {#bridgehead_N3490080}

The GetBudgetExchangeRateResult type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| budgetExchangeRateList | BudgetExchangeRateList | Returns a list of available exchange rates in a budget. |

## BudgetExchangeRateList {#bridgehead_N3490233}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| budgetExchangeRate | BudgetExchangeRate | References the exchange rate for a budget. |

## BudgetExchangeRate {#bridgehead_N3490344}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | References an existing period. |
| fromSubsidiary | RecordRef | References the receiving subsidiary. |
| toSubsidiary | RecordRef | References the originating subsidiary. |
| currentRate | double | References the current rate. |
| averageRate | double | References the average rate. |
| historicalRate | double | References the historical rate. |

## Faults {#bridgehead_N3490837}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3490913}

## SOAP Request {#bridgehead_3705193829}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">        <soapenv:Body>            <getBudgetExchangeRate xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <budgetExchangeRateFilter>                    <ns1:period internalId="3" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns2:fromSubsidiary internalId="4" xmlns:ns2="urn:core_2017_1.platform.webservices.       netsuite.com"/>             </budgetExchangeRateFilter>            </getBudgetExchangeRate>        </soapenv:Body>    </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_3705194115}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Body>          <getBudgetExchangeRateResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformCore:getBudgetExchangeRateResult       xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:budgetExchangeRateList>                   <platformCore:budgetExchangeRate>                      <platformCore:period internalId="3"/>                      <platformCore:fromSubsidiary internalId="4"/>                      <platformCore:toSubsidiary internalId="1"/>                      <platformCore:currentRate>1.9586</platformCore:currentRate>                      <platformCore:averageRate>1.9586</platformCore:averageRate>                      <platformCore:historicalRate>1.9586</platformCore:historicalRate>                   </platformCore:budgetExchangeRate>                </platformCore:budgetExchangeRateList>             </platformCore:getBudgetExchangeRateResult>          </getBudgetExchangeRateResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

## Java {#bridgehead_N3490944}

          `/* Make Record Ref out of an internalId */    public static RecordRef mrr(String internalId)    {       RecordRef toRet = new RecordRef();       toRet.setInternalId(internalId);       return toRet;    }    c.getPort().getBudgetExchangeRate(new BudgetExchangeRateFilter(mrr("3"),mrr("4"),null));` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
