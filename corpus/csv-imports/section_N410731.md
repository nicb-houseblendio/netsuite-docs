---
id: "section_N410731"
type: "section"
title: "Customer Payment Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Customer Payment Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N410731.html"
anchors: ["bridgehead_1491217794", "bridgehead_N410921", "bridgehead_N411103"]
sha256: "f98e666151a9578fb2c809eb18e1a9c788688b275162423637bd1dbc696f3135"
---

NetSuite Customer Payment transactions are records of payments. You can use the customer payment import to import historical sales data.

Note:

To maintain performance, 5000 lines per transaction is the maximum limit for transactions submitted through CSV import. The number of lines a record can contain is specific to the record.

You can import unapplied payment amounts, or apply some or all payment amounts to invoices. If you're importing both customer payments and invoices, and you want to apply imported payments to imported invoices, you need to import invoices first. Include unique IDs, preferably external IDs, for your invoice records. You then can reference invoices in your customer payment import file by including their unique IDs as Invoices sublist field values.

Important:

A payment can be associated with an invoice through the internal ID or external ID only. The transaction ID is not unique and can't be used.

-   The customer payment import uses the following logic to apply payments to invoices, based on values for the Payment Amount field, and Invoices Payment sublist fields:
    
    -   If the Payment Amount value is greater than the total of all Invoices Payment values, the remainder is an unapplied payment.
        
    -   If the Payment Amount is equal to the total of all Invoices Payment values, the entire payment is applied.
        
    -   If the Payment Amount is less than the total of all Invoices Payment values, only the Payment Amount is applied, and no error is returned.
        
-   If you import customer payment records with a value of False for the Undep. Funds field, you must supply an account for each of these records. Otherwise an error occurs. If Undep. Funds is set to True, this value overrides Payment Method, and if Undep. Funds is set to False, Account overrides Payment Method.
    
-   If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account and A/R Account fields should include both account number and name, for example: 11000 Accounts Receivable. If this preference isn't enabled, values should be account name only, for example: Accounts Receivable.
    
-   If your Chart of Accounts includes more than one account of the Accounts Receivable type, map the A/R Account field in the Import Assistant, and include a column with A/R account values in the CSV file. The A/R account value for each customer payment record should match the account to which related invoices were posted. If you don't import an A/R account value for an imported payment record, the default A/R account is used, and an error occurs if the payment is applied to an invoice that was posted to a different account.
    

## Customer Payment Import Examples {#bridgehead_1491217794}

The following example shows a customer payment import where the payment amounts aren't applied to invoices.

| External ID | Customer | Payment Amount | Date |
| --- | --- | --- | --- |
| Cust\_Payment\_3 | John King | 6500 | 4/3/2017 |
| Cust\_Payment\_4 | Marie LaBelle | 15000 | 4/3/2017 |
| Cust\_Payment\_5 | Tim Johnson | 8000 | 4/3/2017 |

The following example shows a customer payment import where the payment amounts are applied to invoices.

| External ID | Customer | Date | Invoice ID | Payment Amount |
| --- | --- | --- | --- | --- |
| CP-001 | John Woodhouse | 5/18/2017 | INV-425 | 10000 |
| CP-002 | Tim Johnson | 5/16/2017 | INV-633 | 6500 |
| CP-003 | Ellen Guest | 5/4/2017 | INV-732 | 1800 |

For details about fields that can be mapped in the customer payment record, see the SOAP Schema Browser's [customer payment](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customerpayment.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Customer Payment imports:

-   [Supported Customer Payment Sublist Data Imports](#bridgehead_N410921)
    
-   [Using Import Assistant for Customer Payments Mass Update](#bridgehead_N411103)
    

## Supported Customer Payment Sublist Data Imports {#bridgehead_N410921}

The Customer Payment import supports the import of Invoices sublist data. Each line in this sublist represents an invoice to which the payment is applied. The sum of Payment field values for sublist records represents the total amount of the payment.

In this sublist, the required Invoice key field holds the transaction IDs for invoices to which payments are applied. An additional, optional Line key field holds the line numbers for the invoice lines to which payments are applied, if payments need to be applied to specific lines.

Note:

If you use only the Invoice key, the following error may be returned to indicate that a unique reference wasn't found, 'Ambiguous sublist reference; multiple matches exist for key value <>'.

An import can add new invoices or invoice lines to which a payment is applied, change the amounts applied to existing invoices or invoice lines, or remove invoices or invoice lines.

When the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option isn't enabled (which is the default), CSV file sublist data selectively updates existing invoices data, based on the Invoice key field. When this option is enabled, CSV file sublist data completely replaces existing invoices data. For example:

-   If the existing Invoices sublist data is:
    
    Invoice A: $100
    
    Invoice B: $200
    
-   And CSV file sublist data is:
    
    Invoice A: $120
    
    Invoice C: $180
    
-   When Overwrite Sublists=F, post update sublist data is:
    
    Invoice A: $120
    
    Invoice B: $200
    
    Invoice C: $180
    
-   When Overwrite Sublists=T, post update sublist data is:
    
    Invoice A: $120
    
    Invoice C: $180
    

The Customer Payment import also supports the import of Accounting Book Detail sublist data. The Accounting Book Detail sublist is available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. This sublist is selectively updateable based on the Accounting Book key field.

Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Using Import Assistant for Customer Payments Mass Update {#bridgehead_N411103}

You can perform a mass update of existing Customer Payments main fields by exporting Customer Payments saved search results, changing data externally, then using the Import Assistant to import modified data, using the Update data handling option. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
