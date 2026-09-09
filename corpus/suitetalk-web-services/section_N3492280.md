---
id: "section_N3492280"
type: "section"
title: "getCurrencyRate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getCurrencyRate"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3492280.html"
anchors: ["bridgehead_N3492338", "bridgehead_N3492458", "bridgehead_N3492643", "bridgehead_N3492796", "bridgehead_N3492934", "bridgehead_3705194565", "bridgehead_3705194817", "bridgehead_3705195147"]
sha256: "203e50bc242504c19c2579a899fe2735a9fea01d32855f6cb47a5f7552fa9767"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

Use this operation to get the exchange rate between two currencies based on a certain date. The exchange rate values you are getting are those that appear in the Exchange Rate column of the Currency Exchange Rates table, which you can view at Lists > Accounting > Currency Exchange Rates.

The role used to perform this operation must have at least View level of the Currency permission (a Lists type permission).

Note:

The Multiple Currencies feature must be enabled in your account before using the getCurrencyRate operation. For information about enabling this feature, see [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html).

![Table of currency exchange rates in the UI.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteTalkWebServices/currencyExchangeRates.png)

## Request {#bridgehead_N3492338}

The GetCurrencyRateRequest type is used for the request. This method accepts the argument CurrencyRateFilter. With this filter you specify what you want returned in the results.

If you do not specify anything in the filter, the resulting CurrencyRateList will contain all currency exchange rates (all combinations) for the actual date. For example, if you specify baseCurrency only (for example, Euro), you will get all rates for Euro {USD,YEN,SING,....}.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| currencyRateFilter | CurrencyRateFilter | Filter the returned currency exchange rates using this filter. |

## CurrencyRateFilter {#bridgehead_N3492458}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| baseCurrency | RecordRef | References the base currency. This argument is optional. |
| fromCurrency | RecordRef | References the from or 'exchange' currency. This argument is optional. |
| effectiveDate | dateTime | This argument is optional. If a date is not provided, the date defaults to the current date. |

## Response {#bridgehead_N3492643}

The GetCurrencyRateResponse type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| currencyRate | double | Returns a list of available currency exchange rates. |

## Faults {#bridgehead_N3492796}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   InsufficientPermissionFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3492934}

## SOAP Request {#bridgehead_3705194565}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <ns1:passport soapenv:mustUnderstand="0" soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">email@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">*******</ns3:password>             <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">1234567</ns4:account>             <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>         </ns1:passport>     </soapenv:Header>     <soapenv:Body>         <getCurrencyRate xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <currencyRateFilter>                 <ns6:baseCurrency internalId="2" xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns7:fromCurrency internalId="1" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">                 <ns8:effectiveDate xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">2012-08          11T06:58:59.628Z</ns8:effectiveDate>             </currencyRateFilter>         </getCurrencyRate>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_3705194817}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1326288_08092012257172984776216537_6c7c330232bb5</platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <getCurrencyRateResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformCore:getCurrencyRateResult xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                 <platformCore:status isSuccess="true"/>                 <platformCore:currencyRateList>                     <platformCore:currencyRate>                         <platformCore:baseCurrency internalId="2"/>                         <platformCore:fromCurrency internalId="1"/>                         <platformCore:exchangeRate>0.42283298</platformCore:exchangeRate>                         <platformCore:effectiveDate>1970-01-01T00:00:00.000-08:00</platformCore:effectiveDate>                     </platformCore:currencyRate>                 </platformCore:currencyRateList>             </platformCore:getCurrencyRateResult>         </getCurrencyRateResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

## Java {#bridgehead_3705195147}

This sample shows how to get the actual rate for tomorrow and for USD to GBP.

          `public void getCurrencyRate() throws Exception    {       this.login();         CurrencyRateFilter crf = new CurrencyRateFilter();       Calendar cal = Calendar.getInstance();       cal.add(Calendar.DAY_OF_YEAR, +1); //tomorrow       crf.setEffectiveDate(cal);         RecordRef currencyRef1 = new RecordRef();       currencyRef1.setInternalId("1"); //USD       crf.setBaseCurrency(currencyRef1);         RecordRef currencyRef2 = new RecordRef();       currencyRef2.setInternalId("2"); //GBP       crf.setFromCurrency(currencyRef2);         GetCurrencyRateResult gcrr = _port.getCurrencyRate(crf);       CurrencyRateList crl = gcrr.getCurrencyRateList();       CurrencyRate cr = crl.getCurrencyRate(0);       Double rate = cr.getExchangeRate();         System.out.println("Exchange rate is = " + rate);    }` 
        

Note:

The mrr() method is a convenience method for specifying a record without the need to indicate a record type.

          `/* Make Record Ref out of an internalId */         public static RecordRef mrr(String internalId)         {                RecordRef toRet = new RecordRef();                toRet.setInternalId(internalId);                return toRet;         }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
