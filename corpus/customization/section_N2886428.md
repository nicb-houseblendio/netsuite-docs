---
id: "section_N2886428"
type: "section"
title: "Sourcing with Custom Records"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Sourcing with Custom Records"
parent: "chapter_N2875173"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886428.html"
anchors: ["procedure_N2886455"]
sha256: "f07e30fe84f47d7d0a1b3e8d2fb292be54ca69eeb50c51d89f8b3bf1d684bca6"
---

You can use sourcing on custom record types to populate fields with information from both standard and custom records. You must first create a List/Record field on your custom record type for the kind of record you want to source information from. After creating the List/Record field, you can select that field in the Source List field.

For example, let's say you've created an Intern custom record type. You want to include information for your intern records about the employees supervising each intern. You can do this by first creating an Employee field with a list of your employees. Then you can source information from employee records to other fields on your intern records.

For information about sourcing and custom fields, see [Setting Sourcing Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2839623.html).

#### To use sourcing with custom record types: {#procedure_N2886455}

1.  Go to _Customization > Lists, Records & Fields > Record Types_.
    
2.  In the **Edit** column, click the name of the record type you want to create a sourced field for.
    
3.  Click the **Fields** subtab.
    
4.  Click **New Field**.
    
5.  In the **Label** field, enter the name of your new field.
    
    For example, to create a field that lists your employees, you'd enter **Employee**.
    
6.  In the **Type** field, select **List/Record**.
    
7.  In the **List/Record** field, select the kind of record you want to include information from in other fields on your record type.
    
    For example, to include information about your employees you'd select **Employee**.
    
8.  Click **Save**.
    
    Now, you can create your sourced fields.
    
9.  Click the **Fields** subtab.
    
10.  Click **New Field**.
     
11.  In the **Label** field, enter a description for your field.
     
     For example, if you wanted to include an employee's email address you would enter **Employee Email**.
     
12.  In the **Type** field, select a type of custom field.
     
     The type you select must match the type of field you want to source from.
     
     For example, if you wanted to include an email address you would select **Email Address** in the **Type** field.
     
     For a list of standard fields and their types, see [Available Standard Fields and Field Types for Custom Record Types and Source Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2886648.html).
     
13.  If you're creating a List/Record field, select the appropriate list or record in the **List/Record** field.
     
     For example, if you're sourcing from the **Sales Rep** field on Customer records, select **Employee** in the **List/Record** field because your sales reps are employees.
     
14.  Click the **Sourcing & Filtering** subtab.
     
15.  In the **Source List** field, select the record type you want to source information from.
     
     This field lists the field you created earlier.
     
     You can create multiple source lists for your custom records. To do so, repeat Steps 1-9 for each kind of record you want to be able to source information from.
     
16.  In the **Source From** field, select the field you want to include information from. If you click to view the list, sourcing and filtering options are available.
     
     You must select a **Source List** before you can select a field.
     
     The selected field's type must match the type selected in the **Type** field.
     
17.  When you have finished, click **Save**.
     
18.  To add **Source List** fields, repeat Steps 1-9.
     
     To add sourced fields, repeat Steps 10-17.
     

You can now source information from standard and custom fields and records on your custom record types. For more information about available standard fields and field types, see [Available Standard Fields and Field Types for Custom Record Types and Source Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2886648.html)

### Related Topics

-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
-   [Parent-Child Record Relationships](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885788.html)
-   [Updating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860753.html)
-   [Using Custom Record Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2888872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
