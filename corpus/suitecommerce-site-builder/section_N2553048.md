---
id: "section_N2553048"
type: "section"
title: "Debugging Your Scriptable Cart with SuiteScript"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Testing and Debugging Scriptable Cart > Debugging Your Scriptable Cart with SuiteScript"
parent: "section_N2550105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553048.html"
anchors: []
sha256: "446b048d53bb938886a7ec35f7bf4bfa824d42ac9c93708da197823b57254ae0"
---

To obtain debug messages, typically you must use record-level deployments. The steps below describe how to use a form-level deployment to generate debugging messages.

1.  Go to Customization > Forms > Transaction Forms.
    
    1.  Customize a **Standard Sales Order - Invoice**, and a **Standard Sales Order - Cash Sale** form. Do not include custom code on either form. You will use these for testing.
        
    2.  After you create the two new forms, make a note of their Internal IDs.
        
2.  Create an alternate version of your scriptable cart script. Keep your original script as your backup.
    
    At the top of each event function, add the following code:
    
                  `if (nlapiGetFieldValue('customform') != '[InternalID of Sales Order - Invoice from Step 1]' &&   nlapiGetFieldValue('customform') != '[InternalID of Sales Order - CashSale from Step 1]'  {       return; }` 
                
    
    This code ensures that the script only fires for the sales order forms you are using on the web store.
    
    Note:
    
    Use an nlapiLogExecution() call each time you want to output a debugging message.
    
3.  Create a new client script, and then deploy it for all sales order forms.
    
    1.  Go to Customization > Scripting > Scripts > New > Client Script.
        
    2.  Enter event functions, and attach any library scripts.
        
    3.  On the **Deployments** subtab, in the **Applies to** column, select **Sales Orders**.
        
    4.  Click **Save & Deploy**.
        
    5.  On the **Audience** subtab of the script deployment record, make sure that **Customer Center** is selected.
        
4.  Select the newly created sales order forms as the **Scriptable Template** for your web store.
    
    1.  Go to _Commerce > Websites > Website List_.
        
    2.  Click **Edit** next to your website name.
        
    3.  In the Preferences section, set the Scripting Templates for your site:
        
        -   **Scripting Template (Credit Card)** - Select your customized Sales Order - Cash Sale form.
            
        -   **Scripting Template (Invoice)** - Select your customized Sales Order - Invoice form.
            

To view the logs, go to the script or the script deployment record, and click the Execution Log tab.

### Related Topics

-   [Testing Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550200.html)
-   [Resolving Permission Errors in Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552581.html)
-   [Debugging Your Shopping Cart Scripts Using Firebug](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552787.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
