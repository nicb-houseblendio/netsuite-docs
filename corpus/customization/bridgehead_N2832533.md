---
id: "bridgehead_N2832533"
type: "bridgehead"
title: "Referencing Related Records in Formula Fields"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Fields > Advanced Features for Custom Fields > Creating Formula Fields > Referencing Related Records in Formula Fields"
parent: "section_N2832369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832533.html"
anchors: []
sha256: "f3a195a2fdbfdbaab2b06e38c8cf0b3c78dd2ef1d88b7cac91817a75209da7d8"
---

This topic describes referencing related records in formula fields. For general information about creating formula fields, see [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html).

When creating a formula field, you can reference data contained in fields on related records.

For example, you create a custom entity field to apply to customer records. You can add a formula field that references a field on the employee record of the sales rep assigned to the customer.

Note:

When referencing fields on other records, you're restricted to the records with search joins.

The format for formula field references is:

**{fieldOnAppliedRecord.fieldOnJoinedRecord}**

For example, if you wanted to display the partner email address on customer records, the format for the formula would be:

![Validation & Defaulting subtab with email formulat format entered.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/PartnerEmail_formulaFormat.png)

**partner** is the field ID for the Partner field on the customer record. **email** is the field ID for the email field on the partner record.

The following example displays the email address on the record for the partner assigned to each customer.

![Sample Customer page with partner email highlighted on the Sales subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/PartnerEmail_formulaexample.png)

Note:

Knowledge of SQL will help you to fully leverage the flexibility and power of SQL functions to define complex formulas, but you can click Set Formula next to the Formula box to add SQL functions or field IDs to your formula.

![Custom Entity Field page with Default Value and Formula highlighted on the Validation & Defaulting subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/PartnerEmailCustField.png)

Note:

For more details, refer to [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html). Also, you can refer to the [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) for tables of NetSuite field IDs.

For information about field types in formulas, see [Formulas with Various Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163612417610.html).

### Related Topics

-   [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html)
-   [Creating a Formula Field Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832724.html)
-   [Creating a Formula Field to Display Transaction Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html)
-   [Using a Field Formula to Remove Extra Spaces After Date/Time Field Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4322174650.html)
-   [Formulas with Various Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163612417610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
