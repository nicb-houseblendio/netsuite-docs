---
id: "section_N261769"
type: "section"
title: "Creating Classes"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Departments and Classes Overview > Creating Classes"
parent: "section_N261602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261769.html"
anchors: ["procedure_N261801"]
sha256: "8c832c2fdfaba58ba2afaa8c04748d6e2665cd6efaee524be7b6f6b5261ca587"
---

Classes are categories you can create to track records such as financials, transactions, and employees. For example, you own a janitorial service and want to track income and expenses separately for household and commercial accounts. You set up a class for each account type and track the financial performance of each class over any time period.

To enable classes, go to _Setup > Company > Enable Features_. On the Company subtab, check the Classes box and then click Save.

#### To create a class record: {#procedure_N261801}

1.  Go to _Setup > Company > Classes > New_.
    
2.  Enter a name for the class, up to 60 letters and numbers.
    
3.  If this class is a subclass of another, in the **Subclass of** field, select the parent class.
    
4.  If you use NetSuite OneWorld, in the **Subsidiary** field, select one or multiple subsidiaries.
    
    To select multiple subsidiaries, hold down the Ctrl key and click each subsidiary.
    
    You need to associate a subsidiary with a class to use it on any transaction or record related to that subsidiary.
    
5.  If you use NetSuite OneWorld, check the **Include Children** box to associate the class with all the child subsidiaries of each subsidiary selected in the **Subsidiary** field.
    
6.  Check the **Class is Inactive** box to make this class inactivate.
    
    Inactive classes don't appear in lists of classes on records and transactions.
    
    Note:
    
    To inactivate classes from the Classes list, go to _Setup > Company > Classes_, check the **Show Inactives** box, check one or more boxes in the **Inactive** column, and then click **Submit**.
    
7.  Click **Save**.
    

You can restrict access to transaction, employee, partner, and optionally item records based on their class values. Also, you can limit which classes users can assign to these records. You can set class restrictions by user role and then apply them to everyone with that role. For more information, see [Restricting Access to Records by Class](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262059.html).

You also can apply class restrictions to custom records if the custom record type has a Class field. You can add this field from the Class record by clicking New Field. For more information, see [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).

### Related Topics

-   [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html)
-   [Modifying and Deleting Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176293394.html)
-   [Restricting Access to Records by Class](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262059.html)
-   [Creating Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262248.html)
-   [Modifying and Deleting Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176372145.html)
-   [Restricting Access to Records by Department](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262535.html)
-   [Converting Classes to Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262723.html)
-   [Converting Classes to Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262871.html)
-   [Custom Segments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4732448748.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
