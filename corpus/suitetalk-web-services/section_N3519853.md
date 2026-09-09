---
id: "section_N3519853"
type: "section"
title: "Search-Related Sample Code"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Operations > search > Search-Related Sample Code"
parent: "section_N3514306"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3519853.html"
anchors: ["bridgehead_N3519940", "bridgehead_N27264151", "bridgehead_N27264291", "bridgehead_N27264471", "bridgehead_N27264531", "bridgehead_N3520026", "bridgehead_3819311291", "bridgehead_N27264741", "bridgehead_N27264801", "bridgehead_3819311637", "bridgehead_N27264961", "bridgehead_N27265021", "bridgehead_3987623272", "bridgehead_3987623425", "bridgehead_3987623353", "bridgehead_N3520104", "bridgehead_N3520212", "bridgehead_N27265751", "bridgehead_N27265811", "bridgehead_N27265871", "bridgehead_N3520255", "bridgehead_N27266031", "bridgehead_N3520280", "bridgehead_N27266231", "bridgehead_N27266291", "bridgehead_N27266351", "bridgehead_N3520331", "bridgehead_N3520363", "bridgehead_N27266711", "bridgehead_N27266771", "bridgehead_N27266841", "bridgehead_N3520409", "bridgehead_N27266961"]
sha256: "0d36cb7eb006b029c7d687854141993aeaf7673667f93981bde3e5098c2b1405"
---

Important:

In many cases, you can achieve the equivalent of SOAP operations using REST web services. For a comparison of available operations in SOAP and REST web services, see [SOAP Web Services vs. REST Web Services Operation Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164155878349.html).

See the following search-related code samples:

