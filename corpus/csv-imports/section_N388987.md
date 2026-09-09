---
id: "section_N388987"
type: "section"
title: "Partners Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Partners Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N388987.html"
anchors: ["bridgehead_N389160", "bridgehead_N389388", "bridgehead_N389419", "bridgehead_N389486", "bridgehead_N389600", "bridgehead_N389676"]
sha256: "8cce095f51d832d567bac40ea1720a7f82b2eaf8fcc165f27001c61d1ce39358"
---

The Partners import adds partners to the Partner list.

Note:

Partners imports aren't available unless partner records are enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the CRM subtab, check Partner Relationship Management.

For details about fields that can be mapped in the partner record, see the SOAP Schema Browser's [partner](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/partner.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Partners imports:

-   [Supported Partner Sublist Imports](#bridgehead_N389160)
    
-   [Importing Partners Primary and Alternate Contact Data](#bridgehead_N389388)
    
-   [Setting the Global Subscription Status Field for Partners](#bridgehead_N389486)
    
-   [Partners as Individuals or Companies](#bridgehead_N389600)
    
-   [Partners Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N389676)
    

## Supported Partner Sublist Imports {#bridgehead_N389160}

The Partners import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Contact Access | Available for updates of existing partners only, to add or update NetSuite access information for existing partner contacts. See [Importing NetSuite Access Details for Partner Contacts](#bridgehead_N389419). selectively updatable based on Contact key field |
| Promotion Codes | \- |
| Subscriptions | Selectively updatable based on Subscription key field. |
| Tax Registrations | Available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab. Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services. For information about working with the tax registrations sublist through SOAP web services, see [Partner](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3645002.html). For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html). |

For imports that update existing Partner records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Importing Partners Primary and Alternate Contact Data {#bridgehead_N389388}

If you plan to import a Partners CSV file that includes data for Primary Contact or Alternate Contact, the Contacts data must first exist in NetSuite.

-   If this data is not yet in NetSuite, you need to complete a CSV import of Contacts data before you import the Partners CSV file. Leave the Company field blank in the Contacts CSV file that you import.
    
-   After the Contacts data exists in your account, you can import the Partners data. Make sure the CSV file includes contact names in the Primary Contact column. When the partners data is imported with the Primary Contact field completed, the system links the Contact record with the partner record.
    

## Importing NetSuite Access Details for Partner Contacts {#bridgehead_N389419}

For Partners imports that update existing records, the Field Mapping page includes a Contact Access sublist. You can map this sublist's fields to provide Partner Center access to contacts.

Sublist fields include:

-   Access - indicating whether to grant NetSuite access to the contact
    
-   Contact - Contact name used the key for the sublist
    
-   Email - Email address used as the NetSuite username for the contact
    
-   Notify - indicating whether to send notification email to contact
    
-   Password - NetSuite password for the contact
    
-   Role - NetSuite role assigned to the contact (Partner Center or Advanced Partner Center)
    

You can import this data during updates of preexisting partner records that have preexisting contact records already attached. You can't add new partner records, add new contact records, or attach new contacts to partners at the same time that you import contact access data. You must complete these other tasks first, either in the user interface or through an import, before you can import contact access data. Here is the workflow: 1) Add partners. 2) Add contacts. 3) Attach contacts to partners. 4) Update partners to give access to attached contacts.

## Setting the Global Subscription Status Field for Partners {#bridgehead_N389486}

The Global Subscription Status field on partner records determines whether a partner can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a partner, set this field's value to Soft Opt-In, because you can't send campaign email to users with Soft Opt-Out status; you can only send opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Partners as Individuals or Companies {#bridgehead_N389600}

NetSuite lets you define each partner as either an individual (a person) or a company. The NetSuite Fields pane of the Import Assistant's Field Mapping page includes an Individual field for Partners. This field is required.

-   The Individual field is a indicating whether the partner is a company or a person. It corresponds to the Type option buttons on the Partner form.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   A True value indicates a partner is an individual; a False value indicates a partner is a company.
        
    -   The Company Name field is required for records with a False value, but not for records with a True value.
        
-   You can set a default value for the Individual field by clicking its edit icon on the Field Mapping page. In the Default Value popup: choose Yes to default partner type to individual, choose No to default partner type to company.
    

Note:

Your account's setting for the Default Partner Type field, at _Setup > Company > General Preferences_, may affect the value of the Individual field for Partners imports.

## Partners Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N389676}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for Partners imports. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)
-   [Managing Partners](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1166465.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
