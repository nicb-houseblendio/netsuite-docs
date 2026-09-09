---
id: "section_N357847"
type: "section"
title: "Chart of Accounts Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Accounting Import Type > Chart of Accounts Import"
parent: "section_N357752"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N357847.html"
anchors: ["bridgehead_4746566287", "bridgehead_4746566439", "bridgehead_N358923"]
sha256: "a2e7b9b8760e740f5060c91de59d2d1c5a7824c8545f69ee274b501417071fbc"
---

The Chart of Accounts import adds ledger accounts to the Account list record. Because the Chart of Accounts is the basis for all company data, you should complete this import first when you're setting up a new NetSuite account.

Please note the following before importing or updating account records with the Import Assistant:

-   This import isn't available in the NetCRM product.
    
-   You can't create a new account or update an existing account with an account number that already exists. You receive an error that the account number is already used.
    
-   To update account numbers on the import, the Use Account Numbers option must be enabled in _Setup > Accounting > Accounting Preferences_ > General.
    
-   If your account is using NetSuite OneWorld, the Subsidiaries field is a required field for Chart of Accounts imports. You must map the NetSuite Subsidiaries field to a field in your CSV file, or the import will fail.
    
-   For information about setting up parent/child relationships for imported account records, see [Referencing Child Accounts by Name and Number](#bridgehead_N358923).
    

For details about fields that can be mapped in the Account record, see the SOAP Schema Browser's [account](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/account.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Account Localization Sublist {#bridgehead_4746566287}

In OneWorld accounts that have multiple languages enabled, Account Localization sublist information can be included in the chart of accounts import. The Account Localization sublist doesn't have a key. The records in the sublist can be language, name, accounting context, and number.

## Chart of Accounts Import Example {#bridgehead_4746566439}

The following tables illustrate sample data in a Chart of Accounts import.

| External Id | Account Number | Account Name | Account Type | Description | Date | Currency | Restrict to Class | Subaccount of |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| CA-ACCT-01 | 515652 | Direct Labor | Expense | Expense account for labor | 01/01/2016 | YEN | Recurring Business | Project Cost |
| CA-ACCT-02 | 987546 | Sales Tax Payable | Other Current Liability | Sales tax liability | 01/16/2016 | USD | Recurring Business | Tax Liability |

## Referencing Child Accounts by Name and Number {#bridgehead_N358923}

For reference types in the CSV file, data values must be written exactly as they appear in the list in the NetSuite record form.

For example, if the Income Account dropdown list has an option entitled 40500 Sales, you must specify the full name '40500 Sales' in the CSV file for the reference type to be imported correctly after it's mapped on the Import Assistant's Field Mapping page.

-   You can't provide only the value '40500'.
    
-   You can't provide only the value 'Sales'.
    
-   The account number and name must be separated by a single space, not a colon or other separator.
    

For more information about reference types, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).

Note:

Account references are different for budget imports; they require only names and not numbers. For more information, see [Budget Template File Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433988.html#bridgehead_N434174).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Chart of Accounts Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1439850.html)

### Related Topics

-   [Accounting Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N357752.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
