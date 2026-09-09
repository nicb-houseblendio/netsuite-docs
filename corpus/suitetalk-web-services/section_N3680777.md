---
id: "section_N3680777"
type: "section"
title: "Item Fulfillment"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Item Fulfillment"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3680777.html"
anchors: ["bridgehead_N3680839", "bridgehead_N3681108", "bridgehead_N3681145", "bridgehead_N3681153", "bridgehead_N3681211", "procedure_N3681228", "bridgehead_N3681351", "bridgehead_N3681402", "bridgehead_3820129206", "bridgehead_3820129467", "bridgehead_3820129623", "bridgehead_3820130095", "bridgehead_3820130280", "bridgehead_3820130404"]
sha256: "41e4221c41c16e72c628d8f2f10b45eb3f298750931af45d590695c3f23d2657"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Item Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161425629582.html).

An item fulfillment transaction records the shipment of some or all items on an order to the customer. The processes for item fulfillment transactions depend on whether the Advanced Shipping feature is enabled.

-   If Advanced Shipping is not enabled, the fulfillment and invoicing processes are combined. When an item fulfillment is created, a related invoice is created at the same time.
    
-   If Advanced Shipping is enabled, fulfillment and invoicing are two independent processes, and shipments can be recorded separately from billing.
    

Note:

Whether Advanced Shipping is enabled or not, order fulfillments should always be entered against sales orders to track the status of items and orders.

For more details about this type of transaction, see [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html).

The item fulfillment record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3680839}

The following operations can be used to manipulate the item fulfillment record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3681108}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [item fulfillment](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/itemfulfillment.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3681145}

## Initializing Item Fulfillments {#bridgehead_N3681153}

