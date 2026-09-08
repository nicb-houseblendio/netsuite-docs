---
id: "section_N262248"
type: "section"
title: "Creating Departments"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Departments and Classes Overview > Creating Departments"
parent: "section_N261602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262248.html"
anchors: ["procedure_N262280"]
sha256: "282fb171a3bbc005b4893d7f8402b372ffb1559145045dd5159a8b13905a2cbc"
---

Departments are categories you can create to separate and track records such as financials, transactions, and employees. For example, you can create a department for each team dedicated to a business area, and then track their income and expenses over any time period.

To enable Departments, go to _Setup > Company > Enable Features_. On the Company subtab, check the Departments box and then click Save.

#### To create a department record: {#procedure_N262280}

1.  Go to _Setup > Company > Departments > New_.
    
2.  Enter a name for the department, up to 60 letters and numbers.
    
3.  If the department is a subdepartment, in the **Subdepartment of** field, select the parent department.
    
4.  If you use NetSuite OneWorld, in the **Subsidiary** field, select one or more subsidiaries.
    
    To select multiple subsidiaries, hold down the Ctrl key and click each subsidiary.
    
    You need to associate a subsidiary to a department to use it on a transaction or record related to that subsidiary.
    
5.  If you use NetSuite OneWorld, check the **Include Children** box to associate the department with all the child subsidiaries of each subsidiary selected in the **Subsidiary** field.
    
6.  Check the **Department is Inactive** box to make this department inactivate.
    
    Inactive departments don't appear in department lists on records and transactions.
    
    Note:
    
    To inactivate departments from the Departments list, go to _Setup > Company > Departments_, check the **Show Inactives** box, check the boxes in the **Inactive** column, and then click **Submit**.
    
7.  Click **Save**.
    

You can restrict access to transaction, employee, partner, and optionally item records based on their department values. You can also limit which departments users can assign to these records. You can set department restrictions per user role and applied then to everyone using that role. For more information, see [Restricting Access to Records by Department](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262535.html).

You also can apply department restrictions to custom records if the custom record type has a Department field. You can add this field to a custom record from the Department record by clicking New Field. For more information, see [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).

### Related Topics

-   [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html)
-   [Creating Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261769.html)
-   [Modifying and Deleting Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176293394.html)
-   [Restricting Access to Records by Class](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262059.html)
-   [Modifying and Deleting Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176372145.html)
-   [Restricting Access to Records by Department](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262535.html)
-   [Converting Classes to Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262723.html)
-   [Converting Classes to Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262871.html)
-   [Custom Segments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4732448748.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
