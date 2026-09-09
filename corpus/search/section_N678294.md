---
id: "section_N678294"
type: "section"
title: "Defining Audiences for Saved Searches"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Saved Searches > Defining a Saved Search > Defining Audiences for Saved Searches"
parent: "section_N676039"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678294.html"
anchors: ["procedure_40144716646"]
sha256: "35e1a78b176fa62ba68ccade2973bd57928481baf2e76c79585928ccfd4a69c2"
---

If you're an administrator or have at least the Create level of the Publish Search permission, you can use the **Audience** subtab to choose who can run the search and see the results. You can also make the search public for all users by checking the **Public** box. For information, see [Making Saved Searches Public](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N678471.html).

Only selected audience members and account administrators see the saved search on search lists. Setting an audience also limits its appearance in other lists, sublists, portlets, and forms. Set these preferences on the **Roles** subtab. By default only administrators and the owner can edit the search. Audience members can't edit it unless you check the **Allow Audience to Edit** box.

Customers, vendors, and most partners can't access saved searches, even public ones. If they do get access, they can run it only if they have permission to that record type, and they can see only their own records.

Important:

If your saved search has sensitive data, don't make it public. Use the fields on the **Audience** subtab to limit the audience.

#### To define an audience for a saved search: {#procedure_40144716646}

1.  When defining or editing a saved search, click the **Audience** subtab.
    
2.  If you want to allow the audience to edit the search, check the **Allow Audience to Edit** box.
    
    -   If you enable this, the audience can change and save the search with the same name.
        
    -   If not, they can make changes but need to save the search with a different name using 'save as'.
        
3.  In the fields provided, choose an audience for your search results. You can select options from any or all of the following audience types.
    
    For each of the audience type, you can select multiple options by holding down the Ctrl key.
    
    -   **Roles** - You can select internal and external roles as follows:
        
        Note:
        
        If the **Public** box is checked, the **Internal Roles** and **External Roles** fields are dimmed, the search is available to all roles and the selection cannot be edited. To select specific internal and external roles, clear the **Public** box first. For more information, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
        
        -   **Internal Roles** - In this field, do one of the following:
            
            -   Check the **Select All** box to make the search available to all internal roles.
                
            -   Clear the **Select All** box and select the internal roles you want.
                
        -   **External Roles** - To make the search available to specific external roles, select them from the list.
            
        
        Note:
        
        If your account has many roles, they may not be in a dropdown list. Increase the number set for Maximum Entries in Dropdowns at _Home > Set Preferences_, on the **General** subtab.
        
    -   **Departments** - Select one or more departments.
        
    -   **Subsidiaries (If Available)** - Select one or more subsidiaries.
        
    -   **Groups** - Select one or more groups.
        
    -   **Employees** - Select one or more employees.
        
        To make the search available to all employees, check the **Select All** box.
        
    -   **Partners** - Select one or more partners.
        
        To share with all partners, check the **Select All** box.
        

Important:

If you choose both role and department options, users must belong to both to access the search. If you choose any other combination, users needs to match only one type of option.

### Related Topics

-   [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html)
-   [Selecting Available Filters for Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678025.html)
-   [Highlighting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N678573.html)
-   [Marking a Search Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4098463669.html)
-   [Editing or Deleting a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679137.html)
-   [Using a Saved Search as a View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679407.html)
-   [Defining a Saved Search as Preferred Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N679861.html)
-   [Defining a Saved Search as a Preferred Search Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680007.html)
-   [Using a Saved Search as a Reminder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N680807.html)
-   [Using Saved Searches for Customer Center Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3842991795.html)
-   [Change of Sign for Expense Account Amounts in Transaction Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3891485192.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
