---
id: "section_N2873968"
type: "section"
title: "Defining Preferred Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Defining Preferred Forms"
parent: "section_N2853340"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html"
anchors: ["procedure_N2874038"]
sha256: "050c2e44a3f245e08f7999d6d48cc1e0c658e03170e08db828efeb277518cdf8"
---

Setting preferred forms for your employees lets you control the entry and transaction forms employees use to enter data. This helps maintain consistency in your company and lets you to capture important business information.

In NetSuite, you can define form preferences in three places.

-   **On the Form:** When you create or edit a custom form, you can check the Form is Preferred box to set the current form as the default form for all users whose role form preferences **aren't** defined. On the Roles subtab, you can also define the form as preferred for specific roles.
    
-   **On the Custom Forms list page:** On the custom forms list page at Customization > Forms > \[Entry Forms or Transaction Forms\], you can check the Preferred box for any form you want to set as the default form for all users whose role form preferences **aren't** defined.
    
-   **On the Manage Roles page:** Define form preferences for specific roles at _Setup > Users/Roles > Manage Roles_ > Edit \[Role\]. In addition to setting preferred forms for a role, you can also restrict access to the preferred form.
    

For custom records, you can select a preferred form on the Forms subtab or set preferred forms for specific roles on the Permissions subtab. The preferred form you set on the Permissions subtab takes precedence over the preferred form set on the Forms subtab.

For example, you set **Custom Form A** as the preferred form on the Forms subtab. On the Permissions subtab, you set the default form for the Sales Rep role to **Custom Form B**. When a sales rep creates a new record, **Custom Form B** is selected by default.

Note:

In some cases with transactions, the form you choose is selected automatically the next time you create a transaction of that type during your current NetSuite session. For example, if you go to the Invoice Customers page, you'll see the Form list set to the form you used the last time you invoiced customers. When you begin a NetSuite session, the preferred form is selected by default on the transaction.

#### To set the preferred form for a specific role: {#procedure_N2874038}

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Click **Edit** next to the role for which you want to set form preferences.
    
    Important:
    
    You **can't** edit standard roles. To define new settings for one of these roles, click **Customize** next to the role, and enter a name for your custom role. Then set the needed custom settings and assign this custom role to the appropriate users.
    
3.  Click the **Forms** subtab.
    
4.  Click the subtab for the section you want to set preferences for.
    
    -   **Transaction** - Set defaults for cash refund, cash sale, credit memo, invoice, estimate, opportunity, purchase order, return authorization and sales order transaction forms.
        
    -   **Entity** - Set defaults for contact, customer, lead, prospect, employee, project, partner and vendor entry forms. When you define preferences for entities, you can set a preferred form for each Customer subtype in the corresponding fields at the top of the Entity subtab - Preferred Lead Form, Preferred Prospect Form and Preferred Subcustomer Form.
        
    -   **CRM** - Set defaults for phone call, campaign, case, event, solution and task entry forms.
        
    -   **Item** - Set defaults for inventory part, noninventory part, service, other charge, description, subtotal, discount, markup, group, kit, assembly and payment item entry forms.
        
5.  Set the form defaults. Note that for some roles, you **can't** modify all of these settings.
    
    -   In the **Enabled** column, for any forms you **don't** want this role to have access to, clear the boxes. This option isn't available for Customer Center roles.
        
    -   In the **Preferred** column, for any form you want to be set as the preferred form for this role, check the box.
        
    -   If you want this form to be the only form available to this role, check the box in the **Restricted** column. This option isn't available for Customer Center roles.
        
        The preferred form settings here override any settings on the Custom Forms page.
        
    
    Note the following about marking a transaction or CRM form **Preferred** for the Customer Center role:
    
    -   External forms, meaning forms with names appended with (External), can be marked preferred for the Customer Center roles, but not for other roles.
        
    -   Non-external forms can't be marked as preferred for Customer Center roles, so they aren't listed on the Forms subtab of Customer Center role records.
        
    
    Warning:
    
    If you set preferred forms **without** restrictions, your employees can still change the form they use when entering transactions or records.
    
6.  Click **Save**.
    

You can specify the entry or transaction form to use as the preferred form for a role. For more information, see [Defining Preferred Entry and Transaction Forms for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4453608888.html)

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
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