You can initialize an item fulfillment from a [Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3690924.html), a [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html), an [Intercompany Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3675550.html), or a [Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3696445.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Item Fulfillment Workflow {#bridgehead_N3681211}

When submitting an item fulfillment record, NetSuite can initialize this record on the server with data from the related transaction (such as a sales order) referenced in the **createdFrom** field. Then the item fulfillment record is updated with the itemList provided in your request and that data is validated against the initialized data from the referenced transaction.

## Partial Fulfillments {#procedure_N3681228}

The 2009.2 and earlier endpoints allow you to specify that only some of the line items in a referenced transaction should be fulfilled. The 2010.1 and later endpoints do not support partial fulfillments of line items from a transaction referenced in the createdFrom field. This behavior is consistent with item fulfillments in the UI and in SuiteScript.

Instead of using the createdFrom field, you can use the initialize operation to create an item fulfillment in SOAP web services. You can then get the item fulfillment record and specify which lines should be fulfilled before submitting the record.

Important:

Validation for Fed Ex or UPS related fields occurs after a record is routed to FedEx or UPS respectively and NOT by the NetSuite application as in the UI. Therefore, it is the responsibility of the client application developer to ensure that the correct fields are populated with the required information for shipping.

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3681351}

As of the 2011.2 endpoint, code to access serial number, lot number, and bin number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the inventory detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Sample Code {#bridgehead_N3681402}

The following code illustrates adding a sales order record with a single item and then fulfilling that order. In this case, the account is set up for shipping with FedEx and FedEx is set as the method of shipping on the sales order record.

First, a sales order is created, set to the pendingFulfillment status, and populated with an itemList.

## Create Sales Order Java {#bridgehead_3820129206}

          `sessMgr.login(); SalesOrder salesOrder = new SalesOrder(); salesOrder.setEntity(Util.makeRecordRef("87", RecordType.customer)); salesOrder.setOrderStatus(SalesOrderOrderStatus._pendingFulfillment); SalesOrderItem soi = new SalesOrderItem(); soi.setItem (Util.makeRecordRef("15", RecordType.inventoryItem)); soi.setQuantity(new Double (1)); soi.setAmount(new Double (14)); SalesOrderItemList soil = new SalesOrderItemList(new SalesOrderItem[]{soi}, true); salesOrder.setItemList(soil); salesOrder = sessMgr.getNetsuitePort().add(salesOrder);` 
        

## Create Sales Order SOAP Request {#bridgehead_3820129467}

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns1:SalesOrder" xmlns:ns1="urn:sales_2017_1.transactions.webservices.netsuite.com"> <ns1:entity internalId="87 customer" xsi:type="ns2:RecordRef" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/> <ns1:orderStatus xsi:type="ns3:SalesOrderOrderStatus" xmlns:ns3="urn:types.sales_2017_1.transactions.webservices.netsuite.com">_pendingFulfillment</ns1:orderStatus> <ns1:itemList replaceAll="true" xsi:type="ns1:SalesOrderItemList"> <ns1:item xsi:type="ns1:SalesOrderItem"> <ns1:item internalId="15 inventoryItem" xsi:type="ns4:RecordRef" xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com"/> <ns1:quantity xsi:type="xsd:double">1.0</ns1:quantity> <ns1:amount xsi:type="xsd:double">14.0</ns1:amount> </ns1:item> </ns1:itemList> </record> </add> </soapenv:Body>` 
        

Using a Get operation on the sales order created above, the itemList information can be determined.

## Get Sales Order SOAP Request {#bridgehead_3820129623}

          `<soapenv:Body> <get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <baseRef internalId="1505 salesOrder" xsi:type="ns1:RecordRef" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/> </get> </soapenv:Body>` 
        

## Get Sales Order SOAP Response {#bridgehead_3820130095}

          `<soapenv:Body> <getResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <readResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <ns1:status isSuccess="true" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/> <record internalId="1505" xsi:type="ns2:SalesOrder" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:ns2="urn:sales_2017_1.transactions.webservices.netsuite.com"> <ns2:entity internalId="87"> <ns3:name xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">Abe Simpson</ns3:name> </ns2:entity> <ns2:tranDate>2006-08-22T00:00:00.000-07:00</ns2:tranDate> <ns2:tranId>SORD10069</ns2:tranId> <ns2:orderStatus>_pendingFulfillment</ns2:orderStatus> <ns2:salesRep internalId="43"> <ns4:name xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">Jon Baker</ns4:name> </ns2:salesRep> <ns2:leadSource internalId="-2"> <ns5:name xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com">Ad</ns5:name> </ns2:leadSource> <ns2:excludeCommission>false</ns2:excludeCommission> <ns2:isTaxable>false</ns2:isTaxable> <ns2:toBePrinted>false</ns2:toBePrinted> <ns2:toBeEmailed>false</ns2:toBeEmailed> <ns2:email>asimpson@boo.com</ns2:email> <ns2:toBeFaxed>false</ns2:toBeFaxed> <ns2:billAddress>Abe Simpson<br>34 Elm St<br>Great Falls MT</ns2:billAddress> <ns2:shipAddress>Abe Simpson<br>34 Elm St<br>Great Falls MT</ns2:shipAddress> <ns2:shipDate>2006-08-22T00:00:00.000-07:00</ns2:shipDate> <ns2:subTotal>14.0</ns2:subTotal> <ns2:total>14.0</ns2:total> <ns2:balance>0.0</ns2:balance> <ns2:lastModifiedDate>2006-08-22T15:49:00.000-07:00</ns2:lastModifiedDate> <ns2:status>Pending Fulfillment</ns2:status> <ns2:itemList> <ns2:item> <ns2:item internalId="15"> <ns6:name xmlns:ns6="urn:core_2017_1.platform.webservices.netsuite.com">Tongue Depressor</ns6:name> </ns2:item> <ns2:quantity>1.0</ns2:quantity> <ns2:price internalId="1"> <ns7:name xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com">Base Price</ns7:name> </ns2:price> <ns2:rate>14.00</ns2:rate> <ns2:amount>14.0</ns2:amount> <ns2:commitInventory>_availableQty</ns2:commitInventory> <ns2:isTaxable>true</ns2:isTaxable> <ns2:isClosed>false</ns2:isClosed> <ns2:line>1</ns2:line> <ns2:quantityBackOrdered>0.0</ns2:quantityBackOrdered> <ns2:quantityBilled>0.0</ns2:quantityBilled> <ns2:quantityCommitted>1.0</ns2:quantityCommitted> <ns2:quantityFulfilled>0.0</ns2:quantityFulfilled> </ns2:item> </ns2:itemList> </record> </readResponse> </getResponse> </soapenv:Body>` 
        

## Item Fulfillment Java {#bridgehead_3820130280}

Next the sales order created above is referenced by setting the createdFrom field to the internalId of the sales order. The specific items to be fulfilled are referenced by setting the Line field to the desired item line from the sales order.

          `ItemFulfillment itemFulfillment = new ItemFulfillment(); itemFulfillment.setCreatedFrom(Util.makeRecordRef(salesOrder.getInternalId(), RecordType.salesOrder)); ItemFulfillmentItemList ifil = new ItemFulfillmentItemList(); ItemFulfillmentItem ifi = new ItemFulfillmentItem(); ifi.setOrderLine(salesOrder.getItemList().getItem(0).getLine()); ifil.setItem(new ItemFulfillmentItem[]{ifi}); itemFulfillment.setItemList(ifil); itemFulfillment = sessMgr.getNetsuitePort().add(itemFulfillment);` 
        

## Item Fulfillment SOAP Request {#bridgehead_3820130404}

          `<soapenv:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="ns1:ItemFulfillment" xmlns:ns1="urn:sales_2017_1.transactions.webservices.netsuite.com"> <ns1:createdFrom internalId="1505 salesOrder" xsi:type="ns2:RecordRef" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/> <ns1:itemList replaceAll="false" xsi:type="ns1:ItemFulfillmentItemList"> <ns1:item xsi:type="ns1:ItemFulfillmentItem"> <ns1:orderLine xsi:type="xsd:long">1</ns1:orderLine> </ns1:item> </ns1:itemList> </record> </add> </soapenv:Body>` 
        

Important:

Item fulfillment creation is affected by the preference set at _Setup > Accounting > Accounting Preferences > Order Management tab > Fulfillment Based on Commitment_. The best practice for creating an item fulfillment in SOAP web services is to use the initialize operation, as it returns the item fulfillment with all the defaults set and users will not have to specify the item quantities themselves. Following this practice prevents users from generating a partially fulfilled order without knowing it. (See [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) in the NetSuite Help Center for details on this operation.)

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
