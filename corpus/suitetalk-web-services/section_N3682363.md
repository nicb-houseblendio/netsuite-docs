---
id: "section_N3682363"
type: "section"
title: "Item Supply Plan"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Item Supply Plan"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3682363.html"
anchors: ["bridgehead_N3682439", "bridgehead_N3683310", "bridgehead_N3683348", "bridgehead_N3683367", "bridgehead_N3683379", "bridgehead_N3683391", "bridgehead_N3683408", "bridgehead_N3683420", "bridgehead_N3683436", "bridgehead_N3683448", "bridgehead_N3683465", "bridgehead_N3683477"]
sha256: "88b545d3093ab5b95ddbb8d87b08155f31142dca19c26401ad12a88f8691f3d9"
---

An item supply plan lists the purchase orders or work orders required to ensure that item quantity meets expected demand.

Importing item supply plan data through SOAP web services is similar to creating a manual item supply plan in the NetSuite user interface. This type of item supply plan is not derived from any demand plan in the NetSuite system and can be based on data or projections from external sources.

For information about working with this record in the UI, see [Creating Item Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html).

Important:

Only one item supply plan per item is supported.

The schema for this record includes:

-   Body fields used to identify the record, such as externalId, internalId, item, location (when Multi-Location Inventory is enabled), memo, subsidiary (for NetSuite OneWorld), and units (when Multiple Units of Measure is enabled).
    
    Note the following:
    
    -   You must provide externalId or iInternal ID values to uniquely identify items, because the Item field may have non-unique values.
        
    -   Values for item, location, and units fields cannot be changed in update operations.
        
-   ItemSupplyPlanOrderList sublist fields that define data for the orders needed to replenish the supply of items.
    

The item supply plan record is defined in the [transactions demandPlanning](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/demandPlanning.xsd) XSD.

## Supported Operations {#bridgehead_N3682439}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3683310}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [item supply plan](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/itemsupplyplan.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3683348}

The item, location, and units body fields cannot be changed in update operations.

An item supply plan's receiptDate cannot be earlier than the orderDate.

The orderCreated field is read-only. It is set to True when an order is generated from an item supply plan.

## Code Samples {#bridgehead_N3683367}

Each of the following examples creates an item supply plan with two order lines.

## SOAP Request {#bridgehead_N3683379}

          `/* SOAP request    <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record externalId="Grape15763464" xsi:type="ns6:ItemSupplyPlan" xmlns:ns6="urn:demandplanning_2017_1.transactions.webservices.netsuite.com">                    <ns6:location internalId="1" type="location" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:item internalId="21" type="inventoryItem" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:orderList replaceAll="false" xsi:type="ns6:ItemSupplyPlanOrderList">                        <ns6:itemSupplyPlanOrder xsi:type="ns6:ItemSupplyPlanOrder">                            <ns6:orderDate xsi:type="xsd:dateTime">2012-06-11T16:30:04.593Z</ns6:orderDate>                            <ns6:receiptDate xsi:type="xsd:dateTime">2012-06-11T16:30:04.593Z</ns6:receiptDate>                            <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                            <ns6:orderType xsi:type="ns9:ItemSupplyPlanOrderType" xmlns:ns9="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns6:orderType>                        </ns6:itemSupplyPlanOrder>                        <ns6:itemSupplyPlanOrder xsi:type="ns6:ItemSupplyPlanOrder">                            <ns6:orderDate xsi:type="xsd:dateTime">2012-07-04T16:30:04.593Z</ns6:orderDate>                            <ns6:receiptDate xsi:type="xsd:dateTime">2012-07-12T16:30:04.593Z</ns6:receiptDate>                            <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                            <ns6:orderType xsi:type="ns10:ItemSupplyPlanOrderType" xmlns:ns10="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns6:orderType>                        </ns6:itemSupplyPlanOrder>                    </ns6:orderList>                </record>       </add>     */` 
        

