---
id: "section_N3697954"
type: "section"
title: "Work Order"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Work Order"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html"
anchors: ["bridgehead_N3697986", "bridgehead_N3698256", "bridgehead_N3698293", "bridgehead_N3698353", "bridgehead_3986840034"]
sha256: "8f8bd7e108ee0380f07a7f1642a733c1111753c1a85990cbc018ab6565134bf9"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_47212826771.html).

Work order transactions track the production of assembly items needed for stock or to fill orders. Work orders track the quantities of assemblies that need to be built and the quantities of components, or member items, needed to do so. This type of transaction is available when the Assembly Items and Work Orders features are enabled and is used when the Allow Purchase of Assembly Items accounting preference is not enabled.

Special order work orders track assemblies for a particular sale, and Production work orders track assemblies to increase stock. Both use the same work order form, but Production work orders do not link to a sales transaction. Production work orders are generated when the back ordered quantity of an assembly reaches its assigned build point. After the build point is reached, a work order is added in the Mass Create Work Orders queue. For more details, see [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html).

The work order record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

## Supported Operations {#bridgehead_N3697986}

The following operations can be used with work order records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3698256}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [work order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/workorder.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3698293}

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3698353}

As of the 2011.2 endpoint, code to access serial number, lot number, and bin number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the inventory detail subrecord to access bin and numbered inventory fields, and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Creating a Work Order by Referencing a Sales Order Line {#bridgehead_3986840034}

If appropriate, you can create a work order by referencing a line on a sales order. To use this approach, you supply values for three fields on the work order record:

-   **sourceTransactionId** - Use this field to reference the internal ID of the sales order.
    
-   **sourceTransactionLine** - Use this field to reference the line of the sales order for which you want to create the work order.
    
-   **specialOrder** - Set this boolean field to true to indicate that you want the previous two fields to be referenced as the work order is created.
    

This technique results in the creation of the following links between the sales order and the work order:

-   On the line item of the sales order, a link to the work order is created in the **Create WO** column.
    
-   On the work order, a link to the sales order is created in the **Created From** body field.
    

This approach to creating a work order is similar to the process of creating a work order through initialization. However, note that some body fields on the work order are not automatically populated. For example, you must manually populate the fields for assembly, subsidiary, and quantity.

The following Java example shows how to create a work order using this method:

          `public void testCreateWO() throws Exception {    WorkOrder  wo = new WorkOrder();     wo.setSourceTransactionId("27"); // SalesOrder internalId    wo.setSourceTransactionLine(1L); // Line Number    wo.setSpecialOrder(true);  // To create a work order by referencing a sales order, this must be true.     wo.setAssemblyItem(mrr("10"));    wo.setSubsidiary(mrr("1"));    wo.setQuantity(1.0);     String woId = c.addRecord(wo);     c.getRecord(woId, RecordType.workOrder); }` 
        

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
