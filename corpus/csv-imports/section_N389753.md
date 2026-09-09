---
id: "section_N389753"
type: "section"
title: "Prospects Only Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Prospects Only Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N389753.html"
anchors: ["bridgehead_N389924", "bridgehead_N390296", "bridgehead_N390318", "bridgehead_N390365", "bridgehead_N390433", "bridgehead_N390551"]
sha256: "40046d60c84820514dab4fc86ca6bc0f3d3d5be4bc54412e28a12ea010c22168"
---

The Prospects Only import adds or updates data in the Customer record. Note that Customers Only imports and Leads Only imports also affect Customer record data. The Stage field on a Customer record defines whether the entity is a Lead, Customer, or Prospect.

Prospects have no associated sales orders, invoices, cash sales, or other sales transactions, but do have associated opportunities or estimates. If a sales transaction is created for a prospect, or an opportunity is closed for a prospect, the prospect becomes a customer.

For details about fields that can be mapped in the customer record, see the SOAP Schema Browser's [customer](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customer.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Prospects imports:

-   [Supported Prospect Sublist Imports](#bridgehead_N389924)
    
-   [Default Values for Prospects' Primary Sales Rep](#bridgehead_N390296)
    
-   [Including Primary Contact in Prospects Import](#bridgehead_N390318)
    
-   [Prospects as Individuals or Companies](#bridgehead_N390365)
    
-   [Setting the Global Subscription Status Field for Prospects](#bridgehead_N390433)
    
-   [Prospects Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N390551)
    

## Supported Prospect Sublist Imports {#bridgehead_N389924}

The Prospects import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Credit Cards | Addition of new records is supported; update of existing lines isn't supported. |
| Downloads | When Sell Files feature enabled. |
| Group Pricing | When Multiple Prices feature enabled. |
| Item Pricing | When Multiple Prices feature enabled. |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| Sales Team | When Team Selling feature enabled. |

Every sublist on each record can optionally have a separate file. For imports that update existing Prospect records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Default Values for Prospects' Primary Sales Rep {#bridgehead_N390296}

For Prospect records added through CSV import, values for Primary Sales Rep don't default to be the user performing the import. This behavior differs from the NetSuite user interface, where the user entering data on the form is the default for Primary Sales Rep. If a CSV file doesn't include values for Primary Sales Rep, you can specify a default value on the Import Assistant's Field Mapping page. For information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).

## Including Primary Contact in Prospects Import {#bridgehead_N390318}

If you plan to import a Prospects CSV file that includes data for Primary Contact, the Contacts data must first exist in NetSuite.

-   If this data is not yet in NetSuite, you need to complete a CSV import of Contacts data before you import the Prospects CSV file. Leave the Company field blank in the Contacts CSV file that you import.
    
-   After the Contacts data exists in your account, you can import the Prospects data. Make sure the CSV file includes contact names in the Primary Contact column. When the entities data is imported with the Primary Contact field completed, the system links the Contact record with the entity record.
    

Note:

It is now possible to import Prospects and Contacts in a single Import Assistant job. See [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html).

## Prospects as Individuals or Companies {#bridgehead_N390365}

NetSuite lets you define each prospect as either an individual (a person) or a company. The NetSuite Fields pane of the Import Assistant's Field Mapping page includes an Individual field for Prospects. This field is required.

-   The Individual field is a indicating whether the prospect is a company or a person. It corresponds to the Type option buttons on the Prospect form.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   A True value indicates a prospect is an individual; a False value indicates a prospect is a company.
        
    -   The Company Name field is required for records with a False value, but not for records with a True value.
        

Note:

Your account's setting for the Default Customer Type field, at _Setup > Company > General Preferences_, may affect the value of the Individual field for Prospects imports.

## Setting the Global Subscription Status Field for Prospects {#bridgehead_N390433}

The Global Subscription Status field on prospect records determines whether a prospect can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a prospect, set this field's value to Soft Opt-In, because you can't send a campaign email to users with Soft Opt-Out status; you can only send an opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Prospects Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N390551}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for Prospects Only imports. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
