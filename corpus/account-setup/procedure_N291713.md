---
id: "procedure_N291713"
type: "procedure"
title: "To Customize the Customer Center Role"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Customizing the Customer Center Role > To Customize the Customer Center Role"
parent: "section_N291685"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N291713.html"
anchors: []
sha256: "67ddefe6c31f265c8e23fda02f3065b7e4b1e51e29c0d850d91cc4afe92b5147"
---

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Click **Customize** next to Customer Center.
    
3.  In the **Name** field, enter a name for this new custom role.
    
    You select this name when you assign the role on customer records.
    
4.  Click the **Permissions** subtab.
    
    1.  On the **Transactions**, **Lists**, and **Setup** subtabs, click the name of the task to which you want to change access.
        
    2.  In the **Level** column, adjust the permission level for the task.
        
    3.  Click **Edit**.
        
    4.  Repeat these steps for each task you want to edit the access level for.
        
5.  Click the **Forms** subtab, and on the **Transaction** and **CRM** subtabs, check the box in the **Preferred** column next to the form you want customers to use in the Customer Center. This overrides the preferred form selected on the Transaction Forms page.
    
    The Customer Center and My Account section of your website use the transaction and entry forms marked as (External) in the Custom Forms list. Note the following:
    
    -   External forms, meaning forms with names appended with (External), can be marked Preferred for Customer Center roles, but not for other roles.
        
    -   Forms that are not external cannot be marked as Preferred for Customer Center roles, so they are not listed on the Forms tab of Customer Center role records.
        
    -   When a non-online order form is marked Preferred for Customer Center, it is saved as the form for the order. However, an online form is not saved as the form for an order, even if it is preferred; instead the preferred non-online order form is used.
        
    
    Note:
    
    To create custom forms for transactions, go to _Customization > Forms > Transaction Forms_. Custom transaction forms must use Basic printing for Customer Center roles. To create custom forms for records, go to _Customization > Forms > Entry Forms_.
    
6.  Click the **Searches** subtab.
    
    1.  To publish a custom search form or custom search results in the Customer Center, select the type of record or transaction to search.
        
        You must already have a public saved search to publish a search form or results in the Customer Center. The fields you select on the **Filters** subtab of the saved search record are used by the customer to set criteria on search forms.
        
    2.  To publish a search form, select the name of the saved search in the **Search Form** column.
        
    3.  To allow customers to view search results as a list, select the name of the saved search in the **List View** column. Searches must be marked both Public and Available as List View to be selected here.
        
        For example, a public transaction saved search marked Available as List View allows customers to view transactions matching the criteria of the search in their transaction lists.
        
    4.  To allow customers to view search results in a list on the Customer Center dashboard, select the name of the saved search in the **Dashboard View** column. Searches must be marked both Public and Available as Dashboard View to be selected here.
        
    5.  To allow customers to view search results in subtab lists, select the name of the saved search in the **Sublist View** column. Search must be marked both Public and Available as Sublist View to be selected here.
        
    6.  Check the box in the **Restricted** column to only allow customers to view the results of this search in the list view, dashboard view or sublist view, respectively.
        
        If you clear this box, customers can select this view in a View filter at the bottom of the list, and the list of all the customer's transactions or records for that page is shown by default.
        
7.  Click the **Preferences** tab to set preferences for the custom center role. The preferences set here are applied to new users assigned to a role and to existing users in a role who have not previously set that preference. See [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html).
    

### Related Topics

-   [Customizing the Customer Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291685.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
