---
id: "bridgehead_N2853604"
type: "bridgehead"
title: "Custom Transaction Forms Properties"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Custom Transaction Forms Properties"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html"
anchors: []
sha256: "b4ec854d857a8cae28b861d392b22f891d41aec35032fc520415db271416bf3b"
---

Note that the options available on your form vary, depending on the type of transaction form being customized.

-   **Form is Preferred** - Check to make the form your default form when entering transactions of this type. Only one form can be defined as the preferred form per transaction type. Checking this box clears any previously defined preferred forms of the same transaction type and replaces it with your new preferred form. For details about how preferred forms are defined, see [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html).
    
    When marking an entry or transaction form as Preferred for the Customer Center role, keep the following in mind:
    
    -   External forms, meaning forms with names appended with (External), can be marked preferred for Customer Center roles, but not for other roles.
        
    -   Non-external forms can't be marked preferred for Customer Center roles.
        
    -   When a nononline order form is marked as preferred for the Customer Center, it's saved as the form for the order. Even if an online form is marked as preferred, it's not saved as the form for an order. The preferred nononline order form is used instead.
        
    
    Employee Center roles have limited access to forms. Only one form is ever made available to this role, and the form set on the Role record takes precedence over the preferred form.
    
-   **Store Form with Record** - Check to store this custom form with each record created using this form. When viewed or edited, any record that was entered with this form is displayed using this form rather than your preferred form.
    
    -   For custom entry forms, the Store Form with Record box is cleared by default.
        
    -   The Store Form with Record box is available only for a subset of transaction forms. For this subset, the box is checked by default. This box isn't available for other transaction forms because custom forms are automatically stored with records. For more information, see [Storing Custom Forms with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2854025.html).
        
    
    Important:
    
    If a custom form is stored with a record, users who access that record will see the custom form, even if it's not enabled for their role.
    
-   **Print Template** - This field is available only when the Advanced PDF/HTML Templates feature is enabled, and the **Printing Type** is set to **Advanced**. Select a template to be used when transactions associated with this form are printed.
    
-   **Allow Add Multiples** - Check to permit the **Add Multiple** button to appear on transaction item lists. You should clear the box on any forms that rely on custom code line item validation scripts. The **Add Multiple** button is displayed on Items lists and lets you add multiple items at a time to the item list. However, when items are added with the **Add Multiple** button, any Validate Line custom code events defined for the form **aren't** triggered.
    
-   **Printing Type** - This field is available only when the Advanced PDF/HTML Templates feature is enabled. The Advanced option that's selected by default enables your custom form to use an advanced PDF/HTML template. For more details, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html). Select **Basic** to enable your custom form to use transaction form PDF layouts and HTML layouts.
    
-   **Email Template** - (Available only when the Advanced PDF/HTML Templates feature is enabled, and the **Printing Type** is set to **Advanced**.) Select a template to use for email attachments when transactions associated with this form are sent by email.
    
-   **Email Message Template** - (Available only for transactions that support custom email templates.) Select which template to use for the message body for this transaction type when NetSuite sends email messages with a PDF attachment. If you select Default Email Template, NetSuite will send transaction email messages using a hard-coded template and body message that you can set up at _Setup > Company > Email > Email Preferences (Administrator)_. For more information, see [Assigning an Email Template to a Transaction Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html#subsect_156145127684).
    
-   **PDF Layouts** - Select a PDF layout for your form.
    
-   **HTML Layouts** - Select an HTML layout for your form. Standard and Classic layouts exist for all the standard form types other than shipping labels.
    
-   **Remittance Slip** - Specify which remittance slip is used on invoices, statements, return authorizations, and packing slips. To prevent the current transaction from printing with a remittance slip, select **None**.
    
    Note:
    
    To use this feature, set the Print Remittance Form with Invoices & Statements feature. For more information, see [Printing Remittance Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1234980.html).
    
-   **Disclaimer** - Enter a disclaimer message to appear at the bottom of your form. The message can be up to 4,000 characters long, including spaces.
    
-   **Address** - Enter an address to be used only on this form. If you don't enter an address, the default address entered at _Setup > Company > Company Information_ is used.
    
-   **Logo** - Select a logo to be used only on this form. You must first upload the image to your File Cabinet at Documents > Files > Images. If you don't select a logo, the default logo selected at _Setup > Company > Company Information_ is used.
    
    When basic printing is used, logos don't appear on these forms: picking ticket, bill of materials, shipping label, opportunity, item fulfillment, item receipt, store pickup fulfillment, and custom transactions.
    
-   **Columns Width** - This is the total width of all the columns on your form. If the total width of your columns is greater than the available column space, NetSuite adjusts the width proportions to fit on the page.
    
-   **Layout Space** - This number is the maximum number of inches of printable space permitted on your form. The measurement is determined by the Page Width of the layout you choose. You can change the page width by creating a custom layout.
    

### Related Topics

-   [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html)
-   [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html)
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
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)
-   [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html)
-   [Transaction Form HTML Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873464.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