## Java {#bridgehead_N3683391}

          `public void addItemSupplyPlan() throws Exception     {        this.login(true);                ItemSupplyPlan isp = new ItemSupplyPlan();              RecordRef rrSubsidiary = new RecordRef();       rrSubsidiary.setInternalId("1");       rrSubsidiary.setType(RecordType.subsidiary);       isp.setSubsidiary(Util.makeRecordRef("1"));               RecordRef rrLocation = new RecordRef();       rrLocation.setInternalId("1");       rrLocation.setType(RecordType.location);       isp.setLocation(rrLocation);              RecordRef rrItem1 = new RecordRef();       rrItem1.setInternalId("21");       rrItem1.setType(RecordType.inventoryItem);       isp.setItem(rrItem1);              ItemSupplyPlanOrderList ispl = new ItemSupplyPlanOrderList();       ItemSupplyPlanOrder[] ispo =  new ItemSupplyPlanOrder[2];              ispo[0] = new ItemSupplyPlanOrder();              Calendar c = Calendar.getInstance();       c.set(2012, 5, 12);       ispo[0].setOrderDate(c);              Calendar c2 = Calendar.getInstance();       c2.set(2012, 5, 12);       ispo[0].setReceiptDate(c2);              ispo[0].setQuantity(3.0);       ispo[0].setOrderType(ItemSupplyPlanOrderType._purchaseOrder);                ispo[1] = new ItemSupplyPlanOrder();                  Calendar c3 = Calendar.getInstance();       c3.set(2012, 6, 05);       ispo[1].setOrderDate(c3);              Calendar c4 = Calendar.getInstance();       c4.set(2012, 6, 13);       ispo[1].setReceiptDate(c4);              ispo[1].setQuantity(3.0);       ispo[1].setOrderType(ItemSupplyPlanOrderType._purchaseOrder);                ispl.setItemSupplyPlanOrder(ispo);         isp.setOrderList(ispl);                _port.add(isp);     }` 
        

Each of the following examples uses the addList operation.

## SOAP Request {#bridgehead_N3683408}

          `/*          <soapenv:Body>            <addList xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record externalId="Grape16979713" xsi:type="ns6:ItemSupplyPlan" xmlns:ns6="urn:demandplanning_2017_1.transactions.webservices.netsuite.com">                    <ns6:location internalId="1" type="location" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:item internalId="21" type="inventoryItem" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns6:orderList replaceAll="false" xsi:type="ns6:ItemSupplyPlanOrderList">                        <ns6:itemSupplyPlanOrder xsi:type="ns6:ItemSupplyPlanOrder">                            <ns6:orderDate xsi:type="xsd:dateTime">2012-06-11T16:42:59.250Z</ns6:orderDate>                            <ns6:receiptDate xsi:type="xsd:dateTime">2012-06-11T16:42:59.250Z</ns6:receiptDate>                            <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                            <ns6:orderType xsi:type="ns9:ItemSupplyPlanOrderType" xmlns:ns9="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns6:orderType>                        </ns6:itemSupplyPlanOrder>                        <ns6:itemSupplyPlanOrder xsi:type="ns6:ItemSupplyPlanOrder">                            <ns6:orderDate xsi:type="xsd:dateTime">2012-07-04T16:42:59.250Z</ns6:orderDate>                            <ns6:receiptDate xsi:type="xsd:dateTime">2012-07-12T16:42:59.250Z</ns6:receiptDate>                            <ns6:quantity xsi:type="xsd:double">3.0</ns6:quantity>                            <ns6:orderType xsi:type="ns10:ItemSupplyPlanOrderType" xmlns:ns10="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns6:orderType>                        </ns6:itemSupplyPlanOrder>                    </ns6:orderList>                </record>                <record externalId="Strawberry10442165" xsi:type="ns11:ItemSupplyPlan" xmlns:ns11="urn:demandplanning_2017_1.transactions.webservices.netsuite.com">                    <ns11:location internalId="1" type="location" xsi:type="ns12:RecordRef" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns11:item internalId="22" type="inventoryItem" xsi:type="ns13:RecordRef" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                    <ns11:orderList replaceAll="false" xsi:type="ns11:ItemSupplyPlanOrderList">                        <ns11:itemSupplyPlanOrder xsi:type="ns11:ItemSupplyPlanOrder">                            <ns11:orderDate xsi:type="xsd:dateTime">2012-06-11T16:42:59.250Z</ns11:orderDate>                            <ns11:receiptDate xsi:type="xsd:dateTime">2012-06-11T16:42:59.250Z</ns11:receiptDate>                            <ns11:quantity xsi:type="xsd:double">3.0</ns11:quantity>                            <ns11:orderType xsi:type="ns14:ItemSupplyPlanOrderType" xmlns:ns14="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns11:orderType>                        </ns11:itemSupplyPlanOrder>                        <ns11:itemSupplyPlanOrder xsi:type="ns11:ItemSupplyPlanOrder">                            <ns11:orderDate xsi:type="xsd:dateTime">2012-07-04T16:42:59.250Z</ns11:orderDate>                            <ns11:receiptDate xsi:type="xsd:dateTime">2012-07-12T16:42:59.250Z</ns11:receiptDate>                            <ns11:quantity xsi:type="xsd:double">3.0</ns11:quantity>                            <ns11:orderType xsi:type="ns15:ItemSupplyPlanOrderType" xmlns:ns15="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns11:orderType>                         </ns11:itemSupplyPlanOrder>                    </ns11:orderList>                </record>            </addList>        </soapenv:Body>        */` 
        

