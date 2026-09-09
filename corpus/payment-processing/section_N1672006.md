---
id: "section_N1672006"
type: "section"
title: "Sending Payment Notifications"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Managing Electronic Bank Payments > Sending Payment Notifications"
parent: "section_N1669310"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672006.html"
anchors: ["procedure_N1672026", "bridgehead_3867187266", "bridgehead_3898645710", "subsect_0722021718"]
sha256: "601b2de31dcd4da79f1425fc363050fcd210f7f201cb836c458f717caa2b37ef"
---

You can notify payees such as, vendors, employees, partners and customers that payment files have been created to process fund transfers to and from their bank accounts. You can also send notifications to notify payees that the payments made for them encountered errors.

To send a payment notification to an email address other than the default email address on the payee's entity record, you can enter multiple addresses in the **Email Address for Payment Notification** field on the main tab of vendor, employee, partner and customer records. To send a payment notification to additional recipients, enter multiple email addresses in this field separated by semicolons.

![Location of the Email Address for Payment Notification field in the Classification section, on the main tab of the Customer record.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EmailAddressForPaymentNotificationField.png)

Note:

If the **Email Address for Payment Notification** field is blank, email payment notifications are sent to the default email address specified on the entity record.

For information about using payment notification templates, see the following topics:

-   [Using Electronic Bank Payment Notification Templates](#bridgehead_3867187266)
    
-   [Adding Subsidiary Information to an Electronic Bank Payment Notification Template](#bridgehead_3898645710)
    

#### To send email notifications: {#procedure_N1672026}

1.  Go to Payments > Payment Processing > Payments File Administration.
    
2.  Click the View link next to the payment file for which you want to send email notifications.
    
3.  Click **Email Payment Notification.**
    
    ![Location of the Email Payment Notification button on the Payment File Administration page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EmailPaymentNotificationButton.png)
4.  In the **Subject** field of the Payment Notification form, change or accept the text for the Subject line of the email notification.
    
    ![Screenshot of location of Subject field on Payment Notification page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EP_SubjectField_PaymentsNotification.png)
5.  In the **From** field, enter a from email address that displays in the payment notification email sent to the customers. The **From** field value overrides the default **From Email Address** field value set in the Set Preferences page.
    
    The **From** field is optional and if left blank, the default email address is considered from the **From Email Address** field in the Set Preferences page. If the default email address is not set, then the email address from which you logged into your account will be used.
    
6.  Next, do one of the following:
    
    -   Type a message in the **Email Notes** field to create a custom email message and include a PDF of the transaction in your email, or
        
    -   Select an email template. Note that you must enable the **Advanced PDF/HTML Templates** feature for this option, and a PDF transaction is not included in the email notification.
        
        Note:
        
        This message is sent to all the payees that you select on the **Select Transactions** subtab.
        
7.  In the **Select** column on the **Select Transactions** subtab, check the box next to each payee to whom you want to send an email notification.
    
    Tip:
    
    Click **Mark All** or **Unmark All** to select or clear boxes, respectively, for all payees in the list.
    
8.  In the **Email Address** field, verify the email address or enter an email address if one doesn't exist. You can enter multiple email addresses separated by semi colon. Don't include spaces in this field.
    
9.  (Optional) In the **CC** and **BCC** columns, enter the email addresses to copy and blind copy other recipients. You can enter multiple email addresses separated by semi colon. Don't include spaces in this field.
    
10.  In the **Custom Email Notes** column, write the email message for the transaction. The text you enter here is sent only to recipients listed in the **Email Address**, **CC** and **BCC** fields on that transaction.
     
     Note:
     
     Text entered in the **Custom Email Notes** field replaces the message written in the **Email Notes** field or the **Email Template** selected for that particular Payee.
     
11.  Click **Submit**.
     

## Using Electronic Bank Payment Notification Templates {#bridgehead_3867187266}

There are two standard email templates that you can use for sending payment notifications:

-   **Standard Vendor Payment** - Use this template when sending notifications to vendors for bill payments,
    
-   **Standard Customer Payment** - Use this template when sending notifications to customers for direct debits, and to customers for refunds.
    

#### To select the template to use for payment notifications:

1.  Go to Payments > Setup > Electronic Payments Preferences.
    
2.  Click the **General Preference** subtab.
    
3.  Click Edit.
    
4.  In the **Email Template for Vendor Payments** field, select the template to use for payment notifications to vendors,
    
5.  In the **Email Template for Customer Payments** field, select the template to use for payment notifications to customers.
    
6.  Click Save.
    

You can also use custom email templates. There are two ways to customize email templates:

-   Download a standard template and customize it.
    
-   Customize an existing Advanced PDF/HTML template
    

#### To customize a standard template:

1.  Go to Documents > Files > File Cabinet > SuiteBundles, and then look for the Templates folder under the bundle number of the Electronic Bank Payments SuiteApp installed in your account.
    
    ![Location of Templates folder under the SuiteBundles menu item.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EP_EmailTemplates17.2.png)
    
    To see the latest bundle number in your account, go to _Customization > SuiteBundler > Search & Install Bundles > List_. On the Installed Bundles page, look for the bundle number of the Electronic Bank Payments SuiteApp in the **Bundle ID** column.
    
2.  Click Download next to the template you want to customize.
    
3.  Download the standard template and save it on your computer.
    
4.  Customize the template using Notepad or Notepad ++.
    
5.  Upload your customized template in the Templates folder of the File Cabinet.
    
    For instructions on adding files to the File Cabinet, see [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html).
    

#### To customize an existing Advanced PDF/HTML template:

1.  Using the template editor, review and change the layout. For more information, see [Advanced Templates Customization in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863632.html).
    
2.  When you have modified the layout to your specifications, click **Source**.
    
3.  Copy and paste the source XML code to a Notepad or Notepad++ file, and then save it on your computer.
    
4.  Upload the new template in the Templates folder of the File Cabinet.
    
    To locate the Templates folder, see Step 1 of To customize a standard template. For instructions on adding files to the File Cabinet, see [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html).
    

## Adding Subsidiary Information to an Electronic Bank Payment Notification Template {#bridgehead_3898645710}

The standard payment notification templates provided by Electronic Bank Payments don't include subsidiary information, such as the name and address of the subsidiary. If you want to include subsidiary information about the payment notifications that you send out, you need to customize an email template to add the relevant subsidiary fields.

#### To add subsidiary information to a payment notification template:

1.  Go to Documents > Files > File Cabinet > SuiteBundles, and then look for the Templates folder under the bundle number of the Electronic Bank Payments SuiteApp installed in your account.
    
    ![Location of Templates folder under the SuiteBundles menu item.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EP_EmailTemplates17.2.png)
    
    To see the latest bundle number in your account, go to _Customization > SuiteBundler > Search & Install Bundles > List_. On the Installed Bundles page, look for the bundle number of the Electronic Bank Payments SuiteApp in the **Bundle ID** column.
    
2.  Click the name of the email template that you want to customize.
    
3.  Copy the contents of the template and paste them into a new file using a text editor, such as Notepad++.
    
4.  Add the subsidiary information to the appropriate location on the new template using the following format:
    
    `${subsidiary.[field id]}`
    
    Note:
    
    To find the internal ID of a field, see [Finding Internal IDs of Record Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416043804.html)
    
    In the following example, the information to be added is the subsidiary address. The field ID of the **Address** field on the subsidiary record is **addrtext**.
    
    **Example:**
    
    `${subsidiary.addrtext}`
    
5.  Save the file with a new template name.
    
6.  Upload the file in the Templates folder of the File Cabinet.
    
    For instructions on adding files to the File Cabinet, see [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html).
    

When you use the new email template, the subsidiary address from the subsidiary record appears on the payment notifications.

![Subsidiary record showing an example subsidiary address that will appear on payment notifications.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EP_subsidiaryaddress.png) ![An example NetSuite payment voucher.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/EP_paymentvoucher.png)

## Customize Return Email Preferences {#subsect_0722021718}

You can use the **Return Email Address** field on the Payment Notification page to receive responses for the email notifications sent to the payment recipients.

You can customize return email preferences on the Electronic Payments Preferences page.

#### To customize return email preferences:

1.  Go to Payments > Setup > Electronic Payment Preference.
    
2.  From the **Return Email Address** list, select one of the following options:
    
    -   **Subsidiary Return Email Address** - This option retrieves the return email address set at the subsidiary level of the processed PFA
        
    -   **Company Return Email Address** - This option retrieves the return email address set on the Company Information page.
        
    -   **Custom Return Email Address** - This option retrieves the custom email return email address value set at the Electronic Payments Preferences page
        
        When you select **Custom Return Email Address**, the **Custom Return Email** field is enabled.
        
    -   If you don't select any option, then the **Return Email Address** field value is blank. The responses are received to the user who triggers the payment notifications.
        
        Note:
        
        A corresponding email address is automatically entered in the **Return Email Address** field on the Payment Notification page based on the option selected in the **Return Email Address** list on the Electronic Payments Preference page.
        
3.  Click **Save**.
    

### Related Topics:

-   [Managing Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669310.html)
-   [Setting Up Multiple Script Queues or Processors to Generate Payment File Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1669543.html)
-   [Setting Up Multi-Currency Payments Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670158.html)
-   [Viewing Electronic Bank Payment Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1670421.html)
-   [Reversing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672279.html)
-   [Rollback](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672610.html)
-   [Reprocessing Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1672857.html)
-   [Recreating a Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727317578.html)
-   [Verifying Issued Checks with Positive Pay](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673097.html)
-   [Setting Schedules for Payment Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1673790.html)
-   [Changing the Priority of a Queued Payment File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1674867.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
