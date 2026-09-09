---
id: "section_N3744760"
type: "section"
title: "Inventory Detail"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Subrecords > Inventory Detail"
parent: "chapter_4599346578"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html"
anchors: ["bridgehead_N3745037", "bridgehead_N3745049", "bridgehead_N3745090", "bridgehead_N3745098", "bridgehead_N3745110", "bridgehead_N3745154", "bridgehead_N3745166", "bridgehead_N28832641", "bridgehead_N28832521", "bridgehead_N28832581", "bridgehead_N3745214", "bridgehead_N28832831", "bridgehead_N3745244"]
sha256: "5b0155292365b75c0bc905e9e8ded805473cd88520e25a9f2a5bc0687f7acee3"
---

The inventory detail subrecord is available when the Advanced Bin / Numbered Inventory Management feature is enabled.

-   This type of record stores values relating to bin numbers and/or serial/lot numbers for items, including line items on transactions.
    
-   This data includes the quantity on hand and quantity available per bin number, or per serial/lot number, or when both are in use, per bin number/serial lot number combination.
    
-   In the UI, the inventory detail subrecord displays as a popup when you click the Inventory Detail body field or sublist field.
    
-   For more details, see [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).
    

The inventory detail subrecord is defined in the [Common](https://webservices.netsuite.com/xsd/platform/v2025_2_0/common.xsd) XSD.

Important:

The SOAP web services code used to access bin number and serial/lot number data for items varies according to whether the Advanced Bin / Numbered Inventory Management feature is enabled. If this feature is not enabled, this data is available directly from the item, and you receive an error if you attempt to access it through the inventory detail record. If this feature is enabled, this data must be accessed through the inventory detail record. See [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Operations Must Be in Parent Context {#bridgehead_N3745037}

Any add, get, update, delete, or search operation on an inventory detail subrecord must be performed within the context of an operation on its parent record. For example, if you want to update inventory detail data for an item on a purchase order transaction, you must update the purchase order record itself; you cannot do an independent update of the inventory detail object. And this same limitation applies to all operations on an inventory detail subrecord.

## Field Definitions {#bridgehead_N3745049}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this subrecord. For details, see the SOAP Schema Browser's [inventory detail reference page](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/inventorydetail.html)

Note:

For information on using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3745090}

See the following sections for more details about this subrecord:

-   [InventoryAssignmentList](#bridgehead_N3745098)
    
-   [Inventory Detail Preferences](#bridgehead_N3745110)
    

## InventoryAssignmentList {#bridgehead_N3745098}

In the schema, InventoryDetail includes a sublist called InventoryAssignmentList, with sublist fields that include the following: internalId, issueInventoryNumber, receiptnventoryNumber, binNumber, toBinNumber, quantity, expirationDate, and quantityAvailable.

## Inventory Detail Preferences {#bridgehead_N3745110}

The following preferences apply to inventory detail (and generally to all subrecords):

-   For an add operation, you can put the subrecord in the nullFieldList to null out the subrecord.
    
-   If a subrecord is not in the nullFieldList, its replaceAll attribute determines whether the subrecord is added or updated during an add operation on its parent record. If this attribute is set to true, the subrecord is deleted and a new one is added. If this preference is set to false, an update of the subrecord is attempted. For inventory detail, the default for the replaceAll attribute is false.
    

## Sample Code {#bridgehead_N3745154}

The following sections show a few examples of how to interact with the inventory details subrecord.

## Setting Inventory Details on an Adjustment {#bridgehead_N3745166}

The following examples illustrate setting inventory detail values on an inventory adjustment transaction.

## Java {#bridgehead_N28832641}

          `InventoryAdjustment ia = new InventoryAdjustment(); ia.setSubsidiary(new RecordRef(null,"1",null,null)); ia.setAccount(new RecordRef(null,"1",null,null));   InventoryAdjustmentInventory item = new InventoryAdjustmentInventory(); item.setItem(new RecordRef(null, i.getInternalId(), null, null)); item.setLocation(new RecordRef(null,"1",null,null)); item.setAdjustQtyBy(new Double(2));   InventoryAssignment assign = new InventoryAssignment(); assign.setReceiptInventoryNumber("Grape19816143,Melon12289447"); assign.setQuantity(new Double(2));   InventoryDetail id = new InventoryDetail(); id.setInventoryAssignmentList(new InventoryAssignmentList(new InventoryAssignment[] {assign},true)); item.setInventoryDetail(id);   ia.setInventoryList(new InventoryAdjustmentInventoryList(new InventoryAdjustmentInventory[] {item},true));   sessMgr.getPort().add(ia);` 
        

## SOAP Request {#bridgehead_N28832521}

          `<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">        <soapenv:Body>          <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record externalId="Strawberry10424664" xsi:type="ns6:InventoryAdjustment" xmlns:ns6="urn:inventory_2017_1.transactions.webservices.netsuite.com">                <ns6:subsidiary internalId="1" xsi:type="ns7:RecordRef" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:account internalId="1" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                <ns6:inventoryList replaceAll="true" xsi:type="ns6:InventoryAdjustmentInventoryList">                    <ns6:inventory xsi:type="ns6:InventoryAdjustmentInventory">                        <ns6:item internalId="169" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns6:inventoryDetail xsi:type="ns10:InventoryDetail" xmlns:ns10="urn:common_2017_1.platform.webservices.netsuite.com">                          <ns10:inventoryAssignmentList replaceAll="true" xsi:type="ns10:InventoryAssignmentList">                                    <ns10:inventoryAssignment xsi:type="ns10:InventoryAssignment">                               <ns10:receiptInventoryNumber xsi:type="xsd:string">Grape19816143,Melon12289447</ns10:receiptInventoryNumber>                               <ns10:quantity xsi:type="xsd:double">2.0</ns10:quantity>                            </ns10:inventoryAssignment>                          </ns10:inventoryAssignmentList>                      </ns6:inventoryDetail>                      <ns6:location internalId="1" xsi:type="ns11:RecordRef" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                       <ns6:adjustQtyBy xsi:type="xsd:double">2.0</ns6:adjustQtyBy>                   </ns6:inventory>                 </ns6:inventoryList>             </record>          </add>       </soapenv:Body>    </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N28832581}

          `<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">       <soapenv:Header>          <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1247336_092920111272224852700968262_b9abc599312e</platformMsgs:nsId>          </platformMsgs:documentInfo>       </soapenv:Header>       <soapenv:Body>          <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <baseRef internalId="76" externalId="Strawberry10424664" type="inventoryAdjustment" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>          </addResponse>       </soapenv:Body>    </soapenv:Envelope>` 
        

## Searching by Inventory or Bin Number {#bridgehead_N3745214}

The following examples illustrate how to search using inventory number or bin number.

With the first approach shown below, you search using the internal ID of the inventory number. (An inventory number is a serial number or a lot number.) In response, the system looks for item records that reference this number. For each occurrence found, the system returns the data available in the Inventory Detail pop-up. Note that these details may be associated with a variety of other records, such as sales orders, inventory adjustments, and so on. This data includes the serial/lot number, the quantity and, if applicable, the bin number.

## SOAP Request for Search by Inventory Number {#bridgehead_N28832831}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <searchRecord xsi:type="ns7:ItemSearchAdvanced" xmlns:ns7="urn:accounting_2017_1.lists.webservices.netsuite.com">                <ns7:criteria xsi:type="ns7:ItemSearch">                   <ns7:inventoryDetailJoin xsi:type="ns8:InventoryDetailSearchBasic" xmlns:ns8="urn:common_2017_1.platform.webservices.netsuite.com">                      <ns8:inventoryNumber operator="anyOf" xsi:type="ns9:SearchMultiSelectField" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                         <ns9:searchValue internalId="143" type="inventoryNumber" xsi:type="ns9:RecordRef"/>                      </ns8:inventoryNumber>                   </ns7:inventoryDetailJoin>                </ns7:criteria>                <ns7:columns xsi:type="ns7:ItemSearchRow">                   <ns7:inventoryDetailJoin xsi:type="ns10:InventoryDetailSearchRowBasic" xmlns:ns10="urn:common_2017_1.platform.webservices.netsuite.com">                      <ns10:binNumber xsi:type="ns11:SearchColumnSelectField" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:internalId xsi:type="ns12:SearchColumnSelectField" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:inventoryNumber xsi:type="ns13:SearchColumnSelectField" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:quantity xsi:type="ns14:SearchColumnDoubleField" xmlns:ns14="urn:core_2017_1.platform.webservices.netsuite.com"/>                   </ns7:inventoryDetailJoin>                </ns7:columns>             </searchRecord>          </search>` 
        

The following example is similar to the preceding one. However, in this example, you search using the internal ID of the bin number. Similar to the previous example, this search looks for item records, this time looking for those whose inventory details reference the bin number identified in your search. Again, these details may be associated with a variety of records. The data returned includes the serial/lot number, the quantity and the bin number.

## SOAP Request for Search by Bin Number {#bridgehead_N3745244}

          `<search xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <searchRecord xsi:type="ns7:ItemSearchAdvanced" xmlns:ns7="urn:accounting_2017_1.lists.webservices.netsuite.com">                <ns7:criteria xsi:type="ns7:ItemSearch">                   <ns7:inventoryDetailJoin xsi:type="ns8:InventoryDetailSearchBasic" xmlns:ns8="urn:common_2017_1.platform.webservices.netsuite.com">                      <ns8:binNumber operator="anyOf" xsi:type="ns9:SearchMultiSelectField" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                         <ns9:searchValue internalId="1" type="bin" xsi:type="ns9:RecordRef"/>                      </ns8:binNumber>                    </ns7:inventoryDetailJoin>                </ns7:criteria>                <ns7:columns xsi:type="ns7:ItemSearchRow">                   <ns7:inventoryDetailJoin xsi:type="ns10:InventoryDetailSearchRowBasic" xmlns:ns10="urn:common_2017_1.platform.webservices.netsuite.com">                      <ns10:binNumber xsi:type="ns11:SearchColumnSelectField" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:internalId xsi:type="ns12:SearchColumnSelectField" xmlns:ns12="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:inventoryNumber xsi:type="ns13:SearchColumnSelectField" xmlns:ns13="urn:core_2017_1.platform.webservices.netsuite.com"/>                      <ns10:quantity xsi:type="ns14:SearchColumnDoubleField" xmlns:ns14="urn:core_2017_1.platform.webservices.netsuite.com"/>                   </ns7:inventoryDetailJoin>                </ns7:columns>             </searchRecord>          </search>` 
        

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
