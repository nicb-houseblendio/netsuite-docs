---
id: "bridgehead_N2853525"
type: "bridgehead"
title: "Custom Entry Form Properties"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Custom Entry Form Properties"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html"
anchors: []
sha256: "25d0b95e3d8eb7dfa1a0082800ec811d0a44f17569970d6162c63eeb863af572"
---

Note that the options available on your form vary, depending on the type of entry form being customized.

-   **Form is Preferred** - Check to make the form your default form when entering transactions of this type. You can have only one preferred form per transaction type. Checking this box clears any previously defined preferred forms of the same transaction type and replaces it with your new preferred form. For details about how preferred forms are defined, see [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html).
    
    Note the following about marking an entry or transaction form as Preferred for the Customer Center role:
    
    -   External forms, meaning forms with names appended with (External), can be marked preferred for Customer Center roles, but not for other roles.
        
    -   Non-external forms can't be marked preferred for Customer Center roles.
        
    -   When you mark a nononline order form as preferred for the Customer Center, it's saved as the form for the order. Even if an online form is marked as preferred, it's not saved as the form for an order. The preferred nononline order form is used instead.
        
    
    Employee Center roles have limited access to forms. Only one form is ever made available to this role, and the form set on the Role record takes precedence over the preferred form.
    
-   **Store Form with Record** - Check to store this custom form with each record created using this form. When viewed or edited, any record that was entered with this form is displayed using this form rather than your preferred form.
    
    -   For custom entry forms, the Store Form with Record box is cleared by default.
        
    -   The Store Form with Record box is available only for a subset of transaction forms. For this subset, the box is checked by default. This box isn't available for other transaction forms because custom forms are stored with records automatically. For more information, see [Storing Custom Forms with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2854025.html).
        
    
    Important:
    
    If a custom form is stored with a record, users who access that record will see the custom form, even if it's not enabled for their role.
    
-   **Print Template** - This field is available only when the Advanced PDF/HTML Templates feature is enabled, and the **Printing Type** is set to **Advanced**. Select a template to be used when transactions associated with this form are printed.
    
-   **Enable Field Editing on Lists** - Check to permit inline editing on this form. Inline editing lets users edit fields on this form from within the record view. When enabled, fields that can be edited from within the record view display the inline editing icon. This option also provides a New menu that lists options to create new related records.
    
-   **Use for Pop-ups** - Check to use this form in popup windows when you add a record of this type from another record. This capability is available only for entity forms, item forms, and custom record forms. For each type of form, only one form can be set as the popup form. Checking this box clears any previously defined popup forms of the same transaction type and replaces it with your new popup form.
    
    Note:
    
    The Use for Pop-ups box is automatically checked for the custom form of a custom record, no other form is already enabled.
    
-   **Popup Only** - When **Use for Pop-ups** is checked, you can check **Popup Only** to use this form only when adding a record of this type from another record. You can't change the form in the popup window if it's a standard popup form.
    

### Related Topics

-   [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html)
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
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
