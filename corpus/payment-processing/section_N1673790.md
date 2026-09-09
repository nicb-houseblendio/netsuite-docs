---
id: "section_N1673790"
type: "section"
title: "Setting Schedules for Payment Batches"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Setting Schedules for Payment Batches"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html"
anchors: ["procedure_3826931880", "bridgehead_4690054364"]
sha256: "2fe5b2e02d781d47aee17ff7de1df179e71fd9a55082a9347d12c6bd171389ea"
---

Set schedules for automatically creating or approving open payment batches of a bank account. For each schedule, you can specify the time and frequency at which batches are created or routed for approval.

Note:

Alternatively, without using payment schedules, you can route all open batches of a bank account for approval when you submit them on the Payment Batch List. For more information, see [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html).

On company bank records, assign payment schedules to saved searches that are used to retrieve transactions for a payment batch. Payment schedules are handled by a script deployment that has a default schedule, which you can update according to your business requirements. For more information, see the following topics:

-   To assign payment schedules to saved searches, see the Setting Up Company Bank Records topic for the specific country. For the complete list, see [Setting Up Bank Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html) or see the topics under [Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1675118.html).
    
-   For more information about the deployment for payment schedules, see [Viewing and updating the script deployment for payment schedules](#bridgehead_4690054364).
    

#### To set schedules for payment batches: {#procedure_3826931880}

1.  Go to Payments > Setup > Payment Schedule > New.
    
2.  Enter a name for this schedule.
    
3.  Select the time zone for this schedule.
    
    The **Time Zone** field displays the time zone setting of your NetSuite account. Your NetSuite account's time zone setting is used as a reference when scheduling the payment batch creation or submission for approval.
    
4.  In the **Event Type** field, select whether this schedule is for creating or routing a batch for approval.
    
    -   **Closing** - schedule that submits payment batches for approval. The status of the payment batch is changed from **Open** to **Pending Approval**.
        
    -   **Creation** - schedule that creates or updates open payment batches.
        
5.  On the **Recurrence** subtab, do the following: select your preferred time interval.
    
    1.  Set your preferred time interval.
        
        Note:
        
        Based on your interval settings, the **Next Scheduled Date** field automatically is updated with the date of the next payment batch creation or approval routing.
        
        -   To set intervals by number of days, select **Daily Event** from the first field and then set the frequency to either of the following options:
            
            | Field Value | Description |
            | --- | --- |
            | Repeat every | To set the frequency by a certain number of days:
            -   Select **Repeat every** from the second field.
            -   Enter the number of days in the third field.
            
             |
            | Repeat every weekday | To set the frequency to daily, except on weekends, select **Repeat every weekday** from the second field. |
            
        -   To set intervals by number of weeks, select **Weekly Event** from the first field and then set the frequency in the following fields:
            
            | Field | Description |
            | --- | --- |
            | Repeat every | Enter the number of weeks before the next payment batches are created or approved. |
            | week(s) on | Select the day of the week when payment batches are created or approved. |
            
        -   To set a monthly schedule, select **Monthly Event** from the first field and then set the frequency to either of the following options:
            
            | Field Value | Description |
            | --- | --- |
            | Day | To set the frequency to a specific calendar day of the month:
            -   Select **Day** from the second field.
            -   In the third field, enter a number from 1 to 31 for the particular day of every month when payment batches are created or approved. For example, you entered 25 for the day. If the current date is April 2, the next payment batch creation or approval is scheduled on April 25.
            
             |
            | The | To set the frequency to a specific day of the week per month:
            
            -   Select **The** from the second field.
            -   In the third field, select the week number within the month from the following options: **first**, **second**, **third**, **fourth**, or **last**.
            -   In the fourth field, select the day of the week from the following options: **Sunday, Monday, Tuesday, Wednesday, Thursday, Friday,** or **Saturday.** For example, you selected third for the week number and Tuesday for the day of the week. If the current date is April 2, the next payment batch creation or approval is scheduled on the third Tuesday of April.
            
             |
            
    2.  In the **Start Time** field, select the time when you want to start the payment batch creation or submission for approval.
        
6.  Click **Save**.
    

Note:

Automated batch payment processing requires the Electronic Bank Payments license and the NetSuite SuiteApps License Client to be installed in the account. If your license expires, existing payment schedules that automatically creates the payment batches will no longer run. As soon as you renew your license, you must update your payment schedule record.

For more information, see [Update Payment Schedule After Advanced Electronic Bank Payments License is Renewed](https://suiteanswers.custhelp.com/app/answers/detail/a_id/81975/kw/81975), SuiteAnswers ID 81975.

## Viewing and updating the script deployment for payment schedules {#bridgehead_4690054364}

The script deployment, `customdeploy_8859_batch_processing_ss`, handles the script for batch payment schedules. To view the deployment record, go to _Customization > Scripting > Script Deployments_. From the list of deployments, look for the record ID under the **ID** column.

-   To use a payment schedule, verify that the script deployment is set to **Scheduled** status.
    
-   By default, this deployment is scheduled to repeat every hour. You can change the default to schedule the deployment to repeat every half hour based on your business requirements. Regardless of the frequency, the scheduled script is queued for processing, so it might not run at the exact time indicated on the record. For example, using the deployment's default start time of 6 p.m., a payment schedule with a start time of 6:20 p.m. might still be included in the 6 p.m. run. For instructions on editing a script deployment, see [Updating a Script Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4515651225.html).
    
-   For each scheduled script run, there is a maximum limit of 80 company bank detail records that can be processed for all payment schedules included in the run. You can set multiple payment schedules to be included in the 7 p.m. run, for example, but be sure that they don't exceed 80 bank records combined.
    

### Related Topics

-   [Processing Bills and Expenses in Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1665332.html)
-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
