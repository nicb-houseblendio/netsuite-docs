---
id: "section_N3717575"
type: "section"
title: "Inventory Item"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Inventory Item"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3717575.html"
anchors: ["bridgehead_N3717588", "bridgehead_N3717811", "bridgehead_N3717849", "bridgehead_N3717857", "bridgehead_N3717869", "bridgehead_N3717881", "bridgehead_1541691826", "bridgehead_N3717898", "bridgehead_N3717939", "bridgehead_3820196107", "bridgehead_1548422297", "bridgehead_N28687381", "bridgehead_N3717921"]
sha256: "ff56fcccf2d81b64dfc2be86dc717e27a6cadbe9a8a4e5c8ed99b05b3a812600"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161522936052.html).

Inventory item records are used to track information about items for which you maintain a stock. For information about using this record in the UI, see [Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247990.html).

## Supported Operations {#bridgehead_N3717588}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3717811}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [inventory item](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/inventoryitem.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3717849}

## Working with Inventory Items Sublists {#bridgehead_N3717857}

The SOAP Schema Browser includes all sublists associated with the inventory item record. See the following information for usage notes regarding specific Inventory Item sublists. Usage notes are not provided for every sublist type.

## InventoryItemLocations {#bridgehead_N3717869}

To provide a locations list, the Multi-Location Inventory feature must be enabled at Setup > Company > Enable Features. Click the Items & Inventory subtab, and check the Multi-Location Inventory box. Otherwise, single entries for each corresponding field can be entered in the regular record fields.

## ItemVendorList {#bridgehead_N3717881}

The Vendor sublist (ItemVendorList) on inventory items contains a **schedule** field that holds pricing schedule values. Note that when this field is set, it triggers a recalc on add and update operations.

## Merchandise Hierarchy Sublist {#bridgehead_1541691826}

This sublist is available if the Merchandise Hierarchy feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Items & Inventory subtab.

## Getting Bin Details for Items {#bridgehead_N3717898}

If the Bin Management feature is enabled, you can use ItemSearchAdvanced to get bin-related details about inventory items. The following code snippets illustrate a search that returns the quantity available per bin.

## Accessing Inventory Detail Data {#bridgehead_N3717939}

If the Advanced Bin / Numbered Inventory Management feature is enabled, inventory items that have Use Bins set to True include data from a new [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord. This subrecord includes quantity on hand and quantity available values per bin number.

If this feature is enabled, you must use the 2011.2 endpoint or later to access the newly supported subrecord and the most up to date bin fields for inventory items. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Examples {#bridgehead_3820196107}

## Java {#bridgehead_1548422297}

Note:

In this sample the variable 'c' is a shortcut for the client that needs to communicate with NetSuite through SOAP web services

          `public void AddInventoryItem() throws Exception {         RecordRef TaxSchedule = new RecordRef();         TaxSchedule.setInternalId("3");         RecordRef BookDpt = new RecordRef();         BookDpt.setInternalId("1");          InventoryItem NewItem = new InventoryItem();         NewItem.setItemId("New Book Delivery");         NewItem.setTaxSchedule(TaxSchedule);         NewItem.setDisplayName("J.K.R. Book");         NewItem.setDepartment(BookDpt);         c.addRecord(NewItem);     }` 
        

## SOAP Request {#bridgehead_N28687381}

          `<soapenv:Body>            <add xmlns="urn:messages_2018_2.platform.webservices.netsuite.com">                <record xsi:type="ns7:InventoryItem" xmlns:ns7="urn:accounting_2018_2.lists.webservices.netsuite.com">                    <ns7:taxSchedule internalId="3" xsi:type="ns8:RecordRef" xmlns:ns8="urn:core_2018_2.platform.webservices.netsuite.com"/>                    <ns7:itemId xsi:type="xsd:string">Testing Second New Item WS</ns7:itemId>                    <ns7:displayName xsi:type="xsd:string">J.K.R. Book</ns7:displayName>                    <ns7:department internalId="1" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2018_2.platform.webservices.netsuite.com"/>                </record>            </add>        </soapenv:Body>` 
        

## SOAP Response {#bridgehead_N3717921}

          `<soapenv:Body>          <addResponse xmlns="urn:messages_2018_2.platform.webservices.netsuite.com">             <writeResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2018_2.platform.webservices.netsuite.com">                   <platformCore:statusDetail>                      <platformCore:afterSubmitFailed>false</platformCore:afterSubmitFailed>                   </platformCore:statusDetail>                </platformCore:status>                <baseRef internalId="244" type="inventoryItem" xsi:type="platformCore:RecordRef" xmlns:platformCore="urn:core_2018_2.platform.webservices.netsuite.com"/>             </writeResponse>          </addResponse>       </soapenv:Body>` 
        

Note:

As of the 2013.1 endpoint, locationBinQuantityAvailable has a type of SearchColumnStringField. In earlier endpoints, it had a type of SearchColumnDoubleField.

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
