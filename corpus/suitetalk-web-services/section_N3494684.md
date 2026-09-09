---
id: "section_N3494684"
type: "section"
title: "getDataCenterUrls"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getDataCenterUrls"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html"
anchors: ["bridgehead_N3494864", "bridgehead_N3497064", "bridgehead_N3497288", "bridgehead_N3497342", "bridgehead_1491373803", "bridgehead_3705201489", "bridgehead_N3497372", "bridgehead_3705202216", "bridgehead_3705202509", "bridgehead_N3497439"]
sha256: "e6d11867dbc91fb2f081b142cad911a66f8c14164c26d10e11f7a091deb88d7e"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

You use the getDataCenterUrls operation to obtain the correct URL for external client access to NetSuite.

getDataCenterURLs requests do not require authentication, nor any information identifying the application. The getDataCenterUrls operation ignores all authentication data, if any such data is sent.

SOAP web services versions 2019.1 and later are only available on account-specific domains. The URL for your account-specific SOAP web services domain includes your account ID. For example, if your account ID was 123456, then your account-specific SOAP web services domain would be 123456.suitetalk.api.netsuite.com. As of 2019.1, the getDataCenterUrls operation also returns your account-specific SOAP web services domain.

For more details, see [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html).

Important:

As of the 2019.1 SOAP web services endpoint, you must use account-specific domains with SOAP web services. Use the SOAP getDataCenterUrls operation to obtain the correct domain. Or, go to _Setup > Company > Setup Tasks > Company Information_ in the NetSuite UI. Your domains are listed on the Company URLs subtab.

In addition to the URL for SOAP web services access, the getDataCentersUrls operation also supports discovery of other NetSuite domains. You can use this operation to discover any of the following:

-   restletDomain - https://<accountID>.restlets.api.netsuite.com
    
-   systemDomain - https://<accountID>.app.netsuite.com
    
-   webservicesDomain - https://<accountID>.suitetalk.api.netsuite.com
    

If you are building an integration for your own use or for a single customer, you integration must include logic to determine the correct URL for the appropriate NetSuite account. If you are building an application that will be distributed to multiple customers, you must incorporate logic that can determine the correct URL for any of those customers.

Important:

The dynamic discovery service is upgraded early and independently of your account, so [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) may be processed with the new WSDL version, even though the target account hasn't been upgraded yet. If your integration uses an older endpoint like 2019\_2 and is negatively impacted, use one of the following alternatives:

-   Use one of the supported endpoints for the NetSuite 2025.2 release on all SOAP calls, ideally the 2025\_2 endpoint.
    
-   Instead of dynamic discovery [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) requests use the Account Specific Endpoint (Setup > Company > Company Information > Company URLs | SuiteTalk SOAP URL) to target all SOAP calls. This way it is still possible to use https://<accountID>.suitetalk.api.netsuite.com/services/NetSuitePort\_2019\_2, if your own account is on the 2025.2 version.
    
