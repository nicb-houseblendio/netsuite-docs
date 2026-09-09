---
id: "bridgehead_N2832808"
type: "bridgehead"
title: "Creating a Formula Field to Display Transaction Line Numbers"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Creating Formula Fields > Creating a Formula Field to Display Transaction Line Numbers"
parent: "section_N2832369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html"
anchors: []
sha256: "979910962e09919635d19bb62cadf332308529470a4cda10afb9e548de29363a"
---

This topic describes how to create a formula field to display transaction line numbers. For general information about creating formula fields, see [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html).

You can display line numbers on the Items subtab of transactions when they're viewed online and in printed transactions. To do so, create a custom field that uses the `{linenumber}` formula, and apply the field to transaction forms.

#### To create a custom field that uses the {linenumber} formula:

1.  To create a custom line number field, go to _Customization > Lists, Records, & Fields > Transaction Column Fields > New_.
    
2.  Enter a label for the field, select a **Type** of **Integer Number**, and clear the **Store Value** box.
    
3.  On the **Applies to** subtab, check boxes for the transactions that should display line numbers, and check the **Print on Standard Forms** box.
    
4.  On the **Display** subtab, select a **Display Type** of **Disabled**.
    
5.  On the **Validation & Defaulting** subtab, check the **Formula** box, and enter `{linenumber}` as the **Default Value**.
    
6.  Save the new field.
    
7.  To enable the line number field to be printed on a custom transaction form, edit the form. On the **Printing Fields**, **Columns** subtab, check the **Print/Email** box for the new field.
    

Note the following:

-   Line numbers display when a transaction record is in View mode. In Edit mode, line number value is shown as 1.
    
-   Line numbers correspond to the printed or viewed results, meaning they're contiguous even when transaction lines are omitted.
    
-   If you're using a line number formula field for viewed and printed transactions, and you also want to include the line number in search results, set up the search as follows. This setup ensures that search results match viewed and printed transaction items:
    
    -   Set a criteria of **Main Line = No (false)**.
        
    -   Filter out transaction line items related to taxes.
        
    -   Add the **Item** field as a results field.
        
    -   Add the **Amount (Gross)** field as a results field; don't use the **Amount** field.
        
    -   Add a **Formula(Numeric)** field as a results field, with the following formula expression: `RANK() OVER (PARTITION by {internalid} ORDER BY {linesequencenumber})`.
        

### Related Topics

-   [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html)
-   [Referencing Related Records in Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832533.html)
-   [Creating a Formula Field Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832724.html)
-   [Using a Field Formula to Remove Extra Spaces After Date/Time Field Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322174650.html)
-   [Formulas with Various Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163612417610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
