---
id: "section_N3491080"
type: "section"
title: "getConsolidatedExchangeRate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getConsolidatedExchangeRate"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3491080.html"
anchors: ["bridgehead_4771608408", "bridgehead_N3491202", "bridgehead_N3491317", "bridgehead_N3491503", "bridgehead_N3491656", "bridgehead_N3491767", "bridgehead_N3492059", "bridgehead_N3492134"]
sha256: "552efed1adb03bb6773478d422118a648a7feef9d84f49be63d6d73028e20fd4"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

On the Consolidated Exchange Rates table, you can maintain exchange rates between the root-parent and child subsidiaries. Use the getConsolidatedExchangeRate operation to get and filter all data related to this table.

Important:

The exposure of the consolidated exchange rate record prompted the removal of the getConsolidatedExchangeRate operation from the 2017.1 endpoint. You can still use the getConsolidatedExchangeRate operation on earlier endpoints. For more information about working with consolidated exchange rates on endpoints starting from 2017.1, see [Consolidated Exchange Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4847555414.html).

Important:

This operation can be used only in NetSuite OneWorld acccounts.

In the UI, you can see the Consolidated Exchange Rates table by going to List > Accounting > Consolidated Exchange Rates. Note that in SOAP web services, this table is read-only.

For general information about currencies and working with the Consolidated Exchange Rate table, see the following topics:

-   [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html)
    
-   [Currency Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1401566.html)
    

Note:

If you choose, you can set exchange rates in the Consolidated Exchange Rates table directly. See the steps under 'To set exchange rates in the Consolidated Exchange Rates table' for details.

-   [Currency Exchange Rate Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404429.html)
    
-   [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html)
    

## getConsolidatedExchangeRate for the Multi-Book Accounting Feature {#bridgehead_4771608408}

Results for the getConsolidatedExchageRate operation can include values for the book field. Results can also be filtered by this field.

-   If the Multi-Book Accounting feature is enabled:
    
    -   If the book is not set in the request, getConsolidatedExchangeRate returns values for all accounting books that have the Enable Consolidation option selected.
        
    -   If the book is set in the request, getConsolidatedExchangeRate returns values for the specified accounting book.
        
-   If the Multi-Book Accounting feature is not enabled:
    
    -   If the book is set in the request, getConsolidatedExchangeRate returns an error with the code = "FEATURE\_DISABLED" and the message = "The ''Multi-Book Accounting'' feature is not enabled in your NetSuite account."
        
    -   Book is not part of the response.
        

Note:

In endpoints prior to 2016.2, the getConsolidatedExchangeRate operation can only be used to return results for the primary accounting book, even if the Multi-Book Accounting feature is enabled.

## Request {#bridgehead_N3491202}

The GetConsolidatedExchangeRateRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| consolidatedExchangeRateFilter | ConsolidatedExchangeRateFilter | You can filter the returned consolidated exchange rates using this filter. |

## ConsolidatedExchangeRateFilter {#bridgehead_N3491317}

ConsolidatedExchangeRateFilter is defined in the [core](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd) XSD.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | References an existing period. This argument is required. |
| fromSubsidiary | RecordRef | References the receiving subsidiary. This argument is optional. |
| toSubsidiary | RecordRef | References the originating subsidiary. This argument is optional. |
| book | RecordRef | References the specific accounting book for accounts with the Multi-Book Accounting feature enabled. |

## Response {#bridgehead_N3491503}

The GetConsolidatedExchangeRateResult type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| consolidatedExchangeRateList | ConsolidatedExchangeRateList | Returns a list of available consolidated exchange rates. |

## ConsolidatedExchangeRateList {#bridgehead_N3491656}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| consolidatedExchangeRate | ConsolidatedExchangeRate | References an existing period. |

## ConsolidatedExchangeRate {#bridgehead_N3491767}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | References an existing period. |
| fromSubsidiary | RecordRef | References the receiving subsidiary. |
| toSubsidiary | RecordRef | References the originating subsidiary. |
| currentRate | double | References the current rate. |
| averageRate | double | References the average rate. |
| historicalRate | double | References the historical rate. |

## Faults {#bridgehead_N3492059}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3492134}

The getConsolidatedExchangeRate and getBudgetExchangeRate operations are used in the same way. Therefore, please refer to the [Sample Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489718.html#bridgehead_N3490913) for getBudgetExchangeRate.

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