## Java {#bridgehead_N3683420}

          `public void addListItemSupplyPlan() throws Exception     {        this.login(true);         ItemSupplyPlan[] isp = new ItemSupplyPlan[2];              ItemSupplyPlanOrderList ispl = new ItemSupplyPlanOrderList();        ItemSupplyPlanOrder[] ispo =  new ItemSupplyPlanOrder[2];               ispo[0] = new ItemSupplyPlanOrder();                Calendar c = Calendar.getInstance();         c.set(2012, 5, 12);        ispo[0].setOrderDate(c);               Calendar c2 = Calendar.getInstance();        c2.set(2012, 5, 12);        ispo[0].setReceiptDate(c2);                 ispo[0].setQuantity(3.0);         ispo[0].setOrderType(ItemSupplyPlanOrderType._purchaseOrder);                 ispo[1] = new ItemSupplyPlanOrder();                Calendar c3 = Calendar.getInstance();        c3.set(2012, 6, 05);        ispo[1].setOrderDate(c3);               Calendar c4 = Calendar.getInstance();        c4.set(2012, 6, 13);        ispo[1].setReceiptDate(c4);                ispo[1].setQuantity(3.0);         ispo[1].setOrderType(ItemSupplyPlanOrderType._purchaseOrder);                           RecordRef[] rrItem = new RecordRef[2];         rrItem[0] =  new RecordRef();        rrItem[0].setInternalId("21");        rrItem[0].setType(RecordType.inventoryItem);                rrItem[1] =  new RecordRef();        rrItem[1].setInternalId("22");        rrItem[1].setType(RecordType.inventoryItem);                     for(int i = 0; i < 2; i++){                     isp[i] = new ItemSupplyPlan();           RecordRef rrSubsidiary = new RecordRef();           rrSubsidiary.setInternalId("1");           rrSubsidiary.setType(RecordType.subsidiary);           isp[0].setSubsidiary(Util.makeRecordRef("1"));                   RecordRef rrLocation = new RecordRef();           rrLocation.setInternalId("1");           rrLocation.setType(RecordType.location);           isp[i].setLocation(rrLocation);                             isp[i].setItem(rrItem[i]);                    ispl.setItemSupplyPlanOrder(ispo);             isp[i].setOrderList(ispl);        }                 _port.add(isp);     }` 
        

Each of the following examples uses the update operation.

