---
id: "section_N2860797"
type: "section"
title: "Associating Custom Code (Client SuiteScript) Files With Custom Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Associating Custom Code (Client SuiteScript) Files With Custom Forms"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html"
anchors: ["bridgehead_4583409706", "procedure_N2860837"]
sha256: "5ee53b353d2755cd08317e5ed378b4cc9cc04d28e8666933f48abb8162cee2ac"
---

If the Client SuiteScript feature is enabled, the Custom Code subtab is available on custom entry and transaction forms. On this subtab, you can define existing client SuiteScript files to be used with the form. When the script's executing function is called, the actions defined within the script (and any built-in NetSuite actions for that form type) are performed.

You can also add a custom button to the form to call the client script. For more information, see [Working with Custom Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2857802.html).

To associate client SuiteScript files with a form, click the plus sign to the right of the Script File field, and add a new script file.

## Permission for Attaching Scripts to Custom Entry and Transaction Forms {#bridgehead_4583409706}

Users who have the Custom Entry Forms or Custom Transaction Forms permission, but who don't have the SuiteScript permission, can't access the Custom Code subtab of custom forms.

Users must have at least the Edit level of the SuiteScript permission to attach a script to a custom form on the Custom Code subtab. For users with the Edit or Full level of the SuiteScript permission, the Custom Code subtab is displayed and is fully editable. Users with the View or Create level of the SuiteScript permission can see the Custom Code subtab but can't edit it. Users who don't have SuiteScript permission can't view the Custom Code subtab.

#### To associate client SuiteScript files with a form: {#procedure_N2860837}

1.  Go to the Custom Code subtab of the form record.
    
2.  In the **Script File** field, select the client SuiteScript file that contains the scripts you want to add to this form. To add a new script file, click the New icon on the right side of the **Script File** field.
    
    **Note:** Client scripts or scripts needed on the client side, such as library files, can't have the **Hide in SuiteBundle** preference enabled.
    
3.  In one or more of the client event type fields, enter the names of the functions you want to perform. When entering function names, don't include parentheses or arguments. For example, type **sampleFunction** for a function that appears as sampleFunction(param1, param2) in your SuiteScript file.
    
    -   **Page Init Function** - Executing function to be called when this form is first loaded.
        
    -   **Save Record Function** - Executing function to be called when this record is saved.
        
    -   **Validate Field Function** - Executing function to be called when a field on this entry form is changed.
        
    -   **Field Changed Function**\- Executing function to be called when a change made to a field is accepted.
        
    -   **Post Sourcing Function** - Function that runs on Post Sourcing events. These events occur following a field change after all the field's child field values are sourced from the server. This enables fieldChange style functionality to occur after all dependent field values have been set.
        
    -   **Line Init Function** - Function that runs on Line Init events. These events occur when an existing line is selected.
        
    -   **Validate Line Function** - Function that runs on Validate Line events. These events occurs prior to a line being added to a sublist (inlineeditor or editor sublists only). It can be thought of as the saveRecord equivalent for sublist line items.
        
    -   **Validate Insert Function** - Function that runs on Validate Insert events. These events occur when you insert a line into an edit sublist. The UI equivalent of this event is when a user selects an existing line in a sublist and then clicks the Insert button. Note that returning false on a validateInsert blocks the insert.
        
    -   **Validate Delete Function**\- Function that runs on Validate Delete events. These events occur when you try to remove an existing line from an edit sublist. Returning false blocks the removal.
        
    -   **Recalc Function** - Script name to be called from the attached script file. This script is called when a line item is added. For example, after entering the information you add an item to a transaction.
        
4.  If your client SuiteScript file references any functions in a library file, add the library files in the **Library Script File** list.
    
5.  Click **Save**.
    

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
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
