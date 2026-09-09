---
id: "section_N3659492"
type: "section"
title: "Transaction Search"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Searches > Transaction Search"
parent: "chapter_4177763939"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html"
anchors: ["bridgehead_1540381495", "bridgehead_N3659641", "bridgehead_N28291051", "bridgehead_N28291111"]
sha256: "9c49e399cc0cf483a9ddc38c94b0199f54bcd63feb188207529cf2a9acd85853"
---

Nearly all transaction record types use the TransactionSearch record for search. The _basic_ element in this record references the TransactionSearchBasic record, which lists all available search filter fields available in a transaction search.

The TransactionSearch record also lists all search joins available in a transaction search. For details, see the SOAP Schema Browser's [TransactionSearch](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/search/transactionsearch.html?mode=package) reference page.

Be aware that the actual search filter fields available will vary depending on the transaction type you are searching against. Not _all_ of the search filter fields defined in TransactionSearchBasic will exist on every single transaction type. For example, the Check transaction type may include search filter fields not available on the Journal Entry type. However, search filters values for both record types will be defined in TransactionSearchBasic.

A TransactionSearchAdvanced request with specified columns returns every tranLine as a record. For example, if a sales order contains 1 item line, search results include up to 3 records, depending on the accounts that are touched. This behavior is the same behavior as transaction search in the UI. By contrast, TransactionSearchBasic, and TransactionSearchAdvanced without specified columns, return the whole transaction record. For example, if a search returns a sales order with 3 item lines, search results consist of one record, with ItemList containing 3 items. These operations return basically the same results as a get() operation.

Note:

The Opportunity and the Time Bill records are the only transaction types that have their own search interfaces. For details, see the SOAP Schema Browser's [OpportunitySearch](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/search/opportunitysearch.html?mode=package) and [TimeBillSearch](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/search/timebillsearch.html?mode=package) reference pages.

          `// the sales order RecordRef salesOrderRef = new RecordRef(); salesOrderRef.setInternalId("873"); TransactionSearchBasic tranSearch = new TransactionSearchBasic(); // type is item fulfill tranSearch.setType( new SearchEnumMultiSelectField( new String [] {RecordType.itemFulfillment.getValue()}, SearchEnumMultiSelectFieldOperator.anyOf)); // created from our sales order tranSearch.setCreatedFrom( new SearchMultiSelectField( new RecordRef [] { salesOrderRef }, SearchMultiSelectFieldOperator.anyOf)); SearchResult result = c.search(tranSearch);` 
        

          `//And the outgoing search SOAP looks like this: <search xmlns="urn:messages_2017_1.platform.webservices.netsu ite.com">  <searchRecord xsi:type="ns1:TransactionSearchBasic" xmlns:ns1="urn:common_2017_1.platform.webservices.netsuite.com">  <ns1:createdFrom operator="anyOf" xsi:type="ns2:SearchMultiSelectField" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">  <ns2:searchValue internalId="873" xsi:type="ns2:RecordRef"/>  </ns1:createdFrom>  <ns1:type operator="anyOf" xsi:type="ns3:SearchEnumMultiSelectField" xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">  <ns3:searchValue xsi:type="xsd:string">itemFulfillment</ns3:searchValue>  </ns1:type>  </searchRecord>  </search>` 
        

Important:

By default only a record's body fields are returned on a search. Therefore, you must set the **bodyFieldsOnly** element of the SearchPreferences type to **false** if you want to also return the information specified on a record's sublist. For general information on searching in SOAP web services, see [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html).

## Usage Notes {#bridgehead_1540381495}

The following transaction searches are _not_ supported in SOAP web services:

-   Blanket Purchase Order
    
-   CCard Refund
    
-   Commission
    
-   Credit Card
    
-   Currency Revaluation
    
-   Customer Payment Authorization
    
-   Deprecated Custom Transaction
    
-   Finance Charge
    
-   Fulfillment Request
    
-   GL Impact Adjustment
    
-   Inventory Count
    
-   Inventory Distribution
    
-   Inventory Status Change
    
-   Inventory Worksheet
    
-   Liability Adjustment
    
-   Ownership Transfer
    
-   Payroll Adjustment
    
-   Payroll Liability Check
    
-   Period End Journal
    
-   Purchase Contract
    
-   Request For Quote
    
-   Revenue Arrangement
    
-   Revenue Commitment
    
-   Revenue Commitment Reversal
    
-   Revenue Contract
    
-   Sales Tax Payment
    
-   Statement Charge
    
-   Store Pickup Fulfillment
    
-   System Journal
    
-   Tax Liability Cheque
    
-   Tegata Payable
    
-   Tegata Receivable
    
-   Transfer
    
-   Vendor Request For Quote
    

## Sample Code {#bridgehead_N3659641}

The following sample returns three records, including one that was modified within two minutes the search was made.

## SOAP Request {#bridgehead_N28291051}

          `<soapenv:Body>  <search xmlns="urn:messages_2017_1.platform.webservices.netsu ite.com">  <searchRecord xsi:type="ns9:TransactionSearchBasic" xmlns:ns9="urn:common_2017_1.platform.webservices.netsuite.com">  <ns9:lastModifiedDate operator="onOrAfter" xsi:type="ns10:SearchDateField" xmlns:ns10="urn:core_2017_1.platform.webservices.nets uite.com"> <ns10:predefinedSearchValue xsi:type="ns11:SearchDate" xmlns:ns11="urn:types.core_2017_1.platform.webservices.netsuite.com">today</ns10:predefinedSearchValue> </ns9:lastModifiedDate>  <ns9:type operator="anyOf" xsi:type="ns12:SearchEnumMultiSelectField" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"> <ns12:searchValue xsi:type="xsd:string">_salesOrder</ns12:searchValue> </ns9:type> </searchRecord> </search> </soapenv:Body>` 
        

## Java {#bridgehead_N28291111}

          `TransactionSearchBasic basic = new TransactionSearchBasic();   SearchEnumMultiSelectField soType = new SearchEnumMultiSelectField(); soType.setSearchValue(new String[1]); soType.setSearchValue(0, TransactionType.__salesOrder); soType.setOperator(SearchEnumMultiSelectFieldOperator.anyOf); basic.setType(soType);   SearchDateField todayLastMod = new SearchDateField(); todayLastMod.setOperator(SearchDateFieldOperator.o nOrAfter); todayLastMod.setPredefinedSearchValue(SearchDate.t oday);   basic.setLastModifiedDate(todayLastMod);` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
