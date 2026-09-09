---
id: "section_N386282"
type: "section"
title: "Leads Only Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Leads Only Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N386282.html"
anchors: ["bridgehead_N386467", "bridgehead_N386839", "bridgehead_N386861", "bridgehead_N386908", "bridgehead_N386976", "bridgehead_N388788", "bridgehead_N388896"]
sha256: "50088b0764bcd6fa28891617d588f8ed7f887db4ee451844a12218dde35bf44e"
---

The Leads Only import adds or updates data in the Customer record. Note that Customers Only imports and Prospects Only imports also affect Customer record data. The Stage field on a Customer record defines whether the entity is a Lead, Customer, or Prospect.

To be defined as a Lead, rather than a Customer or a Prospect, an entity must have no associated estimates, opportunities, or transactions. If an estimate or opportunity is created for a lead, the lead becomes a prospect. If a sales transaction is created for a lead, the lead becomes a customer.

For details about fields that can be mapped in the customer record, see the SOAP Schema Browser's [customer](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customer.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Leads imports:

-   [Supported Lead Sublist Imports](#bridgehead_N386467)
    
-   [Default Values for Leads' Primary Sales Rep](#bridgehead_N386839)
    
-   [Including Primary Contact in Leads Import](#bridgehead_N386861)
    
-   [Leads as Individuals or Companies](#bridgehead_N386908)
    
-   [Sales Rules and Lead Imports](#bridgehead_N386976)
    
-   [Setting the Global Subscription Status Field for Leads](#bridgehead_N388788)
    
-   [Leads Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N388896)
    

## Supported Lead Sublist Imports {#bridgehead_N386467}

The Leads import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Credit Cards | Addition of new records is supported; update of existing lines isn't supported. |
| Downloads | When Sell Files feature enabled. |
| Group Pricing | When Multiple Prices feature enabled. |
| Item Pricing | When Multiple Prices feature enabled. |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| Sales Team | When Team Selling feature enabled. |

Every sublist on each record can optionally have a separate file. For imports that update existing Lead records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Default Values for Leads' Primary Sales Rep {#bridgehead_N386839}

For Lead records added through CSV import, values for Primary Sales Rep don't default to be the user performing the import. This behavior differs from the NetSuite user interface, where the user entering data on the form is the default for Primary Sales Rep. If a CSV file doesn't include values for Primary Sales Rep, you can specify a default value on the Import Assistant's Field Mapping page. For information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).

## Including Primary Contact in Leads Import {#bridgehead_N386861}

If you plan to import a Leads CSV file that includes data for Primary Contact, the Contacts data must first exist in NetSuite.

-   If this data is not yet in NetSuite, you need to complete a CSV import of Contacts data before you import the Leads CSV file. Leave the Company field blank in the Contacts CSV file that you import.
    
-   After the Contacts data exists in your account, you can import the Leads data. Make sure the CSV file includes contact names in the Primary Contact column. When the entities data is imported with the Primary Contact field completed, the system links the Contact record with the entity record.
    

Note:

It is now possible to import Leads and Contacts in a single Import Assistant job. See [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html).

## Leads as Individuals or Companies {#bridgehead_N386908}

NetSuite lets you define each lead as either an individual (a person) or a company. The NetSuite Fields pane of the Import Assistant's Field Mapping page includes an Individual field for Leads. This field is required.

-   The Individual field is a indicating whether the lead is a company or a person. It corresponds to the Type option buttons on the Lead form.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   A True value indicates a lead is an individual; a False value indicates a lead is a company.
        
    -   The Company Name field is required for records with a False value, but not for records with a True value.
        

Note:

Your account's setting for the Default Customer Type field, at _Setup > Company > General Preferences_, may affect the value of the Individual field for Leads imports.

## Sales Rules and Lead Imports {#bridgehead_N386976}

If you want automatic sales territory assignment rules to apply to imported lead records, be aware of the following:

-   In Lead imports, sales rules are not applied to records that have values set for Sales Rep (when Team Selling isn't enabled), or for Sales Role (when Team Selling is enabled). These values can be set either in CSV files or as defaults on the Field Mapping page. For records that don't have values set for Sales Rep or Sales Role, sales rules are applied when other field values trigger them, exactly as in the user interface.
    
-   If territory assignments are not made during import, you can do a mass update after import, at _Lists > Mass Update > Mass Updates_. Under Sales Force Automation, select one of the following updates: Change Sales Rep Assignment, Change Territory Assignment, or Reassign Customers by Sales Territory Rules. Note that billing address data is required for these mass updates to work properly.
    

For more information about sales territory assignments, see [Sales Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039705.html) and [Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html).

## Setting the Global Subscription Status Field for Leads {#bridgehead_N388788}

The Global Subscription Status field on lead records determines whether a lead can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a lead, set this field's value to Soft Opt-In, because you can't send campaign email to users with Soft Opt-Out status; you can only send opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Leads Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N388896}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for Leads Only imports. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type, choose the import character encoding. For information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)
-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