-   [Basic Search Code Sample](#bridgehead_N3519940)
    
-   [Joined Search Code Samples](#bridgehead_N3520026)
    
-   [Advanced Search Code Samples](#bridgehead_N3520104)
    
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
    

## Basic Search Code Sample {#bridgehead_N3519940}

## SOAP Request {#bridgehead_N27264151}

In the following example, customer records that have an email that contains shutterfly.com are searched for. Note that you can limit the search page size at the request level (see [pageSize](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423764)).

          `<soap:Body> <platformMsgs:search> <searchRecord xsi:type="ContactSearch">    <customerJoin xsi:type="CustomerSearchBasic">       <email operator='contains' xsi:type="platformCore:SearchStringField">       <platformCore:searchValue>shutterfly.com</platformCore:searchValue>       <email>    <customerJoin> </searchRecord> </search> </soap:Body>` 
        

## SOAP Response {#bridgehead_N27264291}

Notice that in this example, only one matching record was found. You can see that the page size was set such that if multiple records were found, only 10 would be returned at a time.

          `<soapenv:Body> <searchResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <searchResult xmlns="urn:core_2017_1.platform.webservices.netsuite.com"> <status isSuccess="true"/> <totalRecords>1</totalRecords> <pageSize>10</pageSize> <totalPages>1</totalPages> <pageIndex>1</pageIndex> <recordList>    <record internalId="983" xsi:type="ns1:Customer"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"     xmlns:ns1="urn:relationships_2017_1.lists.webservices.netsuite.com">       <ns1:entityId>Shutter Fly</ns1:entityId>       <ns1:isInactive>false</ns1:isInactive>       <ns1:companyName>Shutter Fly, Inc</ns1:companyName>       <ns1:entityStatus internalId="6"><name>LEAD-New</name>       .       .       .       <ns1:customFieldList>          <customField internalId="165" scriptId="custentity_map" xsi:type="StringCustomFieldRef">             <value>http://maps.google.com</value>          </customField>          <customField internalId="76" scriptId="custentity_had_order_problems"           xsi:type="BooleanCustomFieldRef"><value>false</value></customField>       </ns1:customFieldList>    </record> </recordList> </searchResult> </searchResponse> </soapenv:Body>` 
        

## C# {#bridgehead_N27264471}

          `private void searchCustomer() {       _out.writeLn( "\nEnter search parameters" );        // Instantiate a search object for customers. Note that the search    // object is different from the regular record used for add and update.    CustomerSearch custSearch = new CustomerSearch();        // Search the customer entity id which is a string field    _out.write( "Entity ID (press enter to skip): " );    String nameValue = _out.readLn();    SearchStringField entityId = null;    if ( !nameValue.Equals( "" ) )    {       entityId = new SearchStringField();       entityId.@operator = SearchStringFieldOperator.contains;       entityId.operatorSpecified = true;       entityId.searchValue = nameValue;       custSearch.basic.entityId = entityId; //see note below for an alternative    } //Note:  You could also use CustomerSearchBasic to access entityId directly, for example:       CustomerSearchBasic custSearchBasic = new CustomerSearchBasic();       custSearchBasic.entityId = entityId;     // Search the customer stage which is a list field    _out.write( "Customer Stage (one or more nsKeys separated by commas, press enter to skip): " );    String stageKeysValue = _out.readLn();    SearchMultiSelectField stage = null;    if ( !stageKeysValue.Equals( "" ) )    {       stage = new SearchMultiSelectField();       stage.@operator = SearchMultiSelectFieldOperator.anyOf;       stage.operatorSpecified = true;              string [] nskeys = stageKeysValue.Split( new Char[] {','} );              RecordRef[] recordRefs = new RecordRef[ stageKeysValue.Length ];       for (int i=0; i<nskeys.Length; i++ )       {          RecordRef recordRef = new RecordRef();          recordRef.internalId = nskeys[i];          recordRefs[i] = recordRef;       }       stage.searchValue = recordRefs;       custSearch.stage = stage;    }        // Search by isActive field which is a boolean    /*    SearchBooleanField isActive = new SearchBooleanField();    while ( true )    {       _out.write( "Is active [T/F] (default is T): " );       String upcomingStr = _out.readLn();              if ( "T".Equals( upcomingStr.ToUpper() ) || "".Equals( upcomingStr.ToUpper() ) )       {          isActive.searchValue = true;          isActive.searchValueSpecified = true;          break;       }       else if ( upcomingStr.ToUpper().Equals( "F" ) )       {          isActive.searchValue = false;          isActive.searchValueSpecified = true;          break;       }       else       {          _out.writeLn( "Invalid selection" );       }    }    custSearch.active = isActive;    */    if ( custSearch.entityId == null && custSearch.stage == null )    {       _out.info( "\nNo search criteria was specified. Searching for all records." );    }    else    {       _out.info(       "\nSearching for customers with the following criteria: " +       (entityId==null ? "" : ("\nentityID=" + custSearch.entityId.searchValue) + ",        Operator=" + entityId.@operator.ToString()) +       (stage==null ? "" : ("\nstage nsKeys='" + stageKeysValue + "',        Operator=" + stage.@operator.ToString())) );    }            // Invoke search() web services operation    SearchResult response = _service.search( custSearch );        // Process response    if ( response.status.isSuccess )    {       // Process the records returned in the response and print to console       processCustomerSearchResponse( response );              // Since pagination controls what is returned, verify       // if there are anymore pages to retrieve.       searchMore( response );    }    else    {       _out.error( getStatusDetails( response.status ) );    } }` 
        

## Java {#bridgehead_N27264531}

          `public void searchCustomer() throws RemoteException, ExceededUsageLimitFault, UnexpectedErrorFault, InvalidSessionFault, ExceededRecordCountFault {    _console.writeLn("\nEnter search parameters");        // Instantiate a search object for customers. Note that the search    // object is different from the regular record used for add and update.    CustomerSearch custSearch = new CustomerSearch();        // Search the customer entity id which is a string field    _console.write("Entity ID (press enter to skip): ");    String nameValue = _console.readLn();    SearchStringField entityId = null;    if (!nameValue.equals("")) {       entityId = new SearchStringField();       entityId.setOperator(SearchStringFieldOperator.contains);       entityId.setSearchValue(nameValue);       custSearch.setEntityId(entityId);    }        // Search the customer stage which is a list field    _console    .write("Customer Stage (one or more nsKeys separated by commas, press enter to skip): ");    String stageKeysValue = _console.readLn();    SearchMultiSelectField stage = null;    if (!stageKeysValue.equals("")) {       stage = new SearchMultiSelectField();       stage.setOperator(SearchMultiSelectFieldOperator.anyOf);              String[] nskeys = stageKeysValue.split(",");              RecordRef[] recordRefs = new RecordRef[stageKeysValue.length()];       for (int i = 0; i < nskeys.length; i++) {          RecordRef recordRef = new RecordRef();          recordRef.setInternalId(nskeys[i]);          recordRefs[i] = recordRef;       }       stage.setSearchValue(recordRefs);       custSearch.setStage(stage);    }    if (custSearch.getEntityId() == null && custSearch.getStage() == null) {       _console       .info("\nNo search criteria was specified. Searching for all records.");    } else {       _console       .info("\nSearching for customers with the following criteria: "       + (entityId == null ? ""       : ("\nentityId=" + custSearch       .getEntityId().getSearchValue())       + ", Operator="       + entityId.getOperator().toString())       + (stage == null ? "" : ("\nstage nsKeys='"       + stageKeysValue + "', Operator=" + stage       .getOperator().toString())));    }        // Set page size for number of records to be returned in search    // response        // Invoke search() web services operation    SearchResult result = _port.search(custSearch);        // Process result    if (result.getStatus().isIsSuccess()) {       // Process the records returned in the result and print to console       processCustomerSearchResponse(result);              // Since pagination controls what is returned, verify       // if there are anymore pages to retrieve.       searchMore(result);    } else {       _console.error(getStatusDetails(result.getStatus()));    } }` 
        

## Joined Search Code Samples {#bridgehead_N3520026}

## Customer Search With Contact Join Sample One {#bridgehead_3819311291}

This sample shows how to run a customer search in which the contact email address is specified as the search criteria.

## Java {#bridgehead_N27264741}

          `public void contactSearch_with_CustomerJoin() throws Exception {     ContactSearch cs = new ContactSearch();     ContactSearchBasic contactSearchBasic = new ContactSearchBasic();     contactSearchBasic.setEmail(new SearchStringField("contact@example.com", SearchStringFieldOperator.is));     CustomerSearchBasic customerSearchBasic = new CustomerSearchBasic();     customerSearchBasic.setEntityId(new SearchStringField("My Customer", SearchStringFieldOperator.is));     cs.setBasic(contactSearchBasic);     cs.setCustomerJoin(customerSearchBasic);     sessMgr.getWrappedPort().search(cs, this); }` 
        

## SOAP {#bridgehead_N27264801}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">        <searchRecord xsi:type="ns4:ContactSearch"       xmlns:ns4="urn:relationships_2017_1.lists.webservices.netsuite.com">                <ns4:basic xsi:type="ns5:ContactSearchBasic"       xmlns:ns5="urn:common_2017_1.platform.webservices.netsuite.com">                   <ns5:email operator="is" xsi:type="ns6:SearchStringField"       xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">                      <ns6:searchValue xsi:type="xsd:string">contact@example.com</ns6:searchValue>                   </ns5:email>                </ns4:basic>                <ns4:customerJoin xsi:type="ns7:CustomerSearchBasic"       xmlns:ns7="urn:common_2017_1.platform.webservices.netsuite.com">                   <ns7:entityId operator="is" xsi:type="ns8:SearchStringField"       xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                      <ns8:searchValue xsi:type="xsd:string">My Customer</ns8:searchValue>                   </ns7:entityId>                </ns4:customerJoin>             </searchRecord>          </search>` 
        

## Contact Search With Customer Join Sample Two {#bridgehead_3819311637}

The following sample shows how to return an associated joined list of records. In this case, all contacts associated with customers of internalId 1, 2 and 3 are returned.

## Java {#bridgehead_N27264961}

          `RecordRef[] rr = new RecordRef[]{new RecordRef("1", RecordType.customer),     new RecordRef("2", RecordType.customer), new RecordRef("3", RecordType.customer)};    CustomerSearchBasic customerSearchBasic = new CustomerSearchBasic();    customerSearchBasic.setInternalId(new SearchMultiSelectField(rr,     SearchMultiSelectFieldOperator.anyOf));    ContactSearch contactSearch = new ContactSearch();    contactSearch.setCustomerJoin(customerSearchBasic);` 
        

## SOAP {#bridgehead_N27265021}

          `<soapenv:Body>    <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">    <searchRecord xsi:type="ns1:ContactSearch"        xmlns:ns1="urn:relationships_2017_1.lists.webservices.netsuite.com">       <ns1:customerJoin xsi:type="ns2:CustomerSearchBasic"           xmlns:ns2="urn:common_2017_1.platform.webservices.netsuite.com">          <ns2:internalId operator="anyOf" xsi:type="ns3:SearchMultiSelectField"              xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">             <ns3:searchValue internalId="1" type="customer"              xsi:type="ns3:RecordRef"/>             <ns3:searchValue internalId="2" type="customer"               xsi:type="ns3:RecordRef"/>             <ns3:searchValue internalId="3" type="customer"              xsi:type="ns3:RecordRef"/>          </ns2:internalId>       </ns1:customerJoin>    </searchRecord>    </search> </soapenv:Body>` 
        

## Item Search With Pricing Join Sample Three {#bridgehead_3987623272}

The following sample shows how to search for all items that have a price level of 10.00.

## C# {#bridgehead_3987623425}

          `private void myItemSearch() {              ItemSearchBasic myItemSearchBasic = new ItemSearchBasic();     SearchEnumMultiSelectField myEnum = new SearchEnumMultiSelectField();    myEnum.@operator = SearchEnumMultiSelectFieldOperator.anyOf;    myEnum.operatorSpecified = true;    String[] searchStringArray = new String[1];    searchStringArray[0] = "_inventoryItem";    myEnum.operatorSpecified = true;    myEnum.searchValue = searchStringArray;             myItemSearchBasic.type = myEnum;                                     PricingSearchBasic myPricingSearchBasic = new PricingSearchBasic();                 SearchDoubleField rateValue = new SearchDoubleField();    rateValue.@operator = SearchDoubleFieldOperator.equalTo;    rateValue.operatorSpecified = true;    rateValue.searchValue = 10.00;    rateValue.searchValueSpecified = true;     myPricingSearchBasic.rate = rateValue;      ItemSearch myItemSearch = new ItemSearch();    myItemSearch.basic = myItemSearchBasic;    myItemSearch.pricingJoin = myPricingSearchBasic;                        SearchResult searchResult = _service.search(myItemSearch); }` 
        

## SOAP Request {#bridgehead_3987623353}

          `<soap:Body>    <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <searchRecord xmlns:q1="urn:accounting_2017_1.lists.webservices.netsuite.com" xsi:type="q1:ItemSearch">          <q1:basic>             <type operator="anyOf" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_inventoryItem</searchValue>             </type>          </q1:basic>         <q1:pricingJoin>             <rate operator="equalTo" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">10</searchValue>             </rate>          </q1:pricingJoin>       </searchRecord>    </search> </soap:Body>` 
        

## Advanced Search Code Samples {#bridgehead_N3520104}

The following advanced search samples are provided.

1.  [Perform a search that includes a saved search ID.](#bridgehead_N3520212)
    
2.  [Perform a search with a defined page size.](#bridgehead_N3520255)
    
3.  [Perform a search in which you override search columns in a saved search.](#bridgehead_N3520280)
    
4.  [Perform a search in which you specify additional saved search criteria.](#bridgehead_N3520331)
    
5.  [Programmatically manipulate data returned by a search](#bridgehead_N3520409)
    

## Perform a search that includes a saved search ID. {#bridgehead_N3520212}

## C# {#bridgehead_N27265751}

          `// Create a service  NetSuiteService nss = new NetSuiteService();  // Perform the search. Note that you can get the saved search ID using  // either getSavedSearch() or through the UI TransactionSearchAdvanced tsa1 = new TransactionSearchAdvanced(); tsa1.savedSearchId="57";  //substitute your own saved search internal ID nss.search(tsa1);` 
        

## SOAP Request {#bridgehead_N27265811}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <searchRecord xmlns:q1="urn:sales_2017_1.transactions.webservices.netsuite.com"    xsi:type="q1:TransactionSearchAdvanced" savedSearchId="57" /> </search>` 
        

## SOAP Response {#bridgehead_N27265871}

          `// The default is to return search rows <platformCore:searchRow xsi:type="tranSales:TransactionSearchRow"    xmlns:tranSales="urn:sales_2017_1.transactions.webservices.netsuite.com"> <tranSales:basic xmlns:platformCommon="urn:common_2017_1.platform.webservices.netsuite.com"> <platformCommon:account> <platformCore:searchValue internalId="125"/> </platformCommon:account> <platformCommon:amount> <platformCore:searchValue>12481.9</platformCore:searchValue> </platformCommon:amount> <platformCommon:entity> <platformCore:searchValue internalId="78"/> </platformCommon:entity> <platformCommon:mainline> <platformCore:searchValue>false</platformCore:searchValue> </platformCommon:mainline> <platformCommon:number> <platformCore:searchValue>102</platformCore:searchValue> </platformCommon:number> <platformCommon:postingPeriod> <platformCore:searchValue internalId="72"/> </platformCommon:postingPeriod> <platformCommon:tranDate> <platformCore:searchValue>2005-02-10T00:00:00.000-08:00</platformCore:searchValue> </platformCommon:tranDate> <platformCommon:tranId> <platformCore:searchValue>102</platformCore:searchValue> </platformCommon:tranId> <platformCommon:type> <platformCore:searchValue internalId="SalesOrd"/> </platformCommon:type> </tranSales:basic> </platformCore:searchRow>` 
        

## Perform a search with a defined page size. {#bridgehead_N3520255}

This sample performs the same search as the previous sample, however, you are specifying the number of results that are returned per page.

## C# {#bridgehead_N27266031}

          `TransactionSearchAdvanced tsa2 = new TransactionSearchAdvanced(); tsa2.savedSearchId="57";  //substitute your own saved search internal ID  // Set search preference to return search columns SearchPreferences sp = new SearchPreferences(); sp.pageSizeSpecified = true; sp.pageSize = 10; nss.searchPreferences = sp; nss.search(tsa2);` 
        

## Perform a search in which you override search columns in a saved search. {#bridgehead_N3520280}

In this sample you are returning a specific saved search (57), and then overriding the search return columns in the saved search and specifying your own search return columns.

## C# {#bridgehead_N27266231}

          `TransactionSearchAdvanced tsa3 = new TransactionSearchAdvanced(); tsa3.savedSearchId="57";  //substitute your own saved search internal ID  // Set search preference to return search columns // Already defined returnSearchColumns //SearchPreferences sp = new SearchPreferences(); //sp.returnSearchColumns = true; //nss.searchPreferences = sp;  // Instantiate SearchColumn object TransactionSearchRow tsr = new TransactionSearchRow(); TransactionSearchRowBasic tsrb = new TransactionSearchRowBasic();  // return internId SearchColumnSelectField [] orderIdCols = new SearchColumnSelectField[1]; SearchColumnSelectField orderIdCol = new SearchColumnSelectField(); orderIdCol.customLabel = "Sales Order ID"; // Define a custom label orderIdCols[0] = orderIdCol; tsrb.internalId = orderIdCols;  SearchColumnDateField [] tranDateCols = new SearchColumnDateField[1]; SearchColumnDateField tranDateCol = new SearchColumnDateField(); tranDateCols[0] = tranDateCol; tsrb.tranDate = tranDateCols; SearchColumnBooleanField [] isFulfilledCols = new SearchColumnBooleanField[1]; SearchColumnBooleanField isFulfilledCol = new SearchColumnBooleanField(); isFulfilledCol.customLabel = "Order Fulfilled"; // Define a custom label isFulfilledCols[0] = isFulfilledCol; tsrb.shipRecvStatus = isFulfilledCols;  tsr.basic = tsrb; tsa3.columns = tsr; nss.search(tsa3);` 
        

## SOAP Request {#bridgehead_N27266291}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <searchRecord xmlns:q1="urn:sales_2017_1.transactions.webservices.netsuite.com"       xsi:type="q1:TransactionSearchAdvanced" savedSearchId="57">                   <q1:columns>                      <q1:basic>                         <internalId xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                            <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Sales Order ID          </customLabel>                         </internalId>                         <shipRecvStatus xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                            <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Order Fulfilled          </customLabel>                         </shipRecvStatus>                         <tranDate xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                      </q1:basic>                   </q1:columns>                </searchRecord>             </search>` 
        

## SOAP Response {#bridgehead_N27266351}

          `<platformCore:searchRow xsi:type="tranSales:TransactionSearchRow"    xmlns:tranSales="urn:sales_2017_1.transactions.webservices.netsuite.com">         <tranSales:basic xmlns:platformCommon="urn:common_2017_1.platform.webservices.netsuite.com">                      <platformCommon:internalId>                      <platformCore:searchValue internalId="117"/>                     <platformCore:customLabel>Sales Order ID</platformCore:customLabel>                     </platformCommon:internalId>                     <platformCommon:tranDate>                     <platformCore:searchValue>2005-04-23T00:00:00.000-07:00</platformCore:searchValue>                     </platformCommon:tranDate>                      </tranSales:basic>                      </platformCore:searchRow>` 
        

## Perform a search in which you specify additional saved search criteria. {#bridgehead_N3520331}

The next sample shows how to take a saved search and specify additional search filter criteria. The additional search critera will not override the criteria already defined in the saved search.

## C# {#bridgehead_N3520363}

          `TransactionSearchAdvanced tsa4 = new TransactionSearchAdvanced(); tsa4.savedSearchId="57";  TransactionSearch ts = new TransactionSearch(); TransactionSearchBasic tsb = new TransactionSearchBasic(); // condition 1: on SO only SearchEnumMultiSelectField semsfTranType = new SearchEnumMultiSelectField(); semsfTranType.operatorSpecified = true; semsfTranType.@operator = SearchEnumMultiSelectFieldOperator.anyOf; String [] tranTypes = new String[1]; String tranType = "_salesOrder"; tranTypes[0] = tranType; semsfTranType.searchValue = tranTypes; tsb.type = semsfTranType;  // condition 2: tranId contains 182 SearchStringField sfTranId = new SearchStringField(); sfTranId.searchValue = "182"; // tranId contains 11 sfTranId.@operator = SearchStringFieldOperator.contains; sfTranId.operatorSpecified = true; tsb.tranId=sfTranId;  // condition 3: Is MultiShipping Routes enabled SearchBooleanField sbfShipLineEnabled = new SearchBooleanField(); sbfShipLineEnabled.searchValue = true; sbfShipLineEnabled.searchValueSpecified = true; tsb.shipping = sbfShipLineEnabled;  // condition 4: Open SO SearchBooleanField sbfTranStatus = new SearchBooleanField(); sbfTranStatus.searchValue = true; sbfTranStatus.searchValueSpecified = true; tsb.shipRecvStatusLine = sbfTranStatus;  ts.basic = tsb; tsa4.criteria = ts; tsa4.columns = tsr; //note - columns previously defined above. nss.search(tsa4);` 
        

## SOAP Request {#bridgehead_N27266711}

          `<searchRecord xmlns:q1="urn:sales_2017_1.transactions.webservices.netsuite.com" xsi:type="q1:TransactionSearchAdvanced">                <q1:criteria>                   <q1:basic>                      <tranId operator="contains" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">182</searchValue>                      </tranId>                      <type operator="anyOf" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_salesOrder          </searchValue>                      </type>                   </q1:basic>                </q1:criteria>                <q1:columns>                   <q1:basic>                      <internalId xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Sales Order ID          </customLabel>                      </internalId>                      <shipRecvStatus xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Order Fulfilled          </customLabel>                      </shipRecvStatus>                      <shipRecvStatusLine xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">          Order Line Fulfilled</customLabel>                      </shipRecvStatusLine>                      <tranDate xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                      <tranId xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                   </q1:basic>                </q1:columns>             </searchRecord>` 
        

## SOAP Request (with Shipping and ShipRecvStatusLine criteria) {#bridgehead_N27266771}

          `<searchRecord xmlns:q1="urn:sales_2017_1.transactions.webservices.netsuite.com"    xsi:type="q1:TransactionSearchAdvanced">                <q1:criteria>                   <q1:basic>                      <shipRecvStatus xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">true</searchValue>                      </shipRecvStatus>                      <tranId operator="contains" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">11</searchValue>                      </tranId>                      <type operator="anyOf" xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <searchValue xmlns="urn:core_2017_1.platform.webservices.netsuite.com">_salesOrder          </searchValue>                      </type>                   </q1:basic>                </q1:criteria>                <q1:columns>                   <q1:basic>                      <internalId xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Sales Order ID          </customLabel>                      </internalId>                      <shipRecvStatus xmlns="urn:common_2017_1.platform.webservices.netsuite.com">                         <customLabel xmlns="urn:core_2017_1.platform.webservices.netsuite.com">Order Fulfilled          </customLabel>                      </shipRecvStatus>                      <tranDate xmlns="urn:common_2017_1.platform.webservices.netsuite.com" />                   </q1:basic>                </q1:columns>             </searchRecord>` 
        

## SOAP Response {#bridgehead_N27266841}

          `<platformCore:searchRow xsi:type="tranSales:TransactionSearchRow" xmlns:tranSales="urn:sales_2017_1.transactions.webservices.netsuite.com">     <tranSales:basic xmlns:platformCommon="urn:common_2017_1.platform.webservices.netsuite.com">                         <platformCommon:internalId>                            <platformCore:searchValue internalId="986"/>                            <platformCore:customLabel>Sales Order ID</platformCore:customLabel>                         </platformCommon:internalId>                         <platformCommon:shipRecvStatusLine>                            <platformCore:searchValue>true</platformCore:searchValue>                            <platformCore:customLabel>Order Line Fulfilled</platformCore:customLabel>                         </platformCommon:shipRecvStatusLine>                         <platformCommon:tranDate>                            <platformCore:searchValue>2008-09-11T00:00:00.000-07:00</platformCore:searchValue>                         </platformCommon:tranDate>                      </tranSales:basic>                   </platformCore:searchRow>` 
        

## Programmatically manipulate data returned by a search {#bridgehead_N3520409}

## Java {#bridgehead_N27266961}

          `public void searchCustomerBySavedSearch() throws RemoteException {         this.login(true);                  CustomerSearchAdvanced searchRecord = new CustomerSearchAdvanced();         searchRecord.setSavedSearchId("26"); // A saved customer search                  SearchResult result = _port.search(searchRecord);                  if( result.getTotalRecords() > 0 ) {                 // retain the search ID  to get more pages                 String sSearchId = result.getSearchId();                                  SearchRowList rowList = result.getSearchRowList();                                  processRowList(rowList);                                  int iNumPages = result.getTotalPages();                                  for ( int i=2; i<=iNumPages; i++) {                         result = _port.searchMoreWithId(sSearchId, i);                         rowList = result.getSearchRowList();                                                  processRowList(rowList);                 }                 } }   public void processRowList(SearchRowList rowList) {         for (int i=0; i<rowList.getSearchRow().length; i++) {                 CustomerSearchRow row = (CustomerSearchRow) rowList.getSearchRow(i);                 CustomerSearchRowBasic basic = row.getBasic();                                  SearchColumnStringField companyName = basic.getCompanyName(0);                                  _console.write("Company Name: "+companyName.getSearchValue());                 if (basic.getEmail(0).getSearchValue() != null) {                         String email = basic.getEmail(0).getSearchValue();                         _console.write("\tEmail: "+email);                 }                 if (basic.getPhone(0).getSearchValue() != null) {                         String phone = basic.getPhone(0).getSearchValue();                         _console.write("\tPhone: "+phone);                 }                 _console.writeLn("\n");         } }` 
        

### Related Topics

-   [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html)
-   [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html)
-   [Joined Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516345.html)
-   [Advanced Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3516862.html)
-   [Joining Through Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770131952.html)
-   [Setting Valid Search Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518134.html)
-   [Setting the anyof, mine, or myteam Filtering Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518157.html)
-   [Searching by lastModifiedDate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518534.html)
-   [Understanding Sorting in Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3518731.html)
-   [Searching for a Multi-select Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3522048.html)
-   [Search Issues and Best Practices for SOAP Web Services and SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519647409.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
