---
id: "section_N390628"
type: "section"
title: "Vendors Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Vendors Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N390628.html"
anchors: ["bridgehead_N390786", "bridgehead_N391550", "bridgehead_N391659", "bridgehead_N391727"]
sha256: "647c517d5e946e05a6f6caa336719cb017884ce42f089723c5483242680a1bbb"
---

The vendors import adds vendors to the Vendors list.

For details about fields that can be mapped in the vendor record, see the SOAP Schema Browser's [vendor](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendor.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Important:

You must create payment terms prior to referencing them during the Import Assistant's Vendor import. In the previously supported CSV import process for vendors, new Payment Terms referenced during a Vendor import would cause a new payment term to be created in the account.

Review the following guidelines for Vendors imports:

-   [Supported Vendor Sublist Imports](#bridgehead_N390786)
    
-   [Setting the Global Subscription Status Field for Vendors](#bridgehead_N391550)
    
-   [Vendors as Individuals or Companies](#bridgehead_N391659)
    
-   [Vendors Primary Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N391727)
    

## Supported Vendor Sublist Imports {#bridgehead_N390786}

The Vendors import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Roles | \- |
| Subscriptions | Selectively updatable based on Subscription key field. |
| Tax Registrations | Available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab. Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services. For information about working with the tax registrations sublist through SOAP web services, see [Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3646902.html). For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html). |

For imports that update existing Vendor records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Setting the Global Subscription Status Field for Vendors {#bridgehead_N391550}

The Global Subscription Status field on vendor records determines whether a vendor can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a vendor, set this field's value to Soft Opt-In, because you can't send a campaign email to users with Soft Opt-Out status; you can only send an opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Vendors as Individuals or Companies {#bridgehead_N391659}

NetSuite lets you define each vendor as either an individual (a person) or a company. The NetSuite Fields pane of the Import Assistant's Field Mapping page includes an Individual field for Vendors. This field is required.

-   The Individual field is a indicating whether the vendor is a company or a person. It corresponds to the Type option buttons on the Vendor form.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   A True value indicates a vendor is an individual; a False value indicates a prospect is a company.
        
    -   The Company Name field is required for records with a False value, but not for records with a True value.
        

Note:

Your account setting for the Default Vendor Type field, at _Setup > Company > General Preferences_, may affect the value of the Individual field for Vendors imports.

## Vendors Primary Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N391727}

If your account is using NetSuite OneWorld, the Primary Subsidiary field is required for Vendors imports. You must map the NetSuite Primary Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

Note:

You can't import a vendor with multiple subsidiaries using CSV Import.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
