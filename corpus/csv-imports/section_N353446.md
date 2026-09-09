---
id: "section_N353446"
type: "section"
title: "CSV Import Error Reporting"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Five Save Mapping & Start Import > CSV Import Error Reporting"
parent: "section_N350233"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html"
anchors: ["bridgehead_N353458", "bridgehead_3705035943", "bridgehead_4601081189", "bridgehead_N353514", "bridgehead_N353550", "bridgehead_1518422758", "bridgehead_1534159345", "bridgehead_N353565"]
sha256: "f2fa57e0135b635c44dc506e5be0bd5b3682c74ac915020dee2d4d2e4b829dde"
---

The CSV Import Assistant provides robust error handling throughout all stages of the import process.

Some basic validation is performed on the fields before the import is performed. For example, if a number is expected and a string is encountered, an error appears.

## Invalid Character Errors {#bridgehead_N353458}

If a file can't be processed due to invalid characters, you receive an error message. The error message describes the type of error and provides the row number, column name, and value that caused the error.

## Incorrect Character Encoding {#bridgehead_3705035943}

In many cases, an invalid character error occurs because the incorrect character encoding has been chosen. You can either:

-   Return to the Scan & Upload CSV File step, change the character encoding option, and click next to scan the files again, or
    
-   Close the Import Assistant, correct the source files, and then upload again.
    

For information about supported character encodings, see [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

## Numbers Converted to Exponents {#bridgehead_4601081189}

If you use Microsoft Excel to create your CSV file, you might notice that narrow columns containing long numbers appear with exponential notation. Excel uses exponential notation if the value is too long for the width of the column, which could result in the import taking longer than it should. To avoid a long import, open the CSV file in a text editor such as Notepad to ensure that the correct numbers are submitted in the import.

## Invalid Country Codes {#bridgehead_N353514}

The Import Assistant does not support the use of country codes in imported CSV files. The following error is returned if a file includes country codes rather than localized country names: 'Invalid country reference key US'.

To avoid this error, change country codes to country names. For more information, see [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html).

## Invalid Subsidiary Errors {#bridgehead_N353550}

For an import of entities such as customers, partners, or vendors, you may receive errors stating that subsidiaries are not valid for their associated entities, if the subsidiary names are not formatted as expected. Errors are like the following: 'Transaction subsidiary <subsidiary\_name> is not valid for entity <customer\_name>. Please choose a different entity.'

To avoid these errors, your CSV file needs to include the full hierarchical names for subsidiaries, with colons used as separators. The format is `<grandparent_name> : <parent_name> : <subsidiary_name>`. An example is Consolidated Parent Company : UK Subsidiary : German Subsidiary.

## Invalid Department Reference Key {#bridgehead_1518422758}

You may receive errors like the following: 'Invalid department reference key for xxx'. If you receive this error, verify the following:

-   Ensure that the department is spelled correctly. If a parent-child relationship exists, make sure that the names of the parent departments are included. For example, if Accounting is a child of Finance, the department must be entered as Finance : Accounting.
    
-   Ensure that the department is active. Go to _Setup > Company > Classifications > Departments_. Check the **Show Inactives** box and make sure that the department specified in the error message is not inactive.
    
-   If internal IDs are used, on the Field Mapping page, click the edit icon beside the **Department** field. Then, click **Choose Reference Type** and select **Internal Id**.
    
-   If external IDs are used, on the Field Mapping Page of the CSV import, click the edit icon beside the **Department** field. Then, click **Choose Reference Type** and select **External Id**.
    

## Exceeded Script Usage Limit Errors {#bridgehead_1534159345}

You may receive errors stating that you exceeded the script execution usage limits. The SuiteScript governance model tracks usage points on the API level and script type level. When certain APIs are called in a script, their assigned usage points are added and the total is compared to the script's usage limit. If the total usage points consumed by all APIs in a script exceeds the usage limit for that script's type, the error is thrown.

For more information, see [Script Type Usage Unit Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3351480.html) and SuiteAnswers article 45313.

## Post Processing Errors {#bridgehead_N353565}

Post processing errors occur after the data has been imported into the NetSuite database. Application errors, such as an invalid value in an enumerated field, or a reference that does not match the record type, are examples of post processing errors.

Another example of a post processing error is a problem with an afterSubmit script. When an afterSubmit script runs after a CSV import, and the script fails, the records are still created or updated in NetSuite. The CSV response indicates that the record has been created or updated even if an afterSubmit script that runs after the CSV import fails. For more information, see [AfterSubmit Script failed, record created with internalId xxx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4568642498.html#bridgehead_1515678023).

If your import incurs post processing errors, the import email notification, that goes to the email address used to log in to the session that initiated the import job, contains a zip file that lists the errors, including the column name and number of rows affected. You can go back and fix these errors, start the Import Assistant, and upload your corrected file. For more details, see [CSV Import Email Notifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html#bridgehead_N353043).

For additional information about CSV import errors, see [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html).

### Related Topics

-   [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html)
-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)
-   [Canceling a CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353181.html)
-   [Deleting Incorrect CSV Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353700.html)
-   [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