-   Append the URL parameter NS\_VER=2025.2 on your endpoint URL for your initial dynamic discovery [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) request (https://webservices.NetSuite.com/services/NetSuitePort\_2019\_2?NS\_VER=2025.2). This will force routing for this initial request to system endpoint where it will not fail.
    

## Request {#bridgehead_N3494864}

The GetDataCenterUrlsRequest type is used for this request. It requires the following field:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| account | string | NetSuite account ID. Note: If an invalid account ID is specified, the default URLs are returned. |

## Response {#bridgehead_N3497064}

The GetDataCenterUrlsResult type is used for the response. It contains the following fields:

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| restDomain | string | URL used by external client applications to access NetSuite through a RESTlet. |
| systemDomain | string | \- |
| webservicesDomain | string | URL used by external client applications to access NetSuite through SOAP web services. |

## Faults {#bridgehead_N3497288}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

Also, a DATA\_REQD error is thrown if no account ID is provided in the request. For an example, see [SOAP Response (empty account)](#bridgehead_N3497439).

## Sample Code {#bridgehead_N3497342}

## C# Sample {#bridgehead_1491373803}

          `class  DataCenterDomains  : NetSuiteService     {          private System.Uri OriginalUri;          public  DataCenterDomains (string account, bool doNotSetUrl)             : base()         {             OriginalUri = new System.Uri(this.Url);             if (account == null || account.Length == 0)                 account = "empty";             if (!doNotSetUrl)             {                  DataCenterUrls urls = getDataCenterUrls(account).dataCenterUrls;                 Uri dataCenterUri = new Uri(urls.webservicesDomain + OriginalUri.PathAndQuery);                 this.Url = dataCenterUri.ToString();             }         }          public void SetAccount(string account)         {             if (account == null || account.Length == 0)                 account = "empty";              this.Url = OriginalUri.AbsoluteUri;             DataCenterUrls urls = getDataCenterUrls(account).dataCenterUrls;             Uri dataCenterUri = new Uri(urls.webservicesDomain + OriginalUri.PathAndQuery);             this.Url = dataCenterUri.ToString();         }     }` 
        

## Java Sample {#bridgehead_3705201489}

          `/**  * Accounts are located in multiple data centers with different domain names.  * To use the correct one, wrap the Locator and get the correct domain first.  *  * See getDataCenterUrls WSDL method documentation in the Help Center.  */ private static class  dataCenters  extends NetSuiteServiceLocator {    private String account;      public  dataCenters (String account)    {       this.account = account;    }      @Override    public NetSuitePortType getNetSuitePort(URL defaultWsDomainURL)    {       try       {          NetSuitePortType _port = super.getNetSuitePort(defaultWsDomainURL);          // Get the webservices domain for your account          DataCenterUrls urls = _port.getDataCenterUrls(account).getDataCenterUrls();          String wsDomain = urls.getWebservicesDomain();            // Return URL appropriate for the specific account          return super.getNetSuitePort(new URL(wsDomain.concat(defaultWsDomainURL.getPath())));       }       catch (Exception e)       {          throw new RuntimeException(e);       }    } }   --- // Locate the NetSuite web service. NetSuiteServiceLocator service = new  dataCenters ("myAccount"); // Get the service port (to the correct data center) _port = service.getNetSuitePort(new URL("https://webservices.netsuite.com/services/NetSuitePort_2025_2"));` 
        

## Java Sample {#bridgehead_N3497372}

          `public void testDataCenterUrlsPublic() throws Exception {     NLWsClient c = new NLWsClient();        c.initPort();     String account = "1326288";         System.out.println("Account: " + account);     DataCenterUrls urls = c.getPort().getDataCenterUrls(account).getDataCenterUrls();         System.out.println("\tREST domain: " + urls.getRestDomain());     System.out.println("\tWeb services domain: " + urls.getWebservicesDomain());     System.out.println("\tSystem domain: " + urls.getSystemDomain());     System.out.println(); }` 
        

## SOAP Request {#bridgehead_3705202216}

          `<?xml version="1.0" encoding="UTF-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Body>           <getDataCenterUrls xmlns="urn:messages_2025_2.platform.webservices.netsuite.com">               <account>1326288</account>           </getDataCenterUrls>       </soapenv:Body>    </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_3705202509}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2025_2.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1326288_08162012790521873260264554_10fa27f165429</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <getDataCenterUrlsResponse xmlns="urn:messages_2025_2.platform.webservices.netsuite.com">             <getDataCenterUrlsReturn xsi:type="GetDataCenterUrlsResult" xmlns:platformCore="urn:core_2025_2.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:dataCenterUrls>                   <platformCore:restDomain>https://<accountID>.restlets.api.netsuite.com</platformCore:restDomain>                   <platformCore:webservicesDomain>https://<accountID>.suitetalk.api.netsuite.com</platformCore:webservicesDomain>                   <platformCore:systemDomain>https://<accountID>.app.netsuite.com</platformCore:systemDomain>                </platformCore:dataCenterUrls>             </getDataCenterUrlsReturn>          </getDataCenterUrlsResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

## SOAP Response (empty account) {#bridgehead_N3497439}

          `<?xml version="1.0" encoding="utf-8"?>    <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2025_2.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES__0911201212589142971204370270_d03cd34b349479541b</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <getDataCenterUrlsResponse xmlns="urn:messages_2025_2.platform.webservices.netsuite.com">             <getDataCenterUrlsReturn xsi:type="GetDataCenterUrlsResult" xmlns:platformCore="urn:core_2025_2.platform.webservices.netsuite.com">                <platformCore:status isSuccess="false">                   <platformCore:statusDetail type="ERROR">                      <platformCore:code>DATA_REQD</platformCore:code>                      <platformCore:message>You need to provide a proper value for the required field: account.</platformCore:message>                   </platformCore:statusDetail>                </platformCore:status>             </getDataCenterUrlsReturn>          </getDataCenterUrlsResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

### Related Topics

-   [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html)
-   [Understanding NetSuite URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4295564687.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
