---
id: "bridgehead_N1669612"
type: "bridgehead"
title: "Defining a New Deployment for the Electronic Bank Payment Processing Scripts"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Multiple Script Queues or Processors to Generate Payment File Formats > Defining a New Deployment for the Electronic Bank Payment Processing Scripts"
parent: "section_N1669543"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1669612.html"
anchors: ["procedure_N1669626"]
sha256: "0214d527214b8329b38e23f0c309a723c0ff35f48cda0c9e7e63d9ed6534e555"
---

You can define multiple script deployments for scheduled scripts and on demand batch processing of Payment File Administration records, using the same queue assigned for payment processing in a particular subsidiary. It's advisable that you use queues that are dedicated to Electronic Bank Payments Processing.

#### To define a new deployment for Electronic Bank Payments processing scripts: {#procedure_N1669626}

1.  Go to _Customization > Scripting > Scripts_ (Administrator).
    
2.  Create multiple script deployments for each of the following script queues that you dedicate to Electronic Bank Payments processing:
    
    -   EP Script Scheduler
        
    -   EP Transaction Marker
        
    -   EP Payment Processor
        
    -   Payment File Generation SS
        
    -   EP Rollback MR
        
    -   EP Reverse Payments MR
        
    -   EP Email Notification MR
        
    -   Payment to Admin Linker MR
        
    -   EP Failed Transaction Unlinker
        
    -   Generic Payment Processing
        
    -   Generic Payment Record Processing
        
    -   Generic Payment Notification
        
    -   Generic Payment Reversals
        
    -   Generic Payment Rollback
        
    -   On Demand Batch Processing (8859\_payment\_batch\_on\_demand)
        
3.  Click the View link next to the script record.
    
4.  Click **Deploy Script**.
    
5.  Complete the following fields on the New Script Deployment page:
    
    | Field | Description |
    | --- | --- |
    | Title | Enter a name for the new script deployment definition. |
    | ID | Enter a unique ID for the new script deployment definition. |
    | Priority | Select how urgently this script should be processed relative to other map/reduce and scheduled scripts that have been submitted. This value is assigned to each job associated with the script deployment. For more information, see [Priority](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509578980.html#subsect_1509391777). Important: You must understand [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html) before you change this setting. For details, see [SuiteCloud Processors Priority Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505170702.html). |
    | Concurrency Limit | Set the number of [SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1498571420.html) that can be used to process the jobs associated with the script deployment. For more details on this field, see [Concurrency Limit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509578980.html#subsect_1509134710). Note: For accounts without SuiteCloud Plus License, you can set the Concurrency Limit to 2. This enables the use of the extra processor to double the processing bandwidth for your map/reduce scripts. For more information, see SuiteAnswers support article [Electronic Bank Payments: Improve Payment Batch Processing and Payment File Generation Performance by Increasing the Concurrency Limit](https://suiteanswers.custhelp.com/app/answers/detail/a_id/81974/kw/81974), ID 81974. |
    
6.  Click **Save**.
    
    New Deployments are added to the list on the **Deployments** subtab of the script record from which it was created.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
