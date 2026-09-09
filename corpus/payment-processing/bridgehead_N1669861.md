---
id: "bridgehead_N1669861"
type: "bridgehead"
title: "Setting Up Multiple Queues for Payment Processing in the Electronic Payments Preferences"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Multiple Script Queues or Processors to Generate Payment File Formats > Setting Up Multiple Queues for Payment Processing in the Electronic Payments Preferences"
parent: "section_N1669543"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1669861.html"
anchors: ["procedure_N1669874"]
sha256: "c27d09a9ac3685683aa8e09baabb7057b07a0cc1c61d809801837bbb24f6d69b"
---

After creating the deployment definitions, you must set them up by entering the script deployment ID for each payment processing script that you want to run concurrently.

Note:

If you have existing multiple queues, the new column fields for these queues will be left blank initially. The default SuiteScript 2.0 scripts will be used until you have allocated your own scripts.

#### To set up the deployment definitions: {#procedure_N1669874}

1.  Go to Payments > Setup > Electronic Payments Preferences.
    
2.  Click **Edit**.
    
3.  On the **Queue Management** subtab, complete the following fields:
    
    | Field | Description |
    | --- | --- |
    | Subsidiary | Select the subsidiaries that'll share the same script queues. Leave this field blank to share the script queue with subsidiaries that do not have any script queue setting. Shared queues among subsidiaries results to queuing for payment files submitted by these subsidiaries. |
    | Scheduler (New) | Enter the script deployment ID for Payment Scheduler. Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing and PFAs using Instant Bank File Generation. |
    | Transaction Marking (New) | Enter the script deployment ID for Transaction Marking. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Scheduler (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing. |
    | Payment Processing (New) | Enter the script deployment ID for Payment Processing. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Transaction Marking (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing. |
    | Bank File Creation (New) | Enter the script deployment ID for Bank File Creation. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Payment Processing (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing and PFAs using Instant Bank File Generation. |
    | Rollback (New) | Enter the script deployment ID for Rollback. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Bank file Creation (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing. |
    | Reversal (New) | Enter the script deployment ID for Reversal. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Rollback (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing and PFAs using Instant Bank File Generation. |
    | Notification (New) | Enter the script deployment ID for Notification. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Reversal (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing and PFAs using Instant Bank File Generation. |
    | Instant Payment Processing (New) | Enter the script deployment ID for Instant Payment Processing. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Notification (New). Applicable to new PFAs created using EFT and DD formats Instant Bank File Generation. |
    | Remove Unprocessed Transaction (New) | Enter the script deployment ID for Remove Unprocessed Transaction. For script deployments that are still using queues, make sure that the script queue is the same as the script queue in Instant Payment Processing (New). Applicable to new PFAs created using EFT and DD formats for Regular Payment Processing. |
    | Parent Deployment (Old) | Enter the script deployment ID for Generic Payment Processing. The script queue for this deployment must be different from the queue number that was set up for the Generic Payment Processing deployment. Applicable to Customer Refunds and Positive Pay format. |
    | Payment Creator Deployment (Old) | Select the script deployment ID for Generic Payment Record Processing. Applicable to Customer Refunds and Positive Pay format. Note: To use multi-threading and to optimize usage of the queues, select multiple script deployment IDs and make sure that at least one of the script deployments has the same script queue as the Parent Deployment. This is only applicable to script deployments that are still using queues. |
    | Rollback Deployment (Old) | Enter the script deployment ID for Generic Payment Rollback. Make sure that the script queue is the same as the script queue in Parent Deployment. Applicable to Batch Payment, Customer Refund, and Positive Pay processing. |
    | Reversal Deployment (Old) | Enter the script deployment ID for Generic Payment Reversals. Make sure that the script queue is the same as the script queue in Parent Deployment. Applicable to Batch Payment, Customer Refund, and Positive Pay processing. |
    | Notification Deployment (Old) | Enter the script deployment ID for Generic Payment Notification. Make sure that the script queue is the same as the script queue in Parent Deployment. Applicable to Batch Payment, Customer Refund, and Positive Pay processing. |
    | Batch Processing Deployment (Old) | Enter the script deployment ID for On Demand Batch Processing. Make sure that the script queue is the same as the script queue in Parent Deployment. Applicable to Batch Payment, Customer Refund, and Positive Pay processing. |
    
    Note:
    
    You must complete all the fields.
    
4.  Click **Add**.
    
5.  Repeat steps 2 and 3 to add more script queue settings for other subsidiaries.
    
6.  Click **Save**.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
