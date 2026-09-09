---
id: "section_N1670158"
type: "section"
title: "Setting Up Multi-Currency Payments Processing"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Multi-Currency Payments Processing"
parent: "section_3831186542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html"
anchors: ["procedure_N1670174"]
sha256: "495429c5606dd1682724e527114d0b6d42119bebc9dace7e8a62c94391f8c734"
---

The Electronic Bank Payments SuiteApp enables you to process multi-currency payments to suppliers and employees, to issue multi-currency customer refunds, and to receive multi-currency customer payments across the globe in a single payment run that uses a single bank account.

To process multi-currency transactions, you need to use a payment format that has a multi-currency option enabled. Examples are J.P. Morgan Freeform GMT and ABBL VIR 2000. Alternatively, you can create a new payment file format and enable its multi-currency options. In addition, you must use a bank account that has been set up to use the new multi-currency file format.

You can process multi-currency payment transactions only if your bank currency matches with your account's base currency. If the bank currency and account's base currency don't match then multi-currency transactions are not available to process on the Payment Processing page.

Note:

The Electronic Bank Payments license and the NetSuite SuiteApps License Client SuiteApp are required if you want to edit and create custom EFT and Direct Debit formats.

#### To create a new multi-currency payment file format: {#procedure_N1670174}

1.  Go to Payments > Setup > Payment File Templates > New.
    
2.  In the **Name** field, enter a name for this multi-currency payment file format.
    
3.  In the **Payment File Type** field, select one of the following:
    
    -   **EFT** - used for vendor payments
        
    -   **DD** - used for customer payments
        
4.  In the **Country** field, enter the name of the country.
    
5.  In the **Currency** field, select the currencies that you want to include in a single payment run when processing payments using the new payment file format. To select all available currencies, check the **Include All Currencies** box.
    
6.  Configure the following fields:
    
    -   **Reference Fields** - Enter custom fields you want to be visible on the Company Bank Details record.
        
    -   **Entity Reference Fields** - Enter custom fields you want to be visible on the Entity Bank Details record.
        
    -   **Field Validator** - Configure the validation for the **Company Bank Details** fields and **Entity Bank Detail** fields. You can validate a field by length or type. You can also use EP validation types such us BIC, Routing Number and IBAN. For more information, see [Adding Field Validations to Custom Payment File Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4005561610.html).
        
7.  In the **Maximum Lines** field, enter the maximum number of transactions that can be processed using this template.
    
    Note:
    
    A limit of 5,000 transactions can be processed in a single payment run.
    
8.  To automatically update the Entity Bank Details when payments are created in this format, check the **Update Entity Bank Details** box.
    
9.  In the **Bank File Template** field, enter the template body using FreeMarker syntax. If the SuiteTax feature is provisioned in your account, enter the template body in the **SuiteTax Bank File Template** field.
    
    Important:
    
    The Bank File Template field is targeted for the end of support soon. In preparation for this change,you should add your template body in the SuiteTax Bank File Template field. For more information, see the [Payment File Template Changes in NetSuite Electronic Bank Payments 2019.1](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1544059237.html).
    
    For more information about using the FreeMarker syntax on your custom templates, see [Working with Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4002314169.html). When using advanced templates, take note of the specific words that must not be used for your custom variables and function names. See the complete list of words in the topic, [Reserved Words](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4090351138.html).
    
10.  In the **Output File Extension** field, enter the file extension to use for the output payment file. For example, **txt**, **csv**, or **aba**.
     
11.  In the **Output File Encoding** field, select the character encoding type to use for the output payment file.
     
12.  Click **Save**.
     

Before you can use the new payment file format to process multi-currency transactions, you must set up the company bank account records you want to use for sending and receiving electronic bank payments.

Note:

For the multi-currency template to work, you must choose a company G/L bank account that uses the subsidiary base currency.

For more information about setting up bank details for electronic bank payments processing, refer to the Setting Up Bank Company Records topic for your country.

### Related Topics

-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
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
