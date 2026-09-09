---
id: "section_N1669543"
type: "section"
title: "Setting Up Multiple Script Queues or Processors to Generate Payment File Formats"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Multiple Script Queues or Processors to Generate Payment File Formats"
parent: "section_3831186542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html"
anchors: []
sha256: "4f8ac904138eecaead65b345e467d2d8ae890c66c1cfcaaa6a1c052be42a3130"
---

You can use multiple script queues or processors to divide processing of the script used by the Electronic Bank Payments SuiteApp for generating payment files.

Note:

Multiple script queues or processors for generating payment file formats require an active Electronic Bank Payments license and the NetSuite SuiteApps License Client installed in the account.

Starting from the 2019.1 release of the Electronic Bank Payments SuiteApp, new scripts will be used for the following processes:

-   Bill Payment Processing
    
-   Invoice Payment Processing
    
-   EFT and DD Instant Bank File Generation
    
-   Removed Unprocessed Transactions from PFA records
    
-   Rollback, Reversal, Recreate File, Email Notification of PFA records. This only includes PFA records that are created from processes that uses new scripts.
    

Old scripts, created with SuiteScript 1.0, will still be used for the following processes:

-   Batch Payment Processing
    
-   Customer Refund Processing
    
-   Positive Pay File Generation
    

Complete the following tasks to set up the Electronic Bank Payments SuiteApp to run multiple script queues or processors to generate payment file formats:

-   [Defining a New Deployment for the Electronic Bank Payment Processing Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1669612.html)
    
-   [Setting Up Multiple Queues for Payment Processing in the Electronic Payments Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1669861.html)
    
-   [Migrating Script Deployments to Use SuiteCloud Processors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1545122444.html)
    

### Related Topics

-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
