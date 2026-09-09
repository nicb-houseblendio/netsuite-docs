---
id: "section_N2858172"
type: "section"
title: "Configuring Printing Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring Printing Fields"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858172.html"
anchors: ["procedure_N2858204", "bridgehead_N2858334", "bridgehead_N2858382"]
sha256: "e11b807454d7b612c6ed58735eeb847139e3891662ceb0ea6f7a3cb02ffb4cdd"
---

Configuration of Printing Fields is required for Transaction Forms only that use basic printing.

On the Printing Fields subtab, you can customize the way your form appears when printed. The Printing Fields subtabs represent the various areas of a printed form.

#### To configure how each section of your printed form displays: {#procedure_N2858204}

Note:

Any configurations made on the Printing Fields subtab are visible only on the printed form.

1.  For all subtabs on the Printing Fields subtab:
    
    -   In the **Print/Email** column, check the boxes next to fields you want to appear on printed and emailed forms.
        
        This column also controls the visibility of a field in the Customer Center. Check the boxes next to fields you want to appear in the Customer Center.
        
    -   In the **Label** column, edit the labels of the fields as needed.
        
    
    Note:
    
    If you change the label for a field on the **Printing Fields** subtab, the label is also automatically applied to the field on the **Sublist Fields** subtab.
    
2.  For the **Body** and **Columns** subtabs:
    
    -   In the **Width** column, enter the width for transaction column fields appearing on your printed and emailed forms.
        
        Note:
        
        To change the width of custom body fields, you must make the change on the Custom Form page. The width you set on the custom field does not affect printed transaction body fields.
        
    -   Rearrange fields as needed. Select and drag each line item to the preferred position.
        
3.  Click **Save**.
    

Important:

If the Advanced Taxes feature is enabled in your account, or if you're using NetSuite OneWorld, which requires Advanced Taxes, you can't directly rename tax fields on a custom transaction form. To change tax field names on a custom form, rename them in the appropriate languages on the Field Naming subtab of the Set Up Taxes page at, _Setup > Accounting > Taxes > Set Up Taxes (Administrator)_. For more information, see [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

For fields on the **Header** subtab, some fields represent **values** that are inserted and some represent **labels** of field data that;s inserted. For the value fields that are values, the defaults from the company setup page are used unless overridden on the printing fields subtab.

The available fields listed by type are as follows:

## Values {#bridgehead_N2858334}

-   Company Name
    
-   Company Phone
    
-   Company URL
    
-   Form Title
    
-   Page Number
    

## Labels {#bridgehead_N2858382}

-   Business Number
    
-   Acct. No.
    
-   Date
    
-   Doc. No.
    
-   Bill To
    
-   Ship To
    

After you've configured the printing fields, you should configure sublists. For more information, see [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html).

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
-   [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html)
-   [Configuring Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515597095.html)
-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
-   [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html)
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
