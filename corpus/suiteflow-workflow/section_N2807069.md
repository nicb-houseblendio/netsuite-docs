---
id: "section_N2807069"
type: "section"
title: "Storing a Return Value from a Custom Action Script in a Workflow Field"
branch: "suiteflow-workflow"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteFlow (Workflow) > Workflow Samples > Storing a Return Value from a Custom Action Script in a Workflow Field"
parent: "chapter_N2796642"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2807069.html"
anchors: ["procedure_N2807106"]
sha256: "8eb393ea0565d3dd33cd77d030dabd59e8917994a98084390d06bec3513ddf67"
---

This sample shows how to store a return value from a custom action script into a workflow field. This example can be useful in the following cases:

1.  You want to get a value from the Item sublist and use this value as a condition in the workflow. You use obj.getSublistValue in the script and return this in the workflow.
    
2.  You want to check if a certain item is existing in the Item sublist. The script returns "0" if item is not existing and "1" if it does.
    
3.  You want to make sure that all items in the Item sublist have a quantity equal to or greater than 1 (similar case as #2).
    

#### To store a return value from a custom action script in a custom field: {#procedure_N2807106}

1.  Create a new Workflow Action script.
    
    This script is an example.
    
                    `/**  * @NApiVersion 2.x  * @NScriptType WorkflowActionScript  */ define([],     function() {         function onAction(scriptContext) {             log.debug({                 title: 'Start Script'             });             var newRecord = scriptContext.newRecord;             var itemCount = newRecord.getLineCount({                                 sublistId: 'item'                                 });             log.debug({                 title: 'Item Count',                  details: itemCount             });             for(var i = 0; i < itemCount; i++)             {                 var quantity = newRecord.getSublistValue({                                    sublistId: 'item',                                     fieldId: 'quantity',                                     line: i                                });                 log.debug({                     title: 'Quantity of Item ' + i,                      details: quantity                 });                 if(quantity === 0)                 {                     return 0;                 }             }             log.debug({                 title: 'End Script'             });             return 1;         }         return {             onAction: onAction         }     });` 
                  
    
2.  You need to make sure that the script returns a value. On the Script record page, on the **Parameters** tab, select a value from the **Return Type** list.
    
3.  In SuiteFlow, create a workflow field. The field should be the of the same type as the return parameter of the Workflow Action script.
    
    ![A screenshot showing the Type field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/StoreReturnValueWorkflowField_19.1.png)
4.  Within a state, add the custom action (this is the Workflow Action script).
    
    ![Screenshot of the custom action options.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/StoreReturnValueCustomAction.png)
    
    The return value from the Workflow Action script can be stored in the **Store Result In** field.
    
    ![A screenshot of the Workflow Action script being set to be stored in Return Value (Workflow) field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteFlowWorkflow/StoreReturnValueParameters.png)

### Related Topics

-   [Workflow Samples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2796642.html)
-   [Lead Nurturing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2797000.html)
-   [Lead that Did Not Convert to Customer Within Three Days](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801202.html)
-   [Estimate Approval Routing Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2801522.html)
-   [Welcome Email Sent to Customers Three Days After First Order Workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2806856.html)
-   [Custom Action](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2752089.html)
-   [Creating and Using Workflow Action Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158378266601.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
