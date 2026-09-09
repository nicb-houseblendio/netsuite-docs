---
id: "section_N2549847"
type: "section"
title: "Deploying and Running Scriptable Cart"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Deploying and Running Scriptable Cart"
parent: "chapter_N2545000"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html"
anchors: ["procedure_N2549883"]
sha256: "276ed377e4b37dbeb8d00a33f150649e62d8e2d3edbb1b7be9b76abb6fafc3df"
---

Scriptable Cart runs customized sales order forms you select as Scripting Templates. These sales order forms contain the order while customers are shopping on your web store. Your custom SuiteScript is attached to these forms.

To run SuiteScript in the shopping cart, an administrator must enable the following features: Advanced Site Customization, Client SuiteScript.

Note that creating a script record is the first step when using SuiteScript in the shopping cart, however it is the fourth step when creating a script in a non-web store context. For general information about creating a script record, see [SuiteScript 1.0 Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7151939532.html).

#### To deploy a script in the shopping cart: {#procedure_N2549883}

1.  Go to Customization > Forms > Transaction Forms.
    
    Customize a sales order form for use in the shopping cart by attaching SuiteScript. If you use terms for your customers, you must attach your script to both types of sales order forms: cash sale and invoice. For more information read the FAQ topic, [What type of sales order forms can I use for the Scriptable Cart?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html#question_N2553515)
    
    Note:
    
    It is important that the fields on the custom sales order form correspond with features you have enabled in your account. For example: If you use a script that reads revenue recognition fields, you must include these fields on your custom sales order form.
    
2.  Go to _Commerce > Websites > Website List_.
    
    Click **Edit** next to the required website.
    
3.  Click the **Setup** tab.
    
4.  In the Preferences section, check the **Scriptable Cart and Checkout** box.
    
5.  Set the Scripting Templates for your site:
    
    -   **Scripting Template (Credit Card)** - Select your customized Sales Order - Cash Sale form.
        
    -   **Scripting Template (Invoice)** - Select your customized Sales Order - Invoice form.
        
6.  Click **Save**.
    

Based on the sales order form you select as a Scripting Template, your custom script executes against data in the shopping cart.

Important:

When you set a script deployment record to Released, you must select the correct customer center role for the script to run in the shopping cart. The role you select on the script deployment must be the same customer center role you have selected in the **Default Role for New Customers** field at Setup > Company > General Preferences.

Before you deploy a script to run in the shopping cart, test your script thoroughly. For more information, see [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html).

For more information about the client events available in the Scriptable Cart, see [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html).

### Related Topics

-   [SuiteScript for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2545233.html)
-   [Creating Customer-Facing Messages from Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2548158.html)
-   [Custom Error Messages for ValidateLine Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549673.html)
-   [Testing and Debugging Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550105.html)
-   [Scriptable Cart FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553295.html)
-   [Sample Scripts for Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553996.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
