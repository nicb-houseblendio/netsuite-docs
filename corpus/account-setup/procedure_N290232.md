---
id: "procedure_N290232"
type: "procedure"
title: "To Set a Default Form for Roles"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Setting Default Forms for Roles > To Set a Default Form for Roles"
parent: "section_N290202"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N290232.html"
anchors: []
sha256: "ca7caf218598a9ddc50e7320da4b00a5ae95b79a60abe850f005c65f0f0d87f8"
---

1.  Go to _Setup > Users/Roles > Manage Roles_.
    
2.  Click **Customize** next to the role you want to set a form for.
    
3.  Enter a name for your custom role.
    
4.  Click the **Forms** subtab.
    
5.  Click the section you want to set default forms for.
    
    -   **Transaction** - Set default forms for transactions such as cash refunds, cash sales, invoices, and sales orders.
        
    -   **Entity** - Set default forms for the records you keep for people and companies in NetSuite, such as employees and customers.
        
    -   **CRM** - Set default forms for CRM-related activities and records such as campaigns, cases, events, and tasks
        
    -   **Time -** Set default forms for time entries.
        
    -   **Item** - Set default forms for item records.
        
    -   **Other Record** - Set default forms for other types of records, such as competitor records.
        
6.  In the **Enabled** column, clear any boxes for forms this role should not have access to. (not available for Customer Center roles)
    
    If you disable all forms for a record or transaction type, users with this role will use the standard form.
    
7.  Check the box in the **Preferred** column next to any form that should be the default for this role.
    
    Note:
    
    Be aware of the following about marking a transaction or CRM form Preferred for Customer Center roles: External forms, meaning forms with names appended with (External), can be marked Preferred for Customer Center roles, but not for other roles. Forms that are not external cannot be marked as Preferred for Customer Center roles, so they are not listed on the Forms tab of Customer Center role records.
    
8.  To have this form to be the only form available to this role, check the box in the **Restricted** column.
    
9.  Click **Save**.
    

If you set default forms and do not make the defaults restricted, your users can still change the form they use when they are entering transactions or records.

After you have set default forms, you need to assign your customized roles to your employees. You can assign roles on the Access subtab of employee records.

### Related Topics

-   [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html)
-   [Setting Default Forms for Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N290202.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
