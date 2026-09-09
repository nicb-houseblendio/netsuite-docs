---
id: "section_N2863334"
type: "section"
title: "Setting Custom Forms to Use Advanced Templates"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced PDF/HTML Templates > Setting Custom Forms to Use Advanced Templates"
parent: "chapter_4453550706"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863334.html"
anchors: ["procedure_N2863353", "subsect_163731920013"]
sha256: "3c959b3ff1219956c58813a4949c75d101cbcc195d5f01f174d2ce4b109da757"
---

When the Advanced PDF/HTML Templates feature is enabled, you can set custom forms for supported transaction types to use advanced templates. When you set a custom form to use an advanced template, that template defines the print and email formatting and contents for transactions that use that custom form.

Note:

If your organization uses the multiple currency feature and advanced printing statements, the template needs to allow for multiple currencies by using list record instead of record root. The Standard Multiple Currency Statement provides an example of how to set up the template.

For an example of a printed form that uses an advanced template, see [Printed Invoice Using Advanced Template](#subsect_163731920013).

#### To define an advanced template for a custom form: {#procedure_N2863353}

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  On the Custom Transaction Forms page, click **Edit** for a custom form or **Customize** for a standard form.
    
3.  On the Edit page for the custom form, review the **Printing Type** options.
    
    -   **Basic** to associate basic PDF layouts and HTML layouts with the custom form.
        
    -   **Advanced** to associate advanced templates with the custom form.
        
4.  Choose a print template and an email template from the dropdown lists.
    
    -   The **Print Template** and **Email Template** dropdown lists contain the standard advanced template and any custom advanced templates for the transaction type.
        
    -   You can select one advanced template for printed transactions and a different template for transactions sent by email. These templates are used for both PDF and HTML formatting.
        
    -   The preferred advanced template is selected by default in the dropdown lists.
        
        ![Custom Transaction Form page with Print Template and Email Template settings outlined in red.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/SetTemplateCustForm.png)

![Sample Purchase Order page with the Custom Form field outlined in red.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/advprintcustformselection.png)

Important:

At any time after you've set a custom form to use an advanced template, you can switch the form back to using basic layouts. Edit the custom form and select **Basic** for **Printing Type**, and choose from the **PDF Layout** and **HTML Layout** dropdown lists. All previously available basic layouts are still available.

When creating a transaction, you can save the transaction and email it as a PDF attachment by clicking Save & Email. The PDF attachment uses the customer's preferred language.

## Printed Invoice Using Advanced Template {#subsect_163731920013}

The following invoice uses the Standard Invoice PDF/HTML Template:

![Sample invoice using an advanced template.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/PrintedSalesOrderBetter.png)

### Related Topics

-   [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html)
-   [Using Advanced Template Formatting Programmatically](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2862762.html)
-   [Account-Specific Domains in Advanced Printing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_159560197793.html)
-   [Enabling the Advanced PDF/HTML Templates Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2862977.html)
-   [Reviewing Available Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863143.html)
-   [Advanced PDF/HTML Multi-Currency Statement Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4364689607.html)
-   [Advanced Templates Customization in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2863632.html)
-   [Scripting with Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1533138530.html)
-   [XML Formatting in Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158204583926.html)
-   [Changing the Script ID of a Custom Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515580300.html)
-   [Advanced Templates for Printing Saved Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4823423235.html)
-   [Advanced Templates Support for Company Printing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950986508.html)
-   [FAQs for Advanced Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159984373188.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
