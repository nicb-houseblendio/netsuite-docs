---
id: "section_N3681685"
type: "section"
title: "Item Receipt"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Item Receipt"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3681685.html"
anchors: ["bridgehead_N3681775", "bridgehead_N3682025", "bridgehead_N3682062", "bridgehead_N3682070", "bridgehead_4770786720", "bridgehead_4788044537", "bridgehead_4770788772", "bridgehead_4770788914", "bridgehead_N3682133", "bridgehead_N3682145"]
sha256: "c19900a715c997a92cf45023be520b04153f83a0656204e204b06161dbef9f45"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0817102411.html).

An item receipt transaction records the receipt of returned items from customers. This transaction updates the following information:

-   Items on return authorizations are recorded as received.
    
-   Inventory records are updated for the new stock levels.
    
-   Inventory asset accounts are updated with the values of returned items.
    
-   Status of the return is updated.
    

The item receipt transaction is available when the Advanced Receiving feature is enabled.

For more details about this type of transaction, see [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html) and [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html).

The item receipt record is defined in [tranPurch (purchases)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/purchases.xsd) XSD.

## Supported Operations {#bridgehead_N3681775}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3682025}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [item receipt](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/itemreceipt.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3682062}

## Initializing Item Receipts {#bridgehead_N3682070}

You can initialize an item receipt from a [Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3687718.html), a [Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3688557.html), a [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html), or an [Intercompany Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3675550.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Initializing Item Receipts from Transfer Orders {#bridgehead_4770786720}

You can enter partial fulfillments and receipts for transfer orders, and track item costs throughout the transfer process. For details, see [Fulfilling Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2312176.html). To fulfill partial transfer orders, you must have the Use Item Cost as Transfer Cost preference enabled for that transfer order.

When an item receipt is initialized from a transfer order, the InitializeAuxRefType itemFulfillment parameter is returned in request responses. The returned itemFulfillment parameter specifies the item fulfillment record associated with the transfer order.

For information about how to work with the transfer order record in the UI, see [Transferring Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308202.html). For information about how to work with the record in SOAP web services, see [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html).

The following example shows the initialization of an item receipt using the itemFulfillment parameter from a that was fulfilled twice.

## Java {#bridgehead_4788044537}

          `public void test_item_receipt_from_transfer_order_specify_fulfillment() throws Exception { ItemReceipt ir = (ItemReceipt) c.initialize(new InitializeRef(null, InitializeRefType.transferOrder, "308", null), InitializeType.itemReceipt, new InitializeAuxRef(null, InitializeAuxRefType.itemFulfillment, "309", null))  c.addRecord(ir)  ItemReceipt ir2 = (ItemReceipt) c.initialize(new InitializeRef(null, InitializeRefType.transferOrder, "308", null), InitializeType.itemReceipt, new InitializeAuxRef(null, InitializeAuxRefType.itemFulfillment, "310", null))  c.addRecord(ir2) }` 
        

## SOAP Request {#bridgehead_4770788772}

          `<soapenv:Body>         <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns8:ItemReceipt" xmlns:ns8="urn:purchases_2017_1.transactions.webservices.netsuite.com">                 <ns8:createdDate xsi:type="xsd:dateTime">2016-12-06T22:32:00.000Z</ns8:createdDate>                 <ns8:lastModifiedDate xsi:type="xsd:dateTime">2016-12-06T22:43:00.000Z</ns8:lastModifiedDate>                 <ns8:exchangeRate xsi:type="xsd:double">1.0</ns8:exchangeRate>                 <ns8:currencyName xsi:type="xsd:string">USA</ns8:currencyName>                 <ns8:createdFrom xsi:type="ns9:RecordRef" internalId="308" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns9:name xsi:type="xsd:string"> #1</ns9:name>                 </ns8:createdFrom>                 <ns8:tranDate xsi:type="xsd:dateTime">2016-12-08T08:00:00.000Z</ns8:tranDate>                 <ns8:postingPeriod xsi:type="ns10:RecordRef" internalId="289" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns10:name xsi:type="xsd:string">Dec 2016</ns10:name>                 </ns8:postingPeriod>                 <ns8:tranId xsi:type="xsd:string">5</ns8:tranId>                 <ns8:itemFulfillment xsi:type="ns11:RecordRef" internalId="310" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns11:name xsi:type="xsd:string">Item Fulfillment #7</ns11:name>                 </ns8:itemFulfillment>                 <ns8:currency xsi:type="ns12:RecordRef" internalId="1" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com">                     <ns12:name xsi:type="xsd:string">USA</ns12:name>                 </ns8:currency>                 <ns8:itemList xsi:type="ns8:ItemReceiptItemList" replaceAll="false">                     <ns8:item xsi:type="ns8:ItemReceiptItem">                         <ns8:itemReceive xsi:type="xsd:boolean">true</ns8:itemReceive>                         <ns8:item xsi:type="ns13:RecordRef" internalId="61" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com">                             <ns13:name xsi:type="xsd:string">Telephone Headset</ns13:name>                         </ns8:item>                         <ns8:orderLine xsi:type="xsd:long">6</ns8:orderLine>                         <ns8:line xsi:type="xsd:long">6</ns8:line>                         <ns8:itemName xsi:type="xsd:string">Telephone Headset</ns8:itemName>                         <ns8:location xsi:type="ns14:RecordRef" internalId="2" xmlns:ns14="urn:core_2017_1.platform.webservices.netsuite.com">                             <ns14:name xsi:type="xsd:string">Warehouse - West Coast</ns14:name>                         </ns8:location>                         <ns8:onHand xsi:type="xsd:double">0.0</ns8:onHand>                         <ns8:quantityRemaining xsi:type="xsd:double">48.0</ns8:quantityRemaining>                         <ns8:quantity xsi:type="xsd:double">48.0</ns8:quantity>                     </ns8:item>                 </ns8:itemList>             </record>         </add>     </soapenv:Body>` 
        

## SOAP Response {#bridgehead_4770788914}

          `<soapenv:Body>         <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                 <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <baseRef xsi:type="platformCore:RecordRef" type="itemReceipt" internalId="409" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>         </addResponse>     </soapenv:Body>` 
        

## Key Field for ItemReceiptItemList {#bridgehead_N3682133}

The orderLine field is used for transforms, because it implies a link between the previous transaction and the current one. For example, to add an item receipt from a purchase order, the purchase order lines would be "orderLines", because the receipt has not been saved. After the item receipt is saved, lines should be accessed through the **line** field.

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3682145}

As of the 2011.2 endpoint, code to access serial number, lot number, and bin number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the inventory detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

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
