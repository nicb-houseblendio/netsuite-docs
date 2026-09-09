---
id: "section_N976686"
type: "section"
title: "Creating an Online Customer Form"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Capturing Leads > Online Customer Forms > Creating an Online Customer Form"
parent: "section_N976289"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976686.html"
anchors: ["procedure_N976802", "procedure_N976889", "procedure_N977168", "procedure_N977719", "procedure_N977821"]
sha256: "5ed6c1045c5bf580854f413716da0eeb222e64f58d01adad6872332b7f7961c5"
---

If you enable both the CRM and Sales Force Automation features, you can create online forms based on the NetSuite default template. You can also use your own HTML template for your forms. HTML templates let you customize your online forms to match your website's look. For more information about creating HTML form templates, read [Online Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981889.html).

To enable these features go to _Setup > Company > Enable Features_. On the **CRM** subtab, check the **Customer Relationship Management** and **Sales Force Automation** boxes, and then click **Save**.

#### To create an online customer form: {#procedure_N976802}

1.  Go to _Setup > Marketing > Setup Tasks > Online Customer Forms > New_.
    
2.  On the Select Type page, choose a template option:
    
    -   **Default Form Template**:
        
        -   Enter a title. This title appears at the top of the form.
            
        -   In the **Message** field, enter a message that your customers will see at the top of the form. This message can include up to 500 HTML characters.
            
        -   If you're using NetSuite OneWorld, use the default form template to pass the subsidiary to the online form using a URL.
            
    -   **Custom HTML Template**:
        
        -   Enter a title. This title appears at the top of the form.
            
        -   Select the HTML template you want to use for this form. For more information about creating HTML form templates, read [Online Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981889.html).
            
        -   If you want NetSuite to insert labels for your form fields, check the **Include Field Labels** box. If this box cleared, you must include field labels in your HTML template file.
            
3.  Check the **Enable Online** box to link to this form from a website.
    

#### To select fields: {#procedure_N976889}

1.  On the **Select Fields** subtab, in the **Field** column, select a field to include on the online customer form. Campaign Event associates an event with an online customer form.
    
    ![Screenshot of a portion of the Select Fields subtab and fields in the Field column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/5461captu_leads_form_.png)
2.  In the **Label** column, edit the name of the field as you want it to appear on the form.
    
3.  In the **Section** column, select the subtab for the field to appear on.
    
    You can create new subtabs for your forms at _Customization > Forms > Subtabs_. Click the **Entity** subtab, enter your new subtab, and then click **Save**.
    
4.  In the **Help** column, enter any text to appear below the field to aid your customers when filling out this form.
    
5.  In the **Width** column, enter the width for the field.
    
6.  If you want to require your customers to enter information in a field, check the box in the **Mandatory** column.
    
7.  To have NetSuite search existing records for information that matches what is entered in a field, check the box in the **Search** column.
    
    If the information closely resembles another record, determine how NetSuite proceeds in the **Handle Duplicate Records** field on the **Set Up Workflow** subtab.
    
    NetSuite requires this option for **First** and **Last Name** fields. You can also search for duplicated information in the following fields:
    
    -   company names
        
    -   email addresses
        
    -   phone numbers
        
    -   city
        
    -   state
        
    -   country
        
    -   postal codes
        
    -   information entered in custom fields
        
    
    Note:
    
    If you permit updates to address fields, the best practice is to make all of the address fields mandatory. Mandatory address fields ensure that no part of the address is overwritten.
    
8.  If you want a field to not show on the form, check the box in the **Hide** column.
    
    This is useful if you pass information into the form through the URL. For more information, see [Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979468.html). **Campaign Event** and **Lead Source** are two of the fields that you may want to mark as hidden. For example, you might want to include the **Lead Source** and **Campaign Event** fields on the form. This inclusion enables you to track the campaign effort that brought the customer to your company. However, you may want to hide this information from the person submitting the form.
    
9.  Check the box in the **Select** column if you want your customer to choose from a list in this field.
    
10.  Click **Add**.
     
11.  Repeat these steps for each field on the form.
     
12.  Use the **Move Up**, **Move Down**, **Move to Top**, and **Move to Bottom** buttons to change the order in which fields appear on your form.
     
13.  On the **Detail Message** subtab, enter a message you would like to appear at the bottom of the form.
     
     This message can include up to 4000 HTML characters.
     
14.  If you want NetSuite to define what information is updated on the Customer records, use the list in the **Update Customer** column.
     
15.  If the customer is a company, use the list in the **Update Contact** column to define what information is updated on the contact record.
     

#### To determine submission handling: {#procedure_N977168}

1.  Click the **Set Up Workflow** subtab.
    
