---
id: "section_N3684743"
type: "section"
title: "Opportunity"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Opportunity"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684743.html"
anchors: ["bridgehead_N3684764", "bridgehead_N3685019", "bridgehead_N3685056", "bridgehead_N3685085", "bridgehead_N3685107", "procedure_N3685144", "bridgehead_3820133117", "bridgehead_3820133241", "procedure_N3685234", "bridgehead_N3685317", "procedure_N3685364", "bridgehead_N3686931"]
sha256: "9d446deb3393ff02a3e2ce72a1d402c3576d747bbe483f7895bb72e2272ecb69"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0718040350.html).

Opportunities represent negotiations with prospects. You must first enable opportunities in your NetSuite account before you can access this record type. To enable opportunities, go to _Setup > Company > Enable Features_. On the CRM subtab, under Sales, check the Opportunities box.

The opportunity record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3684764}

The following operations can be used with the opportunity record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3685019}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [opportunity](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/opportunity.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3685056}

For details about working with opportunities in NetSuite, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).

## Associating Transactions with Opportunities {#bridgehead_N3685085}

You can associate estimates, cash sales, sales orders, and invoices with opportunities. After a transaction other than an estimate is associated with an opportunity, the opportunity's status is automatically set to **Closed Won**. After an opportunity's status is set to **Closed Won**, it is no longer available to be selected on other cash sale, sales order, or invoice records.

## Projected Total, Range High and Range Low Fields {#bridgehead_N3685107}

When working with opportunity records in the UI, the range low, range high and projected total values must comply with the following rules:

-   The rangeLow value must be lower than or equal to the projectedTotal value. This value represents the Worst Case projected total.
    
-   The rangeHigh value must be greater than or equal to the projectedTotal value. This amount represents the Upside projected total.
    

In the UI, these values are calculated but can be overridden by the user. The calculated values are determined by relationships between the summation of amounts of entries in the itemList, projectedTotal values, and range low / range high values. When any of the values are overridden by the user, client side validation ensures that the fields are set correctly according to the above rules and automatically recalculates where appropriate.

To maintain proper rangeHigh, rangeLow and projectedTotal relationships when using SOAP web services, the behavior is as follows:

## If Advanced Forecasting is Off {#procedure_N3685144}

## On Add {#bridgehead_3820133117}

-   projectedTotal is required unless there is an item in the item list.
    
-   If projectedTotal is provided and there are items, then projectedTotal is calculated (with the sum of the item amounts).
    
-   If projectedTotal is provided then it is set unless it is equal to the sum of all items, where in that case it is calculated.
    

## On update {#bridgehead_3820133241}

-   If projectedTotal is not provided and there are no items in the update, then projectedTotal is not changed.
    
-   If projectedTotal is not provided and there are items in the update request, then projectedTotal is set to the sum of all items.
    
-   If projectedTotal is not provided and there are items in the original but no items in the update request, then projectedTotal is not changed except where projectedTotal is equal to the sum of all item amounts. In that case it is calculated.
    
-   If projectedTotal is provided and there are items in the original, then projectedTotal is set.
    
-   If projectedTotal is provided are there are items in the update request, then projectedTotal is set except where projectedTotal is equal to the sum of all items in the update request. In the case it is calculated.
    

## If Advanced Forecasting is On {#procedure_N3685234}

**On Add**

-   If no item list is sent in the request and projectedTotal is not provided an error will be thrown.
    
-   If no item list is sent and one or both of rangeLow or rangeHigh are missing then both are set to projectedTotal
    
-   If a value is NOT provided for projectedTotal, rangeLow or rangeHigh fields, then each field is calculated.
    
-   If a value is submitted for any one field then that field is NOT calculated except when a projectedTotal value is equal to the sum of the amounts for entries in the itemList at any point during item summation. In this case the projectedTotal value is calculated (set to the sum of all item amounts) even though a value was submitted.
    

**On Update**

-   If any of the three fields has the same value as previously set, whether calculated or not, all three fields are calculated.
    
-   If all three fields have different values they are not calculated except when a projectedTotal value is equal to the sum of the amounts for entries in the itemList at any point during item summation. In this case the projectedTotal value is calculated (set to the sum of all item amounts) even though a value was submitted.
    
-   If any of the three fields is empty, then all three fields are populated with calculated values except when there is no change to the itemList.
    

## Working with Opportunity Sublists {#bridgehead_N3685317}

The SOAP Schema Browser includes all sublists associated with the opportunity record. See the following information for usage notes regarding specific Opportunity sublists. Usage notes are not provided for every sublist type.

-   [OpportunityItemList](#procedure_N3685364)
    
-   [OpportunitySalesTeam](#bridgehead_N3686931)
    

## OpportunityItemList {#procedure_N3685364}

In an opportunity, a list of items can be added, modified or deleted in the items sublist. However, each item listed in the item sublist is not a keyed entry - the list is an array of items. Therefore, to modify the contents of the items sublist for a particular opportunity record, follow these guidelines:

-   To update the list of items, resubmit the **entire** list (array) of items associated with the opportunity record.
    
-   To delete a subset of items on the list, submit a partial list of what was retrieved with the get operation.
    
-   To delete the entire list, submit an empty list.
    

Important:

If you are using a customForm that has location, department and class customized at the item level, you can NOT set these fields at the body level.

## OpportunitySalesTeam {#bridgehead_N3686931}

This list is only available when the Team Selling feature is enabled.

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
