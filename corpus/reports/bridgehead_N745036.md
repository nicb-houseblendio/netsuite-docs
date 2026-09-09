---
id: "bridgehead_N745036"
type: "bridgehead"
title: "Defining a Report Audience"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Sharing Custom Reports with Other Users > Defining a Report Audience"
parent: "section_N745002"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N745036.html"
anchors: ["procedure_N745044"]
sha256: "e5cd7336a433c00af8ecdb3d1fd499dc6efbf40cb2837693a80caa0288657fdb"
---

To help people find your report, define an audience for it.

#### To define an audience for your report: {#procedure_N745044}

1.  Click **Customize** in the footer of the report you want to share.
    
2.  On the Report Builder (or Financial Report Builder) page, click **More Options**.
    
3.  In the **Audience** fields, choose an audience for your report:
    
    You can select options from any or all of the following audience types. For each audience type below,you can select multiple options by holding down the Ctrl key.
    
    -   **Roles**: You can select internal and external roles as follows.
        
        -   **Internal Roles** : In the Internal Roles field, do one of the following:
            
            -   To make the custom report available to all internal roles, check the **Select All** box next to Internal Roles.
                
            -   To make the custom report available to specific internal roles, clear the **Select All** box and then select the internal roles from the list.
                
        -   **External Roles**: To make the custom report available to specific external roles, select them from the list.
            
    -   **Departments**: If you've selected any roles, you can also select departments to share your report with.
        
    -   **Subsidiaries**: Select the subsidiaries you want to share this report with.
        
    -   **Groups**: Select a group to share your report with.
        
    -   **Employees**: Select one or more employees to share your report with. To share with all employees, check the **All Employees** box.
        
    -   **Partners**: Select one or more partners to share your report with. To share with all partners, check the **All Partners** box.
        
4.  Click **Save**.
    

Important:

If you select both a role and a department, users need that role and must be in the department to access the report. If you select a group, employee, or partner, the user has to be in that group or be the selected employee or partner. The relationship between Audience groups can be defined as:

Audience = (Role AND Department) OR Group OR Employee OR Partner

You can select roles without selecting departments. However, if you want to select departments, you need to select at least one role.

### Related Topics

-   [Sharing Custom Reports with Other Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N745002.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