2.  Under Preferences:
    
    1.  Check the **Create Customers as Companies** box if you want the customer record created according to the following:
        
        -   If no company name is entered on the form, create the customer record as an individual.
            
        -   If a company name is entered on the form, create the customer record as a company.
            
        
        Clear this box if you want customers to always be created as individuals.
        
        Note:
        
        If you create a company customer record, NetSuite creates a contact record and associates it with the customer. NetSuite only uses information that is applicable to contacts to create this contact record.
        
    2.  In the **Set Lead Status** field, select the customer status to assign to the person who submits the form.
        
        You can create new customer statuses at _Setup > Sales > Setup Tasks > Customer Statuses > New_.
        
    3.  Check the **Allow Update** box to update existing records with this status if the information entered on this form matches an existing record.
        
        You can only update records if you have checked a box in the **Search** column on the **Select Fields** subtab.
        
    4.  In the **Set Lead Source** field, select the lead source to associate with this form.
        
        This lead source appears in the **Lead Source** field on lead, prospect, and customer records.
        
    5.  Check the **Allow Update on Customers** and **Allow Update on Contacts** boxes to update existing records to show the lead source. Clear these boxes if you do not want to show the selected lead source on records.
        
        Note:
        
        You can update existing records only if you set one or more fields to be searched for when the form is submitted. If the search finds a matching record, NetSuite updates the existing record rather than creating a new record. Common search fields include **Email** and **Company Name**. To choose a search field, click **Select Fields** subtab. In the **Search** column, check the box next to the field you want to search for.
        
    6.  If you use NetSuite OneWorld, choose the default subsidiary when NetSuite creates the new record.
        
        For more information about setting the subsidiary on online forms, see [Subsidiaries on Online Customer Forms in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html).
        
    7.  To send your customer to another online customer form after submitting this form, select that form in the **Redirect to Form** field.
        
    8.  Enter the URL to redirect customers to after completing the form. This is a required field.
        
        Your web store home page URL appears by default.
        
    9.  In the **Handle Duplicate Records** field, select how NetSuite should proceed when information submitted on the form matches information in an existing record.
        
    10.  If you use the Duplicate Detection and Merge feature, check the **Use Duplicate Detection Criteria** box. NetSuite detects duplicates on the form using the criteria you set at _Setup > Company > Company Management > Duplicate Detection_.
         
3.  Under Customer Notification:
    
    1.  If you use the **Marketing Automation** feature, you can send an email message to the person who submits the form. Select an email template in the **Send Auto-Reply E-mail** field.
        
        To create email templates, go to Documents > Email Templates.
        
    2.  Enter a subject for the auto-reply email.
        
4.  Under Sales Rep Notification:
    
    1.  **Send E-mail Notification** - Check this box if you want the sales rep assigned to this customer to receive notification when the customer submits this form.
        
    2.  **Template for New Leads** - Select the email template you want to use to notify the assigned sales rep when a new lead, prospect, or customer submits this form.
        
    3.  **Template for Existing Customers** - Select the email template you want to use to notify the assigned sales rep when an existing lead, prospect, or customer submits this form.
        
        You can set the default templates for sales rep notification at _Setup > Marketing > Preferences > Marketing Preferences_. If you do not select a template, NetSuite sends a standard notification message.
        
    4.  If you would like others to receive notification when the form has been submitted, enter the email addresses in the **Cc** field.
        
        You can enter multiple email addresses by separating them with a comma or semicolon.
        

#### To set up the form's appearance: {#procedure_N977719}

1.  Click the **Set Up Appearance** subtab.
    
2.  The options differ based on the template you're using:
    
    -   If you're using the **Default Form Template**:
        
        -   Choose how many columns you want the form to be displayed in.
            
        -   Select a color theme for the form.
            
        -   Select a font for the form.
            
        -   Check the **Unlayered Sections** box if you want your form to appear without tabbed sections.
            
        -   Choose where to place the buttons on the form.
            
        -   Select a logo to place at the top of the form. You can upload new logos at _Commerce > Site Builder > Content > Images > New_.
            
    -   If you're using a **Custom HTML Template**, select a font for the form.
        

#### To add custom code: {#procedure_N977821}

1.  Click the **Custom Code** subtab.
    
    This subtab appears only if you use the **SuiteScript** feature.
    
2.  Select the JavaScript file that contains the scripts you want to use on this form. Check the **Available Without Login** box to ensure proper functionality.
    
    **Note:** Client scripts or scripts referenced on the client side can't have the **Hide in SuiteBundle** preference enabled on the script file record.
    
3.  In the **Page Init Function** field, select the script to call when the form loads.
    
4.  In the **Save Record** field, select the script to call when the form is submitted.
    
5.  In the **Validate Field Function** field, select the script to call when a field on the form is changed.
    
6.  In the **Changed Function** field, select the script to call when a change to a field is accepted.
    
7.  Click **Save**.
    
8.  Click **Preview Form** to review your form.
    

After saving your online customer form, you can publish the form or link to the form. To publish the form, create a customer form information item at _Commerce > Site Builder > Content Management > Publish Forms > New_. For more information, see [Case and Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html).

To link to the form, click the External subtab on the form record. Use the provided URL to link to this form on your website. When you link to the form, the form pops up in a new window.

NetSuite automatically creates or updates records when customers enter information on your website.

### Related Topics

-   [Passing Parameters Through URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N979468.html)
-   [Embedding an Online Form in your Website Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html#bridgehead_N2592052)
-   [Case and Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html)
-   [File Download with Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592134.html)
-   [Online Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N981889.html)
-   [Subsidiaries on Online Customer Forms in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
