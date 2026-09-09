---
id: "section_N1673097"
type: "section"
title: "Verifying Issued Checks with Positive Pay"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Verifying Issued Checks with Positive Pay"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html"
anchors: ["procedure_N1673160"]
sha256: "edadff76336604e8dc56baeabbb3e6f72efb5c3fa4e4252fcb7adf8d8f38baf2"
---

The current version of the Electronic Bank Payments SuiteApp supports Positive Pay verification for the following transaction types:

-   Bill Payment
    
-   Check
    
-   Customer Refund
    
-   Cash Refund
    
-   Paycheck
    
-   Sales Tax Payment
    
-   Vendor Prepayment
    

#### To generate Positive Pay file formats: {#procedure_N1673160}

1.  Go to Payments > Cheques > Positive Pay.
    
2.  Complete the following fields:
    
    | Fields | Description |
    | --- | --- |
    | Bank Account | Select the bank account where the customer refund payments are posted. For more information about setting up your company's bank account details for electronic bank payments, see [Setting Up Bank Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html). The **Bank Account Format**, **Maximum Payments in File**, and **Subsidiary** fields are automatically updated based on the value in this field. Note: If **Maximum Payments in File** displays zero, no available check transaction is displayed in the Select Transactions list. You must return to the custom Payment File format and make sure that the **Maximum** **Lines** field is not set to blank. |
    | Date From | Use this field to show checks issued on this date or later. To include checks issued within a range of dates, enter values for both **Date From** and **Date To** fields. |
    | Date To | Use this field to show checks issued on this date and earlier. To include checks issued within a range of dates, enter values in the **Date From** and **Date To** fields. |
    | Cheque From | Enter the starting check number in a range of checks included in the file format. Checks with numbers lower than this value are excluded in the file format. |
    | Cheque To | Enter the last check number in a range of checks to include in the file format. Checks with numbers higher than this value are excluded in the file format. |
    | Include Void Cheques | Check this box to include checks that are voided through a reverse journal entry. For more information, see [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html). |
    | Exclude Cleared Cheques | Check this box to exclude checks that were cleared in your bank register. |
    
    A list of eligible check transactions is displayed in the Select Transactions list. You can use the search results as a reference for check verification activities.
    
    Note:
    
    To display the **Name** column, go to Payments > Setup > Electronic Payments Preferences, click the **General Preference** subtab, and check the **Include Name in Transaction List** box.
    
3.  Click **Submit**.
    
    The Payment File Administration record containing the details of the generated Positive Pay file format is displayed. You can do the following:
    
    -   Click **Refresh** for the SuiteApp to finish processing the file format and to display the downloadable text file format in the **File Reference** field.
        
    -   Click the download link in the **File Reference** field to download the Positive Pay file format. You can send the file format to your bank online, or upload the file to your bank's Positive Pay system.
        
    -   For more information about viewing payment details, see [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html).
        

### Related Topics

-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Sending Payment Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
