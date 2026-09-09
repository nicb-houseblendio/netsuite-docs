---
id: "section_N383204"
type: "section"
title: "Contacts Only Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Contacts Only Import"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383204.html"
anchors: ["bridgehead_N383364", "bridgehead_N383527", "bridgehead_N383540", "bridgehead_N383609", "bridgehead_N383717", "bridgehead_4734325073", "bridgehead_4734339086", "bridgehead_4734339199", "bridgehead_4734339515"]
sha256: "b0e05288bf8161622f4231662c1a6def9dadda730c262233adc05b016174b474"
---

The Contacts Only import is used to attach individual names to existing entries in the customer, vendor, partner, or other name list. Contacts also can be imported without reference to an entity. These names can later be linked to one or more businesses in these lists.

For details about fields that can be mapped in the contact record, see the SOAP Schema Browser's [contact](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/contact.html) reference page. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Review the following guidelines for Contacts imports:

-   [Supported Contact Sublist Imports](#bridgehead_N383364)
    
-   [Importing Contacts for Existing Entity Data](#bridgehead_N383527)
    
-   [Importing Contacts and New Entities Data](#bridgehead_N383540)
    
-   [Setting the Global Subscription Status Field for Contacts](#bridgehead_N383609)
    
-   [Contacts Subsidiary Field Required for NetSuite OneWorld](#bridgehead_N383717)
    

Note:

If you want to update the Company field for a contact record, you need to use a key of internal ID or external ID, rather than name. To set up this key, click the edit icon for the Company field on the Import Assistant Field Mapping page, and select from the Choose Reference Type list. Otherwise the import job creates a new contact record with the same name and the Company field populated, instead of updating the existing contact record.

## Supported Contact Sublist Imports {#bridgehead_N383364}

The Contacts import supports the import of the following sublist data:

| Sublist | Notes |
| --- | --- |
| Address | Selectively updatable based on Internal ID or Label key field. By default, the sublist Address field is read-only, and data from other sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field. |
| Subscriptions | Selectively updatable based on Subscription key field. |

For imports that update existing Contact records, handling of sublist data updates depends upon the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) advanced option, and on whether the sublist is keyed. Complete deletion of sublist data currently isn't supported. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

## Importing Contacts for Existing Entity Data {#bridgehead_N383527}

If you want to import contacts for entities (Customers, Leads, Prospects, or Vendors) that already exist in NetSuite, include entity names in the Company column of Contacts CSV file data.

## Importing Contacts and New Entities Data {#bridgehead_N383540}

You can import Contacts with their related Customers, Leads, or Prospects in a single Import Assistant job. For more information, see [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html).

The Import Assistant also supports a two-step import of Contacts and entities.

-   You should import Contacts data first, use External ID as a reference type, and don't import values for the Contacts' Company field.
    
-   After the Contacts data exists in your account, then import the entities data.
    
    -   You should use External ID as a reference type.
        
    -   Make sure the entities CSV file includes contact names in the Primary Contact column. When the entities data is imported with the Primary Contact field completed, the system links the Contact record with the entity record.
        
    -   Note that you can't set a role relationship in a two-step import; contacts can be set as primary or with no role.
        

## Setting the Global Subscription Status Field for Contacts {#bridgehead_N383609}

The Global Subscription Status field on contact records determines whether a contact can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email to a contact, set this field's value to Soft Opt-In, because you can't send campaign email to users with Soft Opt-Out status; you can only send opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-Out. When this option is enabled, the field defaults to Soft Opt-In.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Contacts Subsidiary Field Required for NetSuite OneWorld {#bridgehead_N383717}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for Contacts Only imports. You must map the NetSuite Subsidiary field to a field in your CSV file, or the import will fail. CSV file values for subsidiaries should be hierarchical names, in the format grandparent : parent : child, for example, Consolidated Parent Company : UK Subsidiary : Euro Subsidiary.

## Contacts Only CSV File Example {#bridgehead_4734325073}

The following example uses three files to import contacts only information: main contact file, address sublist, and contact subscriptions sublist.

## Contact {#bridgehead_4734339086}

| External ID | First Name | Last Name | Subsidiary | Job Title | Main Phone | Email | Category |
| --- | --- | --- | --- | --- | --- | --- | --- |
| SSE\_CON\_14 | Sandra | Johnson | ACME Corp : U.K. Subsidiary | Regional Manager | 1 958 555 0100 | sandraj@acmecarpet.com | Tradeshow |
| SSE\_CON\_18 | Andrew | Wilson | ACME Corp : German sub | CEO | 1 958 555 0199 | ajw@aaalawn.com | Website |
| SSE\_CON\_20 | Angela | Wolfe | ACME Corp : Canada subsidiary | Regional Sales Manager | 1 958 555 0121 | awolfe@breatherite.com | Phone |

We are importing contacts to associate with entities later, so there's no Company column in the file. If you want to associate the contact with an existing entity by the import, add a Company column to the file. The Subsidiary column is required for OneWorld accounts. Use the format parent : child.

Categories must exist in NetSuite or an error will occur.

## Contact Address {#bridgehead_4734339199}

| Contact Address: External ID | Contact Address: ID | Contact Address: Country | Contact Address: Address | Contact Address: City | Contact Address: State | Contact Address: Zip | Contact Address: Default Billing | Contact Address: Default Shipping |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| SSE\_CON\_14 | 83923 | United States | 123 Elm Street | Chicago | Illinois | 60604 | Yes | Yes |
| SSE\_CON\_18 | 38733 | Czechia | Trnitá 123/45 | Prague | \- | 602 00 | Yes | No |
| SSE\_CON\_20 | 36366 | Australia | Level 2, 15 King Street | Sydney | NSW | 3048 | No | Yes |

## Contact Subscriptions {#bridgehead_4734339515}

| Contact Subscriptions: External ID | Contact Subscriptions: Subscription | Contact Subscriptions: Subscribed |
| --- | --- | --- |
| SSE\_CON\_14 | Newsletters | Yes |
| SSE\_CON\_14 | Marketing | Yes |
| SSE\_CON\_18 | Surveys | Yes |
| SSE\_CON\_20 | Newsletters | No |
| SSE\_CON\_20 | Marketing | Yes |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type, choose the import character encoding. For information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html)
-   [Understanding Leads, Prospects, and Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394436.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
