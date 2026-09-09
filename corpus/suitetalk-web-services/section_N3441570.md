---
id: "section_N3441570"
type: "section"
title: "Updating Sublists in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Sublists in SOAP Web Services > Updating Sublists in SOAP Web Services"
parent: "section_N3439908"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3441570.html"
anchors: ["bridgehead_N3441599", "bridgehead_N3443228", "bridgehead_N3443249", "bridgehead_3705117531", "bridgehead_3705118019"]
sha256: "db74ecb9e5151d0d0b4adf6beb91a419640234d9b54b86176544a216e49d0e74"
---

When working with sublists, the approach for updating the lines in a sublist will vary depending on whether you are working with [Keyed Sublists](#bridgehead_N3441599) or [Non-Keyed Sublists](#bridgehead_3705118019).

## Keyed Sublists {#bridgehead_N3441599}

Keyed sublists have an indexing line element or internal ID that can be used as a key. Keyed sublists allow you to set the **replaceAll** attribute to FALSE to update only the lines you are submitting in your SOAP request. When working with keyed sublists, the value of the replaceAll attribute has the following effects:

-   replaceAll = TRUE: The existing sublist is **replaced** with the sublist submitted in the SOAP web services request. The newly submitted sublist should include all values.
    
    -   Lines that do not match the newly submitted lines are removed.
        
    -   Currently existing lines that match lines in the new sublist submission are updated.
        
    -   Newly submitted lines with no matches are added.
        
    
    The default value for the replaceAll attribute is TRUE.
    
-   replaceAll = FALSE: Lines in the existing sublist are **selectively updated** with lines in the sublist submitted in the SOAP web services request. The newly submitted sublist need only include values to be added and updated.
    
    -   Lines that do not match the newly submitted lines are preserved.
        
    -   Currently existing lines that match lines in the new sublist submission are updated.
        
    -   Newly submitted lines with no matches are added.
        

The following table lists sublists that are categorized as keyed sublists in SOAP web services. Sublists that do not appear in this table are considered [Non-Keyed Sublists](#bridgehead_3705118019). The sublist key listed for each keyed sublist below is used to link the sublist data with the appropriate record.

Important:

PricingMatrixList and demandPlanDetailList are matrix sublists. Updates to matrix sublists may require additional handling related to the replaceAll attribute. See [Matrix Sublists and replaceAll](#bridgehead_N3443249).

| Sublist | Sublist Key | Appears on Record(s) |
| --- | --- | --- |
| accruedTimeList | payrollitem | Employee |
| addressbookList | internalId | Contact, Customer, Employee, Lead, Partner, Project, Prospect, Vendor Note: When you work with the addressbookList on customer records, be sure to use **internalId** as the key. Do not use **label**. |
| applyList | doc | Customer Payment, Credit Memo, Customer Refund, Customer Deposit, Deposit Application, Vendor Credit, Vendor Payment |
| assigneeList | resource | Project Task |
| attendeeList | attendee | Calendar Event |
| binNumberList | binNumber | Assembly Item (BOM Item), Inventory Item, Lot Numbered Assemby Item, Lot Numbered Inventory Item, Serialized Assembly Item, Serialized Inventory Item |
| campaignDirectMailList | internalId | Campaign |
| campaignEmailList | internalId | Campaign |
| campaignEventList | internalId | Campaign |
| 
companyContribution

List



 | payrollitem | Employee |
| component | id | BOM Revision |
| componentList | item | Assembly Unbuild, Assembly Build |
| contactList | company | Customer, Partner, Vendor |
| creditList | doc | Customer Payment, Vendor Payment |
| creditCardsList | internalId | Customer, Job |
| currencyList | currency | Customer (when Multi-Currency Customer enabled) |
| deductionList | payrollitem | Employee |
| depositList | doc | Customer Payment, Customer Refund |
| deptAccessList | dept | Custom Entity Field, CRM Custom Field, Other Custom Field, Item Custom Field, Transaction Body Custom Field, Transaction Column Custom Field, Item Option Custom Field, Custom Record Custom Field, Item Number Custom Field |
| dimensionList | sequence | Fair Value Price |
| directDepositList | internalid | Employee |
| earningList | payrollitem | Employee |
| expCostList | doc | Invoice, Cash Sale |
| expenseList | orderLine or line | Check, Expense Report, Item Receipt, Purchase Order, Purchase Requisition, Vendor Bill, Vendor Credit, Vendor Return Authorization |
| inventoryAssignmentList | internalId |  |
| itemList | orderLine or line | Bin Putaway Worksheet, Bin Transfer, Cash Sale, Check, Estimate, Inventory Transfer, Invoice, Item Fulfillment, Item Receipt, Credit Memo, Return Authorization, Cash Refund, Opportunity, Purchase Order, Purchase Requisition, Sales Order, Vendor Bill, Vendor Credit, Vendor Return Authorization, Work Order Notes:

-   On Item sublists, the value **End of Group** is not returned in SOAP web services. This behavior mimics the behavior of the UI.
-   For cash sale records, the orderLine field establishes the relationship with an existing sales order, if any. You must set a value for orderLine to populate the createdFrom field.
-   To create a credit memo with the createdForm field populated, you must set a value for orderLine. In subsequent update requests, you must use 'line' for line updates.
-   For item receipt records, orderLine is used for transforms, because it implies a link between the previous transaction and the current one. For example, to add an item receipt from a purchase order, the purchase order lines would be "orderLines", because the receipt has not been saved. After the item receipt is saved, lines should be accessed through the "line" field.
-   For opportunity records, line is used.

 |
| itemCostList | doc | Invoice, Cash Sale |
| itemsList | item | Promotion Code, Item Option Custom Field, Item Number Custom Field. |
| lineList | line | Custom Transaction, Journal Entry, Intercompany Journal Entry, Advanced Intercompany Journal Entry, and Statistical Journal Entry |
| locationsList | locationId | Inventory Item, Serialized Inventory Item, Lot Numbered Inventory Item |
| merchandiseHierarchy | hierarchyversion | Inventory Item, Lot Numbered Inventory Item, Serialized Inventory Item Note: This sublist is available if the Merchandise Hierarchy feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Items & Inventory subtab. |
| milestoneList | milestoneId | Billing Schedule Note: This sublist is available only when scheduleType is set to Fixed Bid Milestone. |
| nexusesTaxList | nexus | Tax Type |
| partnersList | partner | Estimate, Cash Sale, Invoice, Sales Order, Opportunity, Credit Memo, Return Authorization, Cash Refund, Customer |
| partnersList | partner | Promotion Code |
| paymentList | The internal ID of the record being referenced in the sublist line. | Deposit |
| periodDemandPlanList | startDate | Item Demand Plan Note: This sublist includes additional handling for replaceAll. See [Matrix Sublists and replaceAll](#bridgehead_N3443249). |
| predecessorList | task | Project Task |
| pricingMatrixList | Varies according to enabled features. See [Pricing Matrix Keys](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707950.html#bridgehead_N3708589). | Item Note: This sublist includes additional handling for replaceAll. See [Matrix Sublists and replaceAll](#bridgehead_N3443249). |
| ratesList | subsidiary | Expense Category Note: Sublist available only to OneWorld accounts. |
| recurrence | recurrenceId | Billing Schedule Note: This sublist is available only when scheduleType is set to Standard and frequency is set to Custom. |
| resourceList | resource | Calendar Event |
| roleAccessList | role | Entity Custom Field, CRM Custom Field, Other Custom Field, Item Custom Field, Transaction Body Custom Field, Transaction Column Custom Field, Item Option Custom Field, Custom Record Custom Field, Item Number Custom Field |
| salesTeam | employee | Customer, Invoice, Cash Sale |
| taxRegistrations | id | Customer, Partner, Vendor Sublist available when the SuiteTax feature is enabled. |
| timeList | doc | Invoice, Cash Sale |

## Example {#bridgehead_N3443228}

The following sample shows how to add an item to an opportunity record and modify an existing item in that record. To do this, set replaceAll to FALSE, add the new item, and modify the existing item by referencing the desired item in the line property. The following shows that the existing line item is modified to change the quantity.

          `<soapenv:Body> <platformMsgs:update xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/"  xmlns:s0="urn:sales_2017_1.transactions.webservices.netsuite.com"  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"  xmlns:xsd="http://www.w3.org/2001/XMLSchema"  xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com"> <platformMsgs:record xsi:type="s0:Opportunity" internalId="1638">    <s0:itemList replaceAll="false">       <s0:item>          <s0:item internalId="380" type="inventoryItem" />          <s0:quantity>1.0</s0:quantity>          <s0:amount>20.0</s0:amount>       </s0:item>       <s0:item>          <s0:line>2</s0:line>          <s0:quantity>10.0</s0:quantity>       </s0:item>    </s0:itemList> </platformMsgs:record> </platformMsgs:update> </soapenv:Body>` 
        

## Matrix Sublists and replaceAll {#bridgehead_N3443249}

Matrix sublists respect the replaceAll attribute for updates, as other [Keyed Sublists](#bridgehead_N3441599) do, but in some cases, updates to matrix sublists require additional handling.

Matrix sublists require additional handling for replaceAll because body-level fields populate values into them. For example, setting the pricing schedule for an item dictates values in the pricing matrix. In the UI, when a pricing schedule is selected, the pricing schedule logic is run first, and values specified in the pricing matrix sublist are taken into account to arrive at what the update should do. However, the UI does not have the notion of replaceAll because the user interacting with the form can delete values they do not want to keep in individual fields.

SOAP web services requests cannot delete individual field values in a sublist. The only way to get rid of old values is to set replaceAll to TRUE and send all values in the update request. Some body fields can override values in a matrix sublist, but a SOAP web services request can then change some or all of these sublist values, depending on the replaceAll setting.

Review the following cases to get an understanding of how the slaving of values from body fields into a matrix sublist interacts with the replaceAll setting on updates:

-   No sublist values from body fields and replaceAll=TRUE
    
    The SOAP web services request does not include any body field values that drive values in the sublist, so the update is handled like those in other keyed sublists where replaceAll is set to TRUE.
    
    The existing sublist is **replaced** with the sublist submitted in the SOAP web services request. The newly submitted sublist should include all values.
    
-   No sublist values from body fields and replaceAll = FALSE
    
    The SOAP web services request does not include any body field values that drive values in the sublist, so the update is handled like those in other keyed sublists where replaceAll is set to FALSE.
    
    Lines in the existing sublist are **selectively updated** with lines in the sublist submitted in the SOAP web services request. The newly submitted sublist need only include values to be added and updated.
    
-   Sublist values from body fields and replaceAll=TRUE
    
    The SOAP web services request sets body field value(s) that drive values in the sublist, so specialized handling is required.
    
    First, all sublist values are removed. Next, sublist values driven by body field values are set. Then, the sublist is updated with all lines specified in the newly submitted sublist. The newly submitted sublist lines thus override the values driven by body fields.
    

Important:

When sublist values from a SOAP web services request override values driven by body fields, errors may occur. If you do not want these overrides, you must set replaceAll to FALSE. For example, if you are setting a quantity pricing schedule, you should set ReplaceAll to FALSE.

-   Sublist values from bodyfields and replaceAll=FALSE
    
    The SOAP web services request sets body field value(s) that drive values in the sublist, so specialized handling is required.
    
    First, sublist values driven by body field values are set. Then, the sublist is updated with any updated or added lines from the newly submitted sublist.
    

Note:

By default, replaceAll is set to TRUE for matrix sublists, like other sublists.

## Currently Supported Matrix Sublists {#bridgehead_3705117531}

The pricingMatrixList on Items and periodDemandPlanList on Item Demand Plans are currently supported matrix sublists. For details about these sublists, see [Pricing Matrix List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707950.html) and [Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3679563.html).

Important:

In endpoints prior to 2012.1, updates to pricingMatrixList ignore the replaceAll attribute. For the 2012.1 and later endpoints, replaceAll is respected for this sublist.

## Non-Keyed Sublists {#bridgehead_3705118019}

Non-keyed sublists have no indexing line element or internal ID that can be used as a key. Each line in a non-keyed sublist is recorded in a _flat_ list.

In the UI, non-keyed sublists and keyed sublists may look similar; however, technically, they are quite different. Because non-keyed sublists contain no referencing keys (or handles), you cannot update a specific line in a non-keyed sublist. Instead, you must interact with the **sublist as a whole.** In non-keyed sublists, the **replaceAll** attribute is ignored and behaves as if it were set to TRUE for all requests. Consequently, an update operation is similar to the add operation with respect to non-keyed sublists.

In the context of SOAP web services, all sublists not listed as [Keyed Sublists](#bridgehead_N3441599) are considered to be non-keyed sublists. The following bullets outline the behaviors of non-keyed sublists.

-   To update a single line in the sublist, retrieve the entire sublist, change a single line as desired, and then resubmit the entire sublist.
    
-   To replace the sublist with a subset of lines, retrieve the entire sublist, and then resubmit the subset of lines. The original sublist is purged and replaced by the new sublist containing the subset of lines.
    
-   To delete the sublist, submit an empty sublist. See [Deleting All Lines on a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443838.html) for more information.
    

### Related Topics

-   [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html)
-   [Sublist Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443715.html)
-   [Deleting All Lines on a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443838.html)
-   [Searching a Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3443977.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
