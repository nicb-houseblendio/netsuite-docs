---
id: "section_N405092"
type: "section"
title: "Support Cases Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Support Import Type > Support Cases Import"
parent: "section_N404668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405092.html"
anchors: ["bridgehead_N405248"]
sha256: "26b11fa3b642464195728129cb124a4eaab71d196e25eabeca40d1914c40a38e"
---

A support case, also known as a case, is a record of a customer-reported question, issue, or suggestion, and subsequent actions taken.

The support case data that you can import depend on the fields available on either your preferred Case form, or the custom case form selected on the Import Assistant Import Options page. For details about specifying a custom form, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).

For details about fields that can be mapped in the support case record, see the SOAP Schema Browser's [support case](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/supportcase.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Be aware of the following:

-   Required case fields for import are: Company, Subject, Status, and Incident Date.
    
-   The Incident Date field includes both a date and a time. You need to exercise care when you format values for this field in your CSV files. To avoid errors, review and follow the guidelines in [Setting Incident Date Field Values for Cases](#bridgehead_N405248).
    
-   Imports can't send case-related email.
    
-   Escalations and Solutions sublist data can be imported. Escalation records are selectively updatable based on Escalatee key field.
    
-   If you're doing a cases import for the addition of new cases, select the **Add** data handling option, rather than **Add or Update**.
    
-   If you need to use an import to update existing case records, you must map either the Internal ID or External ID field to uniquely identify records. This requirement is enforced when you select the **Update** data handling option and when you select the **Add or Update** data handling option.
    

## Setting Incident Date Field Values for Cases {#bridgehead_N405248}

The Incident Date mapped field for CSV import represents both the date and the time when a case is reported, as shown in the fields labeled **Incident Date** and **Incident Time** on the standard Case form.

Note the following guidelines when you enter values for Incident Date fields in CSV files used for case imports:

-   Provide both a date and a time, for example: **04/12/2010 09:00 AM**.
    
-   Specify values according to the NetSuite Date Format and Time Format set at _Home > Set Preferences_ for the user doing the import. The following are example formats:
    
    -   Date Format is **MM/DD/YYYY**.
        
    -   Time Format is **hh:mm AM/PM**.
        
    -   A space should be included between the date and time, for example: **04/12/2010 10:00 AM**.
        

Note:

If a date is provided without a time value, **12:00 AM** will be assumed by default.

-   To avoid Excel formatting errors for Incident Date values, you should right-click the column and choose Format Cells to explicitly select a format that matches the Date Format (and if applicable, Time Format) set up in NetSuite.
    
    ![Format Cells window.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TaskDateFormats.png)

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Working With Cases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2434254.html)

### Related Topics

-   [Support Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404668.html)
-   [Issues Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404746.html)
-   [Solutions Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N404868.html)
-   [Topics Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405456.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
