---
id: "section_N3500304"
type: "section"
title: "getPostingTransactionSummary"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > getPostingTransactionSummary"
parent: "chapter_N3477815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3500304.html"
anchors: ["bridgehead_N3500569", "bridgehead_N3500756", "bridgehead_N3501157", "bridgehead_N3502473", "bridgehead_N3502768", "bridgehead_N3502897", "bridgehead_N3503342", "bridgehead_N3503417", "bridgehead_N3503426", "bridgehead_N3503459", "bridgehead_N3503470", "bridgehead_N27135141", "bridgehead_N27135201", "bridgehead_N3503513"]
sha256: "cfe11451eff0d1ff64ed956c7ddfaf582488e73b47edde3768bbb13d31d7528b"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

The getPostingTransactionSummary operation lets you retrieve a summary of the actual data that posted to the general ledger in an account. You can use available filters and fields to generate reports that are similar to what you see when you run financial reports such as a Trial Balance, Balance Sheet, or an Income Statement.

Note:

For information about NetSuite financial reports and financial statements, see the following topics:

-   [Financial Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1520496.html)
    
-   [Financial Statements Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2092547.html)
    

The getPostingTransactionSummary operation returns the fields defined in [PostingTransactionSummary](#bridgehead_N3502897). You can query by any filter defined in [PostingTransactionSummaryFilter](#bridgehead_N3501157) and group the results by any field defined in [PostingTransactionSummaryField](#bridgehead_N3500756).

The first call to the operation returns the first page, total number of hits (totalRecords), and the number of pages. You can then retrieve subsequent pages by giving the page number.

Note:

NetSuite caches the results after the first call to getPostingTransactionSummary as subsequent pages are being retrieved. The cache is reset if the session expires, or if you make another call to this operation with a page index of 1.

Also note the following:

-   This operation can only be executed in a role that has the Financial Statements permission assigned. To enable this permission for a role, a NetSuite administrator must go to _Setup > User Roles > Manage Roles_, click the Reports subtab, select **Financial Statments** from the Permission list, and then click Save.
    
-   To search for null, specify -1. If the return is null, the element will be skipped (not -1).
    
-   A maximum of 10,000 expressions is supported. A request with more than this number of expressions returns an error.
    
-   For large reports (for example, you have chosen all the columns), the query will take a long time on first request, but subsequent requests will be fast. Make sure your timeout limit is set high.
    

Important:

The information in the following paragraph pertains to **NetSuite OneWorld** accounts **only**.

The amounts returned from getPostingTransactionSummary are in the currency of the **subsidiary**, not the parent. If you want the amounts in the currency of the parent, you must programmatically apply the appropriate exchange rate. To obtain exchange rates, you must call [getConsolidatedExchangeRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3491080.html), which reads data from the Consolidated Exchange Rate table. In your code, you must then multiply amount values returned by getPostingTransactionSummary by the exchange rate values returned by getConsolidatedExchangeRate.

Although the NetSuite UI automatically consolidates all amounts, you must perform your own exchange rate calculations in SOAP web services.

Note:

You may want to do planning in your local currency, in which case there is no need for exchange rate conversions.

## Request {#bridgehead_N3500569}

The GetPostingTransactionSummaryRequest type is used for the request.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| fields | PostingTransactionSummaryField | Specify how you want your data grouped. |
| filters | PostingTransactionSummaryFilter | Specify your filtering criteria. |
| pageIndex | xsd:int | Specify the page to be returned. |

## PostingTransactionSummaryField {#bridgehead_N3500756}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | Specify to group data by period. |
| account | RecordRef | Specify to group data by account. |
| parentItem | RecordRef | Specify to group data by parent item. |
| item | RecordRef | Specify to group data by item. |
| customer | RecordRef | Specify to group data by customer. |
| department | RecordRef | Specify to group data by department. |
| class | RecordRef | Specify to group data by class. |
| location | RecordRef | Specify to group data by location. |
| subsidiary | RecordRef | Specify to group data by subsidiary. |
| book | RecordRef | If you use the Multi-Book Accounting feature, specify to group data by accounting book. |

## PostingTransactionSummaryFilter {#bridgehead_N3501157}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | Filter your request by period. |
| account | RecordRef | Filter your request by account. |
| parentItem | RecordRef | Filter your request by parent item. |
| item | RecordRef | Filter your request by item. |
| customer | RecordRef | Filter your request by customer. |
| department | RecordRef | Filter your request by department. |
| class | RecordRef | Filter your request by class. |
| location | RecordRef | Filter your request by location. |
| subsidiary | RecordRef | Filter your request by subsidiary. |
| book | RecordRef | If you use the Multi-Book Accounting feature, filter your request by accounting book. |

## Response {#bridgehead_N3502473}

The GetPostingTransactionSummaryResult type is used for the response.

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| status | Status | The status for this operation. All applicable errors or warnings are listed within this type. |
| totalRecords | xsd:int | The total number of records for this search. Depending on the pageSize value, some or all the records may be returned in this response. |
| pageSize | xsd:int | The page size for this search. |
| totalPages | xsd:int | The total number of pages that are part of this search. |
| pageIndex | xsd:int | The page index for the current set of results. |
| postingTransactionSummaryList | PostingTransactionSummaryList | Returns a list of available transaction summary results based on filters defined in your request. |

## PostingTransactionSummaryList {#bridgehead_N3502768}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| postingTransactionSummary | PostingTransactionSummary | Returns a list of available transactions that are filtered by and grouped by values specified in [PostingTransactionSummaryField](#bridgehead_N3500756) and [PostingTransactionSummaryFilter](#bridgehead_N3501157). |

## PostingTransactionSummary {#bridgehead_N3502897}

| Element Name | XSD Type | Notes |
| --- | --- | --- |
| period | RecordRef | Returns a summary based on period. |
| account | RecordRef | Returns a summary based on account. |
| parentItem | RecordRef | Returns a summary based on parent item. |
| item | RecordRef | Returns a summary based on item. |
| customer | RecordRef | Returns a summary based on customer. |
| department | RecordRef | Returns a summary based on department. |
| class | RecordRef | Returns a summary based on class. |
| location | RecordRef | Returns a summary based on location. |
| subsidiary | RecordRef | Returns a summary based on subsidiary. |
| book | RecordRef | If you use the Multi-Book Accounting feature, specify to group data by accounting book. |
| **amount** | double | Returns a summary based on amount. Important: This argument is required. |

## Faults {#bridgehead_N3503342}

This operation can throw one of the following faults. See [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html) for more information about faults.

-   InvalidSessionFault
    
-   InvalidCredentialsFault
    
-   ExceededRequestLimitFault
    
-   ExceededUsageLimitFault
    
-   ExceededRecordCountFault
    
-   ExceededRequestSizeFault
    
-   UnexpectedErrorFault
    

## Sample Code {#bridgehead_N3503417}

## Example One {#bridgehead_N3503426}

The sample provided shows how to get and print account values using the getPostingTransactionSummary operation.

## Java {#bridgehead_N3503459}

          `/* Make Record Ref out of an internalId */    public static RecordRef mrr(String internalId)    {       RecordRef toRet = new RecordRef();       toRet.setInternalId(internalId);       return toRet;    }    public void testPostingActivity() throws Exception { //c.setHttpPort(80); c.login(); PostingTransactionSummaryField pagb = new PostingTransactionSummaryField();       pagb.setParentItem(Boolean.TRUE);  /* pagb.set_class(Boolean.FALSE); pagb.setItem(Boolean.FALSE); pagb.setCustomer(Boolean.FALSE); pagb.setLocation(Boolean.FALSE); */  PostingTransactionSummaryFilter paf = new PostingTransactionSummaryFilter(); //paf.setAccount(new RecordRefList(new RecordRef[]{mrr("5"),mrr("12")})); long start = System.currentTimeMillis(); GetPostingTransactionSummaryResult res = c.getPort().getPostingTransactionSummary(pagb, paf, 1);  for (int i=0; i<10; i++) { if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getAccount() != null) System.out.println("Account:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getAccount().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getPeriod() != null) System.out.println("Period:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getPeriod().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getCustomer() != null) System.out.println("Customer:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getCustomer().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).get_class() != null) System.out.println("_class:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).get_class().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getDepartment() != null) System.out.println("Department:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getDepartment().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getLocation() != null) System.out.println("Location:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getLocation().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getSubsidiary() != null) System.out.println("Subsidiary:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getSubsidiary().getInternalId()); if (res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getItem() != null) System.out.println("Item:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getItem().getInternalId()); System.out.println("Amount:" + res.getPostingTransactionSummaryList().getPostingTransactionSummary(i).getAmount()); } for (int i=res.getPageIndex(); i<res.getTotalPages(); i++) { System.err.println("Elapsed Time : " + (System.currentTimeMillis() - start)); res = c.getPort().getPostingTransactionSummary(pagb,paf,i+1); } System.err.println("Elapsed Time : " + (System.currentTimeMillis() - start)); GetPostingTransactionSummaryResult p = c.getPort().getPostingTransactionSummary(pagb, paf, res.getTotalPages()+2); assertFalse(p.getStatus().isIsSuccess()); }` 
        

## Example Two {#bridgehead_N3503470}

The following SOAP and Java show how to get the posting activity for posting period 109. The sample prints the unconsolidated and consolidated amounts in the parent subsidiary by child subsidiary and account - for example, if subsidiary **2** is in Euros and subsidiary **1**, the parent company, is in dollars, show the amount in Euros and the amount in dollars for that account in period 109.

## SOAP Request {#bridgehead_N27135141}

          `<soapenv:Body>            <getPostingTransactionSummary xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <fields>                <ns6:period xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">true</ns6:period>                <ns7:account xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">true</ns7:account>                    <ns8:subsidiary xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">true<          ns8:subsidiary>             </fields>             <filters>                 <ns9:period xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                   <ns9:recordRef internalId="109"/>                </ns9:period>             </filters>             <pageIndex>1</pageIndex>            </getPostingTransactionSummary>        </soapenv:Body>` 
        

## SOAP Reponse {#bridgehead_N27135201}

          `<soapenv:Body>          <getPostingTransactionSummaryResponse       xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformCore:getPostingTransactionSummaryResult       xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                <platformCore:status isSuccess="true"/>                <platformCore:totalRecords>19</platformCore:totalRecords>                <platformCore:pageSize>1000</platformCore:pageSize>                <platformCore:totalPages>0</platformCore:totalPages>                <platformCore:pageIndex>1</platformCore:pageIndex>                <platformCore:postingTransactionSummaryList>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="2"/>                      <platformCore:subsidiary internalId="1"/>                      <platformCore:amount>500.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="6"/>                      <platformCore:subsidiary internalId="1"/>                      <platformCore:amount>19.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="6"/>                      <platformCore:subsidiary internalId="2"/>                      <platformCore:amount>5.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="6"/>                      <platformCore:subsidiary internalId="4"/>                      <platformCore:amount>6.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="6"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>-3.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="16"/>                      <platformCore:subsidiary internalId="6"/>                      <platformCore:amount>-4.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="24"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>-100.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="58"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>100.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="112"/>                      <platformCore:subsidiary internalId="1"/>                      <platformCore:amount>-496.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="112"/>                      <platformCore:subsidiary internalId="5"/>                      <platformCore:amount>-1.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="139"/>                      <platformCore:subsidiary internalId="4"/>                      <platformCore:amount>-9.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="142"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>3.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="145"/>                      <platformCore:subsidiary internalId="5"/>                      <platformCore:amount>1.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="148"/>                      <platformCore:subsidiary internalId="2"/>                      <platformCore:amount>-5.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="153"/>                      <platformCore:subsidiary internalId="6"/>                      <platformCore:amount>4.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="155"/>                      <platformCore:subsidiary internalId="1"/>                      <platformCore:amount>-23.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="175"/>                      <platformCore:subsidiary internalId="4"/>                      <platformCore:amount>3.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="186"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>0.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                   <platformCore:postingTransactionSummary>                      <platformCore:period internalId="109"/>                      <platformCore:account internalId="187"/>                      <platformCore:subsidiary internalId="8"/>                      <platformCore:amount>0.0</platformCore:amount>                   </platformCore:postingTransactionSummary>                </platformCore:postingTransactionSummaryList>             </platformCore:getPostingTransactionSummaryResult>          </getPostingTransactionSummaryResponse>       </soapenv:Body>` 
        

## Java {#bridgehead_N3503513}

          `/* Make Record Ref out of an internalId */    public static RecordRef mrr(String internalId)    {       RecordRef toRet = new RecordRef();       toRet.setInternalId(internalId);       return toRet;    }         public void testPostingWorkflow() throws Exception    {       c.setCredentials(CRED_DB96_SIC);       c.useRequestLevelCredentials();         // Show and group by subsidiary, period and account.       // These are basic columns. If you do not include account,       // all amounts will be 0.       PostingTransactionSummaryField pagb = new PostingTransactionSummaryField();       pagb.setSubsidiary(Boolean.TRUE);       pagb.setPeriod(Boolean.TRUE);       pagb.setAccount(Boolean.TRUE);         PostingTransactionSummaryFilter paf = new PostingTransactionSummaryFilter();       paf.setPeriod(new RecordRefList(new RecordRef[]{mrr("109")}));       GetPostingTransactionSummaryResult gestalt =          c.getPort().getPostingTransactionSummary(pagb,paf,1);       ConsolidatedExchangeRateFilter f = new ConsolidatedExchangeRateFilter();       f.setPeriod(mrr("109"));       f.setToSubsidiary(mrr("1"));       GetConsolidatedExchangeRateResult cerr = c.getPort().getConsolidatedExchangeRate(f);         for (PostingTransactionSummary unConsolidated :           gestalt.getPostingTransactionSummaryList().getPostingTransactionSummary())       {          ConsolidatedExchangeRate rate = null;          for (ConsolidatedExchangeRate testRate :             cerr.getConsolidatedExchangeRateList().getConsolidatedExchangeRate())          {             if                (testRate.getFromSubsidiary().getInternalId().equals                (unConsolidated.getSubsidiary().getInternalId()))             {                rate = testRate;                break;             }          }          if (rate == null)             continue;  // the Target Subsidiary will not have a conversion rate to itself.           System.out.println("\n\nFor Subsidiary: " + unConsolidated.getSubsidiary().getInternalId()  +             " to Consolidated Parent (1).\nPeriod: " + unConsolidated.getPeriod().getInternalId() +                   "\nAccount Id: " + unConsolidated.getAccount().getInternalId() +                    "\nUnconsolidated Amount is: " + unConsolidated.getAmount() +                   "\nConsolidated Amounts are (Avg/Historical/Current): "                      + (unConsolidated.getAmount()*rate.getAverageRate()) + " / " +                      (unConsolidated.getAmount()*rate.getHistoricalRate()) + " / " +                      (unConsolidated.getAmount()*rate.getCurrentRate()));       }    }` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html)
-   [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html)
-   [SOAP Web Services Standard Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3478008.html)
-   [SOAP Web Services List Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480490.html)
-   [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
