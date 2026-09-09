---
id: "section_N3212114"
type: "section"
title: "Demand Plan Detail Sublist"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Demand Plan Detail Sublist"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3212114.html"
anchors: ["bridgehead_N3212283", "bridgehead_N3212358", "bridgehead_N3212374", "bridgehead_N3212464", "bridgehead_N3212480", "bridgehead_N3212589", "bridgehead_N3215271"]
sha256: "9098c6ead0a1ca77d31b6d611b3f8a9fe52703e1232e88c85739c3efd7582969"
---

The internal ID for this sublist is **demandplandetail**.

The Demand Plan Detail sublist appears on the [Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3195081.html) record type.

The Demand Plan Detail sublist is a matrix that is similar to the Pricing sublist. This matrix stores projected quantities demanded by date. Each row in the matrix represents a specific month, week, or day, and each column in the matrix represents an expected quantity demand.

For help working with this record in the UI, see [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html).

Functionally, this sublist shares many of the characteristics of List Sublists. However, scripting with the Demand Plan Detail sublist is not like scripting with most other sublists in NetSuite. You must use [Matrix APIs for the Demand Plan Detail Sublist](#bridgehead_N3215271) to access quantity values on a per-row, per-column basis, similar to the way that item pricing values are accessed. These APIs are a subset of the [N/currentRecord Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html) and [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html) APIs more commonly used for scripting with other sublists.

The format of the Demand Plan Detail sublist depends on the values set in body fields for the start date of the plan, the end date of the plan, and the time period to be used (monthly, weekly, or daily). Because of this dependence, you should work with the Item Demand Plan record and the Demand Plan Detail sublist in dynamic mode. See [SuiteScript 2.x Standard and Dynamic Modes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1524156901.html)

Be aware of the following requirements:

-   To script with the Item Demand Plan record and the Demand Plan Detail sublist for inventory items, the Demand Planning feature must be enabled. For assembly/BOM items, the Work Orders feature also must be enabled.
    
-   You must Demand plans are supported only for item(s) that have the **supplyreplenishmentmethod** field set to Time Phased. To change this setting, go to the item record and set the Replenishment Method to Time Phased.
    
-   Required body field values must be defined before matrix field values can be edited. In dynamic mode, current values may be retrieved. Start date and end date body fields default to the first day and last day of the current year.
    

For more details and code samples for each type of demand plan, see the following help topics:

-   [Monthly Demand Plan](#bridgehead_N3212283)
    
-   [Weekly Demand Plan](#bridgehead_N3212374)
    
-   [Daily Demand Plan](#bridgehead_N3212480)
    

## Monthly Demand Plan {#bridgehead_N3212283}

A monthly demand plan includes a row for each month within the body field start date and end date, and one quantity column for each month.

![Monthly Demand Plan section of the Demand Plan Detail Sublist page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/demandplanmonthly.png)

-   The sublist startdate and enddate fields are system-calculated and read-only.
    
    -   The startdate is the date of the first day of the month represented by each row.
        
    -   The enddate is the date of the last day of the month represented by each row.
        
    -   The month for row 1 is the month set in the body field start date, the month for row 2 is the next month, and so on, until the month set in the body field end date is reached.
        
-   The values for the quantity field can be set in SuiteScript. For monthly demand plans, the column parameter for this field is always 1.
    

## Monthly Demand Plan Code Sample {#bridgehead_N3212358}

The following sample sets quantities for the month of January 2023:

Note:

Some of the values in these samples are placeholders. Before using these samples, replace all hard-coded values, such as IDs and file paths, with valid values from your NetSuite account. If you run a script with an invalid value, the system may throw an error.

          `/**  * @NApiVersion 2.1  */   require(['N/record', 'N/log'], (record, log) => {   const demandplan = record.create({     type: record.Type.ITEM_DEMAND_PLAN,     isDynamic: true   })   demandplan.setValue({     fieldId: 'demandplancalendartype',     value: 'MONTHLY'   })   demandplan.setValue({     fieldId: 'subsidiary',     value: 1   })   demandplan.setValue({     fieldId: 'location',     value: 1   })   demandplan.setValue({     fieldId: 'item',     value: 253   })   const id = demandplan.save({     enableSourcing: true   })      const loadDemandPlan = record.load({     type: record.Type.ITEM_DEMAND_PLAN,     id: id,     isDynamic: true    })   loadDemandPlan.setValue({     fieldId: 'startdate',     value: '1/1/2023'   })   loadDemandPlan.setValue({     fieldId: 'enddate',     value: '12/31/2023'   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '0'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 100   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '1'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 200   })   loadDemandPlan.commitLine({     sublistId: 'demandplandetail'   })   loadDemandPlan.save() })` 
        

## Weekly Demand Plan {#bridgehead_N3212374}

A weekly demand plan includes a row for each week contained in the time period set by the body field start date and end date, and one quantity column for each week.

![Weekly Demand Plan section of the Demand Plan Detail Sublist page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/demandplanweekly.png)

-   The sublist startdate and enddate fields are system-calculated and read-only.
    
    -   The startdate is the date of the first day of the week represented by each row.
        
    -   The enddate is the date of the last day of the week represented by each row.
        
        Note:
        
        The first day of the week by default is Sunday, but may vary according to the company preference set for First Day of the Week at Setup > Company > General Preferences.
        
    -   The week for row 1 is the week of the date set in the body field start date. Note that unless the body field start date happens to be the first day of the week, the startdate for this first row may precede the body field start date.
        
    -   The week for the final sublist row is the week of the date set in the body field end date. Note that unless the body field end date happens to be the last day of the week, the enddate for this last row may be after the body field enddate.
        
-   The values for the quantity field can be set in SuiteScript. For weekly demand plans, the column parameter for this field is always 1.
    

## Weekly Demand Plan Code Sample {#bridgehead_N3212464}

The following sample sets quantities for the first two weeks of the year:

Note:

Some of the values in these samples are placeholders. Before using these samples, replace all hard-coded values, such as IDs and file paths, with valid values from your NetSuite account. If you run a script with an invalid value, the system may throw an error.

          `/**  * @NApiVersion 2.1  */   require(['N/record', 'N/log'], (record, log) => {   const demandplan = record.create({     type: record.Type.ITEM_DEMAND_PLAN,     isDynamic: true   })   demandplan.setValue({     fieldId: 'demandplancalendartype',     value: 'WEEKLY'   })   demandplan.setValue({     fieldId: 'subsidiary',     value: 1   })   demandplan.setValue({     fieldId: 'location',     value: 1   })   demandplan.setValue({     fieldId: 'item',     value: 252   })   const id = demandplan.save({     enableSourcing: true   })        const loadDemandPlan = record.load({     type: record.Type.ITEM_DEMAND_PLAN,     id: id,     isDynamic: true    })   loadDemandPlan.setValue({     fieldId: 'startdate',     value: '1/1/2023'   })   loadDemandPlan.setValue({     fieldId: 'enddate',     value: '12/31/2023'   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '0'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 100   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '1'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 200   })   loadDemandPlan.commitLine({     sublistId: 'demandplandetail'   })   loadDemandPlan.save() })` 
        

## Daily Demand Plan {#bridgehead_N3212480}

A daily demand plan includes a row for each week contained in the time period set by the body field start date and end date, and seven quantity columns for each week, one for each day of the week.

![Daily Demand Plan section of the Demand Plan Detail Sublist page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptRecordsGuide/demandplandaily.png)

-   The sublist startdate and enddate fields are system-calculated and read-only.
    
    -   The startdate is the date of the first day of the week represented by each row.
        
    -   The enddate is the date of the last day of the week represented by each row.
        
        Note:
        
        The first day of the week by default is Sunday, but may vary according to the company preference set for First Day of the Week at Setup > Company > General Preferences.
        
    -   The week for row 1 is the week of the date set in the body field start date. Note that unless the body field start date happens to be the first day of the week, the startdate for this first row may precede the body field start date.
        
    -   The week for the final sublist row is the week of the date set in the body field end date. Note that unless the body field end date happens to be the last day of the week, the enddate for this last row may be after the body field enddate.
        
-   The values for the quantity fields can be set in SuiteScript.
    
    -   The column parameter for a quantity field is 1,2,3,4,5,6, or 7, depending on the day of the week.
        
    -   In the screenshot above, the week starts with Sunday, which is the default first day of the week, and in this case, maps to a column parameter of 1. However, 1 does not always map to Sunday; it maps to the first day of the week as set in the company preferences.
        

## Daily Demand Plan Code Sample {#bridgehead_N3212589}

Note:

Some of the values in these samples are placeholders. Before using these samples, replace all hard-coded values, such as IDs and file paths, with valid values from your NetSuite account. If you run a script with an invalid value, the system may throw an error.

          `/**  * @NApiVersion 2.1  */   require(['N/record', 'N/log'], (record, log) => {   const demandplan = record.create({     type: record.Type.ITEM_DEMAND_PLAN,     isDynamic: true   })   demandplan.setValue({     fieldId: 'demandplancalendartype',     value: 'DAILY'   })   demandplan.setValue({     fieldId: 'subsidiary',     value: 1   })   demandplan.setValue({     fieldId: 'location',     value: 1   })   demandplan.setValue({     fieldId: 'item',     value: 254   })   const id = demandplan.save({     enableSourcing: true   })        const loadDemandPlan = record.load({     type: record.Type.ITEM_DEMAND_PLAN,     id: id,     isDynamic: true    })   loadDemandPlan.setValue({     fieldId: 'startdate',     value: '1/1/2023'   })   loadDemandPlan.setValue({     fieldId: 'enddate',     value: '12/31/2023'   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '0'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 100   })   loadDemandPlan.selectLine({     sublistId: 'demandplandetail',     line: '1'   })   loadDemandPlan.setCurrentSublistValue({     sublistId: 'demandplandetail',     fieldId: 'quantity_1_',     value: 200   })   loadDemandPlan.commitLine({     sublistId: 'demandplandetail'   })   loadDemandPlan.save() })` 
        

## Matrix APIs for the Demand Plan Detail Sublist {#bridgehead_N3215271}

Use the following matrix APIs with the Demand Plan Detail sublist:

-   [Record.getCurrentMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4599582937.html)
    
-   [CurrentRecord.getCurrentMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637585905.html)
    
-   [Record.setCurrentMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4600520541.html)
    
-   [CurrentRecord.setCurrentMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637579872.html)
    

Note:

With all APIs listed above, use the [Record.selectLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273169163.html) or [CurrentRecord.selectLine(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637580249.html) APIs first to select an existing line.

-   [Record.getMatrixSublistField(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4599708431.html)
    
-   [CurrentRecord.getMatrixSublistField(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637584261.html)
    
-   [Record.getMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4599712373.html)
    
-   [CurrentRecord.getMatrixSublistValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637584028.html)
    
-   [Record.findMatrixSublistLineWithValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4597993860.html)
    
-   [CurrentRecord.findMatrixSublistLineWithValue(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4637586269.html)
    

For more information about APIs, see [N/currentRecord Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html) and [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html).

### Related Topics

-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
