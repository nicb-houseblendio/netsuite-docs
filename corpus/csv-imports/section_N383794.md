---
id: "section_N383794"
type: "section"
title: "Customers Only Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Customers Only Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html"
anchors: ["bridgehead_N384844", "bridgehead_N385334", "bridgehead_N385356", "bridgehead_N385403", "bridgehead_N385478", "bridgehead_N385500", "bridgehead_N385568", "procedure_N385597", "bridgehead_N385675", "bridgehead_N385793"]
sha256: "e1a62ba0e52e502a8784caba8632e909afd4b4545820dd3ad92e93154742e1e1"
---

The Customers Only import adds or updates data in the Customer record. Note that Leads Only imports and Prospects Only imports also affect Customer record data. The Stage field on a Customer record defines whether the entity is a Lead, Customer, or Prospect. To be defined as a Customer, rather than a Lead or a Prospect, an entity must have one or more associated sales transactions or closed opportunities.

For details about fields that can be mapped in the customer record, see the SOAP Schema Browser's [customer](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customer.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Customers imports:

-   [Supported Customer Sublist Imports](#bridgehead_N384844)
    
-   [Default Values for Customers' Primary Sales Rep](#bridgehead_N385334)
    
-   [Including Primary Contact in Customers Import](#bridgehead_N385356)
    
-   [Customers as Individuals or Companies](#bridgehead_N385403)
    
-   [Setting Sales Teams for Child Customers](#bridgehead_N385478)
    
-   [Importing NetSuite Access Details for Customer Contacts](#bridgehead_N385500)
    
-   [Setting Multiple Transaction Currencies for Customers](#bridgehead_N385568)
    
-   [Setting the Global Subscription Status Field for Customers](#bridgehead_N385675)
    
-   [Customers Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N385793)
    

## Supported Customer Sublist Imports {#bridgehead_N384844}

The Customers import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Contact Access | Available for updates of existing customers only, to add or update NetSuite access information for existing customer contacts. See [Importing NetSuite Access Details for Customer Contacts](#bridgehead_N385500). Selectively updatable based on Contact key field. |
| Credit Cards | Addition of new records is supported. Update of existing lines isn't supported. |
| Currencies | When Multiple Currencies feature enabled. See [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html) and [Setting Multiple Transaction Currencies for Customers](#bridgehead_N385568). |
| Downloads | When Sell Files feature enabled. |
| Group Pricing | When Multiple Prices feature enabled. |
| Item Pricing | When Multiple Prices feature enabled. |
| Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| Sales Team | When Team Selling feature enabled. See [Setting Sales Teams for Child Customers](#bridgehead_N385478). |
| Subscriptions | Selectively updatable based on Subscription key field. |
| Tax Registrations | Available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab. Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services. For information about working with the tax registrations sublist through SOAP web services, see [Working with Customer Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html#bridgehead_N3641457). For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html). |

Every sublist on each record can optionally have a separate file. For imports that update existing Customer records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Default Values for Customers' Primary Sales Rep {#bridgehead_N385334}

For Customer records added through CSV import, values for Primary Sales Rep don't default to be the user performing the import. This behavior differs from the NetSuite user interface, where the user entering data on the Customer form is the default for Primary Sales Rep. If a CSV file doesn't include values for Primary Sales Rep, you can specify a default value on the Import Assistant's Field Mapping page. For information, see [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).

## Including Primary Contact in Customers Import {#bridgehead_N385356}

If you plan to import a Customers CSV file that includes data for Primary Contact, the Contacts data must first exist in NetSuite.

-   If this data is not yet in NetSuite, you need to complete a CSV import of Contacts data before you import the Customers CSV file. Leave the Company field blank in the Contacts CSV file that you import.
    
-   After the Contacts data exists in your account, you can import the Customers data. Make sure the CSV file includes contact names in the Primary Contact column. When the entities data is imported with the Primary Contact field completed, the system links the Contact record with the entity record.
    

Note:

It is possible to import Customers and Contacts in a single import job. See [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html).

## Customers as Individuals or Companies {#bridgehead_N385403}

NetSuite lets you define each customer as either an individual (a person) or a company. The NetSuite Fields pane of the Import Assistant's Field Mapping page includes an Individual field for Customers. This field is required.

-   The Individual field is a indicating whether the customer is a company or a person. It corresponds to the Type option buttons on the Customer form.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   A True value indicates a customer is an individual; a False value indicates a customer is a company.
        
    -   The Company Name field is required for records with a False value, but not for records with a True value.
        
-   You can set a default value for the Individual field by clicking its edit icon on the Field Mapping page. In the Default Value popup: choose Yes to default customer type to individual, choose No to default customer type to company.
    

Note:

Your account's setting for the Default Customer Type field, at _Setup > Company > General Preferences_, may affect the value of the Individual field for Customers imports.

## Setting Sales Teams for Child Customers {#bridgehead_N385478}

Note that if a customer is set up as a child of another customer, by default the child customer inherits the sales team of the parent customer. If you want to set up a different sales team for a child customer, enable the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option and include sales team values in the CSV file.

## Importing NetSuite Access Details for Customer Contacts {#bridgehead_N385500}

For Customers Only imports that update existing records, the Field Mapping page includes a Contact Access sublist. You can map this sublist's fields to provide Customer Center access to contacts.

Sublist fields include:

-   Access - indicating whether to grant NetSuite access to the contact
    
-   Contact - Contact name used the key for the sublist
    
-   Email - Email address used as the NetSuite username for the contact
    
-   Notify - indicating whether to send notification email to contact
    
-   Password - NetSuite password for the contact
    
-   Role - NetSuite role assigned to the contact (Customer Center)
    

You can import this data during updates of preexisting customer records that have preexisting contact records already attached. You can't add new customer records, add new contact records, or attach new contacts to customers at the same time that you import contact access data. You must complete these other tasks first, either in the user interface or through an import, before you can import contact access data. Here is the workflow: 1) Add customers. 2) Add contacts. 3) Attach contacts to customers. 4) Update customers to give access to attached contacts.

## Setting Multiple Transaction Currencies for Customers {#bridgehead_N385568}

The Multiple Currencies feature enables you to enter sales transactions in multiple currencies for individual customers. For details about using this feature, see [Currency Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1395057.html).

When this feature is enabled, you can define a primary currency for customers by including the Currency body field in your CSV file and mapping it in the Import Assistant, exactly as you would without the feature enabled. However, you can also define additional currencies that can be used in this customer's transactions, called transaction currencies, by mapping a Currencies sublist Currency field to an additional Currency field in your CSV file, for each additional currency to be supported.

#### To import transaction currencies for a customer: {#procedure_N385597}

1.  In your Customers CSV file, add a column for each additional currency that you want to support, with a different name for each column, for example: TransCurrency1, TransCurrency2, TransCurrency3.
    
2.  Start a Customers import.
    
3.  On the Field Mapping page, after you have mapped other customer fields as necessary, map the Customer Currencies 1 sublist's Currency field to an additional currency column in your CSV file.
    
4.  Click the + sign next to the Customer Currencies folder to create another Customer Currencies sublist, and map that Currency field to another currency column in your CSV file.
    
5.  Repeat step 4 until all currency columns in your CSV file are mapped.
    
    ![Transaction currencies import example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CustCurrImport.png)
6.  Complete the import as you normally would.
    

Note:

The currencies defined for the Customer Currencies sublist can be imported as values for the Currency field in Cash Sale, Estimate, Invoice, and Sales Order imports.

## Setting the Global Subscription Status Field for Customers {#bridgehead_N385675}

The Global Subscription Status field on customer records determines whether a customer can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a customer, set this field's value to Soft Opt-In, because you can't send campaign email to users with Soft Opt-Out status, you can only send opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Customers Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N385793}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for Customers Only imports. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

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
