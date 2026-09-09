---
id: "bridgehead_N2832724"
type: "bridgehead"
title: "Creating a Formula Field Example"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Creating Formula Fields > Creating a Formula Field Example"
parent: "section_N2832369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832724.html"
anchors: []
sha256: "245a1b19848fe031c9bf274a9e2498d86721492e4840b4cce3b560a051c69bbc"
---

This topic provides an example of creating a formula field. For general information about creating formula fields, see [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html).

Suppose, for example, you want to display the remaining credit available to a customer on the customer record. Create a custom entity field of the type Currency called **Remaining Credit**. Apply the field to the Customer record and set it to display on the Financial subtab. Define the field with the following formula in the Validation & Defaulting subtab:

`{creditlimit}-nvl({balance},0)`

(where `creditlimit` and `balance` are standard customer fields and the `nvl NULL` handling function forces the value to be set to the second parameter when the field is NULL)

Make sure that you enable the Formula field and clear the Store Value box to ensure that the value is always dynamically recalculated as a formula.

When a customer record is viewed, the Remaining Credit field returns a calculated value based on the credit limit and customer balance fields.

For an additional detailed example of creating a formula field, see Example of Creating a Formula Field (SuiteAnswers ID 1014946).

### Related Topics

-   [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html)
-   [Referencing Related Records in Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832533.html)
-   [Creating a Formula Field to Display Transaction Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html)
-   [Using a Field Formula to Remove Extra Spaces After Date/Time Field Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322174650.html)
-   [Formulas with Various Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163612417610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
