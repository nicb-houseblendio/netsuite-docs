---
id: "section_N2552787"
type: "section"
title: "Debugging Your Shopping Cart Scripts Using Firebug"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Scriptable Cart > Testing and Debugging Scriptable Cart > Debugging Your Shopping Cart Scripts Using Firebug"
parent: "section_N2550105"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552787.html"
anchors: ["procedure_N2552826"]
sha256: "3bfbe4e08fb9a3c2125ac2c7b3e908013caabe7ade952410682bb7e8c4dba40b"
---

Most of the scripts you write for Scriptable Cart are client scripts. To debug your shopping cart scripts, use firebug to verify that your script runs properly in the NetSuite application. After you have verified your script works in the application, you can use SuiteScript to verify it functions properly in the web store. For more information, see [Debugging Your Scriptable Cart with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553048.html).

For debugging in the application, use [Firebug](http://getfirebug.com/) which integrates with the Firefox browser. Firebug is a free client application that includes a JavaScript debugger. Use Firebug to set breakpoints in your script for investigating your code.

#### To debug shopping cart scripts: {#procedure_N2552826}

1.  Go to Customization > Forms > Transaction Forms. Attach your script to a Standard Sales Order - Invoice or Standard Sales Order - Cash Sale form.
    
2.  Download Firebug.
    
3.  Launch Firebug.
    
    In the **Tools** menu of the Firefox window, select Firebug, then open Firebug.
    
4.  Log in to NetSuite.
    
5.  Go to Customization > Forms > Transaction Forms. Select the custom sales order form that has your script attached.
    
6.  Verify your script is running on the sales order form.
    
    1.  In the Firebug console, click **Script**, choose **Enabled**. Notice several scripts are listed in bold in the console. These are all the scripts NetSuite runs on this transaction form page.
        
    2.  Click the path to your script. Your script displays the path that ends with **/core/media.nl**. You can set break points to help you step through the code. Read the Firebug help documentation for more information about using Firebug.
        
7.  Enter data in the sales order and submit.
    

### Related Topics

-   [Testing Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2550200.html)
-   [Resolving Permission Errors in Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2552581.html)
-   [Debugging Your Scriptable Cart with SuiteScript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2553048.html)
-   [Deploying and Running Scriptable Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2549847.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
