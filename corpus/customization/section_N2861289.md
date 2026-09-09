---
id: "section_N2861289"
type: "section"
title: "Linking Transaction Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Linking Transaction Forms"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html"
anchors: ["procedure_N2861319"]
sha256: "8f47aa150a8231d7024a6de15ae579ab17b7268d5f56fa301171393ab123cad2"
---

On the Linked Forms subtab, you can specify which transaction form is used when you transform one transaction into another. You can create a chain of transaction forms that mirror your business workflow.

For example, a company has three custom sales order forms that are each used for a certain set of items they sell. When one of these sales orders is used to create a picking ticket, the specific picking ticket form created for each type of sales order is used. The employee creating the picking ticket does not have to search the custom form list to find the proper picking ticket form.

To set up this form workflow, the company administrator edits the custom sales order form, and selects the picking ticket form on the Linked Forms subtab.

When you transform a transaction you created with a custom transaction form, the custom form set on the Linked Forms subtab is selected by default. In the preceding example, when one of the sales orders is used to print a picking ticket, the custom picking ticket form selected on the sales order form is used by default.

#### To set up linked forms: {#procedure_N2861319}

1.  Open the custom entry form or custom transaction form you want to create the linkage from. For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).
    
2.  Click the **Linked Forms** subtab.
    
    A list of the transactions that you can transform to from the type of transaction form you're customizing is shown. For example, if you're customizing an estimate form, you can link forms for cash sales, invoices, and sales orders.
    
3.  In the **Custom Form** column, select the standard or custom form for each transaction.
    
    If you want to use the preferred form for the transaction type, don't specify a linked form for that transaction type.
    
4.  Click **Save**.
    

When the transaction is transformed, the correct transaction form is used automatically.

Note:

If the person is assigned a role that's restricted to use only specific transaction forms, the forms set for that role override the forms you've set on the **Linked Forms** subtab.

### Related Topics

-   [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html)
-   [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html)
-   [Custom Transaction Forms Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html)
-   [Storing Custom Forms with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2854025.html)
-   [Configuring Subtabs for Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2855162.html)
-   [Moving Fields and Lists Between Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860592.html)
-   [Configuring Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856559.html)
-   [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html)
-   [Configuring Buttons and Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857647.html)
-   [Configuring Printing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858172.html)
-   [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html)
-   [Configuring Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515597095.html)
-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
-   [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html)
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