## SOAP Request {#bridgehead_N3683436}

          `/*        <update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <record externalId="Strawberry10442165" internalId="6" xsi:type="ns8:ItemSupplyPlan" xmlns:ns8="urn:demandplanning_2017_1.transactions.webservices.netsuite.com">                    <ns8:location internalId="1" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns9:name xsi:type="xsd:string">LOC 1</ns9:name>                    </ns8:location>                    <ns8:item internalId="22" xsi:type="ns10:RecordRef" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                        <ns10:name xsi:type="xsd:string">Item2-ISP</ns10:name>                    </ns8:item>                    <ns8:memo xsi:type="xsd:string">IamupdatingthisISP</ns8:memo>                    <ns8:orderList replaceAll="false" xsi:type="ns8:ItemSupplyPlanOrderList">                        <ns8:itemSupplyPlanOrder xsi:type="ns8:ItemSupplyPlanOrder">                            <ns8:orderLineId xsi:type="xsd:long">0</ns8:orderLineId>                            <ns8:orderDate xsi:type="xsd:dateTime">2012-06-11T07:00:00.000Z</ns8:orderDate>                            <ns8:receiptDate xsi:type="xsd:dateTime">2012-06-11T07:00:00.000Z</ns8:receiptDate>                            <ns8:quantity xsi:type="xsd:double">3.0</ns8:quantity>                            <ns8:orderCreated xsi:type="xsd:boolean">false</ns8:orderCreated>                            <ns8:orderType xsi:type="ns11:ItemSupplyPlanOrderType" xmlns:ns11="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns8:orderType>                        </ns8:itemSupplyPlanOrder>                        <ns8:itemSupplyPlanOrder xsi:type="ns8:ItemSupplyPlanOrder">                            <ns8:orderLineId xsi:type="xsd:long">1</ns8:orderLineId>                            <ns8:orderDate xsi:type="xsd:dateTime">2012-07-04T07:00:00.000Z</ns8:orderDate>                            <ns8:receiptDate xsi:type="xsd:dateTime">2012-07-13T16:54:01.528Z</ns8:receiptDate>                            <ns8:quantity xsi:type="xsd:double">3.0</ns8:quantity>                            <ns8:orderCreated xsi:type="xsd:boolean">false</ns8:orderCreated>                            <ns8:orderType xsi:type="ns12:ItemSupplyPlanOrderType" xmlns:ns12="urn:types.demandplanning_2017_1.transactions.webservices.netsuite.com">_purchaseOrder</ns8:orderType>                        </ns8:itemSupplyPlanOrder>                    </ns8:orderList>                </record>            </update>         */` 
        

## Java {#bridgehead_N3683448}

          `public void  updateItemSupplyPlan() throws Exception     {        this.login(true);                RecordRef rrIsp =  new RecordRef();        rrIsp.setInternalId("6");        rrIsp.setType(RecordType.itemSupplyPlan);                ItemSupplyPlan isp =  (ItemSupplyPlan)sessMgr.getPort().get(rrIsp).getRecord();                isp.setMemo("IamupdatingthisISP");        Calendar c = Calendar.getInstance();        c.set(2012, 6, 14);                isp.getOrderList().getItemSupplyPlanOrder(1).setReceiptDate(c);                Preferences p =  new Preferences();        p.setIgnoreReadOnlyFields(true);                _setPreferences(p);        _Port().update(isp);     }` 
        

Each of the following examples uses the search operation.

## SOAP Request {#bridgehead_N3683465}

          `/*    Request     <soapenv:Body>            <search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">                <searchRecord xsi:type="ns6:ItemSupplyPlanSearch" xmlns:ns6="urn:demandplanning_2017_1.transactions.webservices.netsuite.com">                    <ns6:basic xsi:type="ns7:ItemSupplyPlanSearchBasic" xmlns:ns7="urn:common_2017_1.platform.webservices.netsuite.com">                        <ns7:item operator="anyOf" xsi:type="ns8:SearchMultiSelectField" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com">                            <ns8:searchValue internalId="22" type="inventoryItem" xsi:type="ns8:RecordRef"/>                        </ns7:item>                    </ns6:basic>                </searchRecord>            </search>        </soapenv:Body>        */` 
        

## Java {#bridgehead_N3683477}

          `public void searchItemSupplyPlan() throws Exception     {            this.login(true);        ItemSupplyPlanSearch isp =  new ItemSupplyPlanSearch();       ItemSupplyPlanSearchBasic ispb =  new  ItemSupplyPlanSearchBasic();              RecordRef rrItem =  new RecordRef();       rrItem =  new RecordRef();       rrItem.setInternalId("22");        rrItem.setType(RecordType.inventoryItem);              SearchMultiSelectField smsi =  new SearchMultiSelectField();       smsi.setOperator(SearchMultiSelectFieldOperator.anyOf);       smsi.setSearchValue(new RecordRef[] { rrItem });              ispb.setItem(smsi);        isp.setBasic(ispb);        SearchResult sr = _port.search(isp);            }` 
        

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
