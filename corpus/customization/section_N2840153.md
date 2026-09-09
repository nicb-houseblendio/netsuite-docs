---
id: "section_N2840153"
type: "section"
title: "Setting Filtering Criteria"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Creating a Custom Field > Setting Filtering Criteria"
parent: "section_N2829580"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840153.html"
anchors: ["procedure_N2840184", "kaltura_player_272"]
sha256: "cb00dedf8efe8009f25c582472a5282045d67624ce6103de19282e4a6fa060b9"
---

When creating a list/record or multiple select custom field, you can filter the choices available in that field on records and transactions based on selections made in other fields. Filtering enables you to tailor the exact choices offered to users entering records and transactions.

You can filter based on the selections in multiple list fields. For more information, see [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html).

Note:

Filtering applies only to lists of records. It doesn't apply to custom lists.

#### To filter a list/record or multiple select custom field: {#procedure_N2840184}

1.  Click the **Sourcing & Filtering** subtab.
    
2.  In the **Filter Using** field, select a field to filter on.
    
    The field you select here is a field on the record you selected in the **List/Record** field.
    
    The selected field limits the results based on your filter criteria. For instance, to show only sales representatives in an employee list, you'd select the **Sales Rep** field in the Filter Using column. Sales Rep is the field on the employee record being filtered.
    
    Note:
    
    If you specify two or more filters, the custom field uses a popup list instead of a dropdown list.
    
3.  If the field selected in the **Filter Using** column is a check box, check the **Is Checked** box to show only records with that box checked.
    
    In the sales representative example, check the **Is Checked** column.
    
4.  In the **Compare Type** column, select how you want to compare the information to your filter criteria.
    
    For example, select **equal** to ensure that the information you set as criteria matches the selections available in the list exactly.
    
5.  In the **Compare Value to** column, enter the value you want to filter the list by.
    
    For example, if you select **State** in the **Filter Using** field, enter **GA** to filter the list to records only with the state listed as Georgia.
    
6.  If the field selected in the **Filter Using** field is a list, select the value to show in the **Value Is** column.
    
7.  To include all records with a value entered in your filter field, check the **Is Not Empty** box.
    
    The Is Not Empty option isn't available for check box fields.
    
8.  To include all records with no value entered in your filter field, check the **Is Empty** box.
    
9.  In the **Compare To Field** column, select which field on the record selected in the **List/Record** field you want to compare to the field in the **Filter Using** column.
    
10.  Click **Add/Edit**.
     
11.  Add all necessary filters to the custom field.
     
     The more filters you add, the fewer options will be available in the field. To be included, each selection must match each filter.
     
12.  Click **Save**.
     

Watch the following help video for information about setting sourcing and filtering criteria for a custom field.

<a id="kaltura_player_272"></a>

Next, you can set up access to your custom field. For more information, see [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html).

Warning:

Custom field filters are type sensitive. If you change the type of a custom field, filters defined for the field can become incompatible. This incompatibility results in unexpected errors when a form containing the field is displayed. Before changing a custom field's type, review it's existing filters and remove or change these filters to avoid errors. For information about various custom field types, see [Field Type Descriptions for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842731.html).

### Related Topics

-   [Creating a Custom Field](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2829580.html)
-   [Creating Custom Fields by Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161732113352.html)
-   [Assigning Custom Fields to Specific Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830027.html)
-   [Behavior of View from Order Only Settings on Transaction Line and Transaction Body Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0528113109.html)
-   [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html)
-   [Setting Validation and Defaulting Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830711.html)
-   [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html)
-   [Sourcing and Filtering Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839994.html)
-   [Dependent Dropdown Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2840468.html)
-   [Restricting Access to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2841053.html)
-   [Restricting Access to Employee Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1514478336.html)
-   [Creating Read-Only Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2842596.html)
-   [Adding Translations for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4308565496.html)
-   [Adding Custom Fields to Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828541.html)
-   [Tracking Changes to Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_54095541974.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
