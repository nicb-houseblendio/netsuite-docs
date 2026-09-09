---
id: "section_N429286"
type: "section"
title: "Vendor Payment Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Vendor Payment Import"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N429286.html"
anchors: ["bridgehead_1543229505", "bridgehead_N429482", "bridgehead_N429664"]
sha256: "d19878e8649430e67962a60221526deaceca0af368f43b130adcf676625694e5"
---

NetSuite Vendor Payment transactions record payment of vendor bills when they're due. These transactions post expenses to the general ledger, and affect both accounts payable and the bank account used for the payment.

Note:

To maintain performance, don't submit transactions that contain more than 5000 lines through CSV import.

For more details about vendor payments in NetSuite, see [Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2381615.html).

## Usage Notes {#bridgehead_1543229505}

Consider the following usage notes when importing vendor payment data.

-   You can import Vendor Payment transaction data in a single CSV file, or in multiple files.
    
-   You must map external ID or internal ID to serve as a unique ID per record. The unique ID should be included in every line of the CSV files. For imports of new data, use external ID.
    
-   Each imported Vendor Payment record should include a reference to a NetSuite Vendor record, mapped to the Vendor Payment's Payee field. This reference should match exactly the Vendor ID field value in the Vendor Record.
    
-   You must map a CSV file field to the NetSuite Account field to represent the accounts from which payments are made. You have the option of mapping to the A/P Account field to represent the accounts payable accounts impacted by payments. If the Use Account Numbers preference has been enabled at _Setup > Accounting > Accounting Preferences_, imported values for the Account and A/P Account fields should include both account number and name, for example: 11000 Accounts Payable. If this preference isn't enabled, values should be account name only, for example: Accounts Payable.
    
-   All vendor payments must be applied to vendor bills in full. You can't import unapplied amounts. You can't import a total amount value for a payment; this amount is calculated by adding all of the values for the Payment field in the Bills sublist data.
    
    If you're importing both vendor payments and vendor bills, and you want to apply imported payments to imported bills, you need to import bills first.
    
-   If the Multiple Currencies feature is enabled, you must map the Exchange Rate field. If your CSV file doesn't include values for this field, you can set it to a default value. Currency values are taken from referenced vendors. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).
    
-   To import data for the In-Transit, Available Balance, Approval Status, and Next Approver fields, you must enable the following features and set the following preferences:
    
    -   Enable the In-Transit Payments feature at _Setup > Company > Setup Tasks > Enable Features_, on the Accounting subtab.
        
    -   Check Vendor Bills and Vendor Payments at _Setup > Accounting > Preferences > Accounting Preferences_, on the Approval Routing Subtab.
        
    -   Select a Vendor In-Transit Payment Account at _Setup > Accounting > Preferences > Accounting Preferences_, on the General subtab, under Accounts Payable. Also check the Use In-Transit Vendor Payments by Default box.
        

For details about fields that can be mapped in the vendor payment record, see the SOAP Schema Browser's [vendor payment](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendorpayment.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for vendor payment imports:

-   [Supported Vendor Payment Sublist Data Imports](#bridgehead_N429482)
    
-   [Using Import Assistant for Vendor Payments Mass Update](#bridgehead_N429664)
    

## Supported Vendor Payment Sublist Data Imports {#bridgehead_N429482}

The Vendor Payment import supports the import of Bills sublist data. Each line in this sublist represents a vendor bill to which the payment is applied. The sum of Payment field values for sublist records represents the total amount of the payment.

In this sublist, the required Bill key field holds the transaction IDs for vendor bills to which payments are applied. An additional, optional Line key field holds the line numbers for the vendor bill lines to which payments are applied.

Note:

If you use only the Bill key, the following error may be returned to indicate that a unique reference wasn't found, 'Ambiguous sublist reference; multiple matches exist for key value <>'.

An import can add new vendor bills or vendor bill lines to which a payment is applied, change the amounts applied to existing vendor bills or vendor bill lines, or remove vendor bills or vendor bill lines.

When the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option isn't enabled (which is the default), CSV file sublist data selectively updates existing vendor bills data. When this option is enabled, the CSV file sublist data completely replaces existing vendor bills data. For example:

-   If the existing Vendor Payment Bills sublist data is:
    
    Vendor Bill A: $100
    
    Vendor Bill B: $200
    
-   And CSV file sublist data is:
    
    Vendor Bill A: $120
    
    Vendor Bill C: $180
    
-   When Overwrite Sublists=F, post update sublist data is:
    
    Vendor Bill A: $120
    
    Vendor Bill B: $200
    
    Vendor Bill C: $180
    
-   When Overwrite Sublists=T, post update sublist data is:
    
    Vendor Bill A: $120
    
    Vendor Bill C: $180
    

The Vendor Payment Import also supports the import of Accounting Book Detail sublist data. Accounting Book Detail sublist data is available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. This sublist is selectively updateable based on the Accounting Book key field.

Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Using Import Assistant for Vendor Payments Mass Update {#bridgehead_N429664}

You can perform a mass update of existing Vendor Payment main fields by creating a Transaction saved search with a filter of Type is Vendor Payment, changing data externally, then using the Import Assistant to import modified data. For more information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
