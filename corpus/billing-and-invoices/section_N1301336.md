---
id: "section_N1301336"
type: "section"
title: "Printing Mini Statements"
branch: "billing-and-invoices"
category: "order-management"
breadcrumb: "Order Management > Billing and Invoices > Invoices > Customer Statements > Printing Mini Statements"
parent: "section_N1300430"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1301336.html"
anchors: ["procedure_N1301374", "procedure_N1301460"]
sha256: "2f4c3a967d76bcf4f261c0f0354e6a8bf63d4a657dec31aaead8ce557c17b156"
---

You can print a mini-statement at the bottom of invoices that show the customer's current balance and aging totals. This is the same information that shows at the bottom of regular customer statements.

Note:

If you use the Consolidated Payments feature, mini-statements show the consolidated balance and aging amounts for individual customers instead of the consolidated balance. For more information, see [Consolidated Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1288474.html).

To print the mini-statement in HTML or PDF layout, customize your invoice transaction form first. If you print in PDF Layout, you should also set your PDF form layout to do so.

#### To customize invoices to print mini-statements: {#procedure_N1301374}

1.  Go to _Customization > Forms > Transaction Forms_ (Administrator).
    
2.  Click **Customize** next to the form you want to add the mini-statement to.
    
3.  On the new Custom Transaction Form page, in the **Name** field, enter a name for the new custom form.
    
4.  Check the **Form is Preferred** box.
    
5.  Select **Basic** to set the printing type.
    
6.  Click the Printing Fields subtab.
    
7.  On the Printing Fields subtab, click the Footer subtab, and check the **Print/Email** box for Aging:Current.
    
8.  Click **Save**.
    

Now, invoices can print the mini-statement in HTML format. If you don't print statements in PDF format, you don't need to take additional steps.

To print mini-statements on invoices using PDF format, you should use a PDF transaction form layout that includes statement aging fields. You can select a standard layout or customize a standard layout.

#### To set your PDF form to print mini-statements: {#procedure_N1301460}

1.  Go to _Customization > Forms > Transaction Form PDF Layouts_ (administrator).
    
2.  Select a PDF transaction form layout that includes statement aging fields:
    
    -   To select a standard layout, check the **Preferred** box next to the layout you want. There are four layouts that include statement aging fields:
        
        -   Standard Aging Invoice Layout
            
        -   Classic Aging Invoice Layout
            
        -   Standard Aging/Disclaimer Invoice Layout
            
        -   Classic Aging/Disclaimer Invoice Layout
            
    -   To customize a layout, click **Customize** next to one of the four layouts that include statement aging fields. Then, enter your customization choices for the layout and check the **Layout is Preferred** box.
        
3.  Click **Save** or **Submit**.
    

### Related Topics:

-   [Customer Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300430.html)
-   [Generating Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300518.html)
-   [Printing a Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1300905.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html)
-   [Using the Billing Tab and Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4483926245.html)
-   [Global Invoicing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1237960.html)
-   [Creating an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1238506.html)
-   [Choosing an Invoice Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240040.html)
-   [Billing Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4063198073.html)
-   [Billing or Invoicing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1240951.html)
-   [Invoicing Billable Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1241287.html)
-   [Closing or Voiding an Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158654862294.html)
-   [Creating Installments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1540928779.html)
-   [Progress Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1243687.html)
-   [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
