---
id: "section_N3639940"
type: "section"
title: "Customer"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Entities > Customer"
parent: "chapter_N3639664"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html"
anchors: ["bridgehead_N3639972", "bridgehead_N3640244", "bridgehead_N3640281", "bridgehead_159420584789", "bridgehead_N3640391", "bridgehead_N3640460", "bridgehead_N3641393", "bridgehead_N3641457", "bridgehead_N3641610", "bridgehead_N3641660", "bridgehead_N3641673", "bridgehead_N3641702", "bridgehead_N3641735", "bridgehead_N3641748", "bridgehead_N3641762", "bridgehead_1544450444"]
sha256: "04422098c85d410fdd91fc529a86c9260709d3567918ff0514bf5ec848777d80"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161581923822.html).

Customer records represent people or companies that purchase goods and services from your business. Use the customer record to manage these customers. Client applications can create, update, or delete customer records. For more details, see [Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1076428.html).

The Customer record is defined in the [listRel (relationship)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) XSD.

## Supported Operations {#bridgehead_N3639972}

The following operations can be used to modify Customer records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3640244}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [customer](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customer.html) reference page. For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The monthlyClosing field is used only by the Japan Edition of NetSuite.

Note:

The balance, overdueBalance, and depositBalance fields are only returned when using advanced search. They are not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. These fields are not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3640281}

Usage notes are provided for the following topics:

-   [The EntityID Field](#bridgehead_159420584789)
    
-   [Understanding Customer Stages](#bridgehead_N3640391)
    
-   [Customer Status and Stage Internal IDs](#bridgehead_N3640460)
    
-   [Returning a Contact List for a Customer](#bridgehead_N3641393)
    
-   [Working with Customer Sublists](#bridgehead_N3641457)
    

## The EntityID Field {#bridgehead_159420584789}

The entityID field is set as an inline text field by default. Inline text fields are read only fields and may not be edited through SOAP web services. To create a new customer record, you must leave out the entityID field.

## Understanding Customer Stages {#bridgehead_N3640391}

In the NetSuite UI, there are three possible stages that can be defined for a customer - lead, prospect or customer. When entering new customers into NetSuite, you can create the record as a lead, prospect or customer record, or you can create the customer as a lead and allow NetSuite to automatically update the stage as certain criteria are met.

-   **Lead** - lets you track all the information you need to convert a lead into a customer. Leads have no estimates, opportunities or transactions associated with them. If an estimate or opportunity is created for a lead, the lead becomes a prospect. If you create a sales transaction for a lead, the lead becomes a customer.
    

Note:

When adding leads through SOAP web services, you can use the rules you have defined in the SFA (Sales Force Automation) feature to assign leads. Be aware that SFA rules are applied regardless of the setting for the 'Use Conditional Defaults on Add' preference.

-   **Prospect** -lets you track all the information you need to convert a prospect into a customer. Prospects have no sales orders, invoices, cash sales or other sales transactions associated with them. They can have opportunities and estimates associated with them, however. If a sales transaction is created for a prospect, or an opportunity is closed for a prospect, the prospect becomes a customer.
    
-   **Customer** - lets you track all the information about your current customers.
    

This workflow is also maintained when working with SOAP web services. The Stage field indicates whether the customer is a lead, prospect or customer as defined above. For example, if a customer record is defined as a Lead by SOAP web services and then that customer record has an opportunity record associated with it by SOAP web services, the customer record Stage field will automatically be updated to reflect the new prospect stage. After the opportunity record is updated to Closed-Won, the record Stage field is automatically updated to Customer. To enter a new customer record at a specified stage, set the Stage field to Lead, Prospect or Customer as desired.

Note:

In SOAP web services the entityID field of a Customer record is by default an Inline Field Type (read-only). If you try to set the entityID when adding a new Customer, you will receive an error message. To avoid the error message, you should not set a value for the entityID field. If you need to enter an entityID, you must enable the Allow Override option for it in _Setup > Company > Setup Tasks > Auto-Generated Numbers_. For more information, see [Overwrite Entity and CRM Record Type Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4340447524.html).

## Customer Status and Stage Internal IDs {#bridgehead_N3640460}

The following table lists the internal IDs for all standard Customer Status and Stage values that can be used to populate the entityStatus or stage field.

Note:

In addition to the following standard custom status values, your organization may have defined _custom_ Customer Status values. If the Show Internal IDs preference is enabled, you can confirm the internal ID values in the associated list. For more details, see [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html)

| Customer Statuses |  | Customer Stages |
| --- | --- | --- |
| ID | Status |  | ID | Stage |
| --- | --- | --- | --- | --- |
| 17 | Dead |  | LEAD | Lead |
| 6 | New |  | PROSPECT | Prospect |
| 18 | Qualified |  | CUSTOMER | Customer |
| 14 | Closed Lost |  | \- | \- |
| 9 | Identified Decision Makers |  | \- | \- |
| 8 | In Discussion |  | \- | \- |
| 11 | In Negotiation |  | \- | \- |
| 7 | Opportunity Identified |  | \- | \- |
| 10 | Proposal |  | \- | \- |
| 12 | Purchasing |  | \- | \- |
| 13 | Closed Won |  | \- | \- |
| 16 | Lost Customer |  | \- | \- |
| 15 | Renewal |  | \- | \- |

## Returning a Contact List for a Customer {#bridgehead_N3641393}

To return a list of contacts associated to a specific customer record, you must first get the customer record and then perform a search for the contacts associated to that customer.

**Sample Java Code**

          `// First get your customer  Customer c = (Customer)port.get(new RecordRef("17",RecordType.customer)).getRecord();   // Now do a specific search for the Contacts  ContactSearch cts = new ContactSearch();   // Search for an exact match between Customer.EntityId and the ContactSearch Field Company.cts.setCompany(new SearchStringField(c.getEntityId(),SearchStringFieldOperator.is));   // Execute the search and you have your contactlist.  SearchResult scts = port.search(cts);` 
        

## Working with Customer Sublists {#bridgehead_N3641457}

The SOAP Schema Browser includes all sublists associated with the customer record. See the following information for usage notes regarding specific customer sublists. Usage notes are not provided for every sublist type.

-   [CustomerContactRoleList](#bridgehead_N3641610)
    
-   [CustomerCreditCardsList](#bridgehead_N3641660)
    
-   [CustomerCurrencyList](#bridgehead_N3641673)
    
-   [CustomerAddressbookList](#bridgehead_N3641702)
    
-   [CustomerSalesTeamList](#bridgehead_N3641735)
    
-   [CustomerDownloadList](#bridgehead_N3641748)
    
-   [SubscriptionsList](#bridgehead_N3641762)
    
-   [Tax Registrations Sublist](#bridgehead_1544450444)
    

For general information about working with sublists in SOAP, see [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html).

## CustomerContactRoleList {#bridgehead_N3641610}

This sublist is available for updates of customer records only. You can update this sublist's data to provide Customer Center access to contacts. You can provide access to contacts that already exist in NetSuite and that have already been attached to a customer that already exists in NetSuite. You cannot use this sublist to attach new contacts. The workflow is as follows: 1) Add customer. 2) Add contacts. 3) Attach contacts to customer. 4) Update customer with contact access information with this sublist.

The fields in this sublist map to the fields on the Access subtab in the UI. These fields include:

-   A Boolean field that indicates whether a contact has access to NetSuite
    
-   A field that indicates whether new notification emails are sent when access changes are made
    
-   A field that indicates whether the password is manually assigned or changed
    
-   A contact name key field
    
-   The email address and password used to log in to NetSuite
    
-   The NetSuite role (Partner Center)
    

Operations on this sublist do not preserve row order. In some cases, rows added to the sublist will not be returned in the same order.

Note:

As of the 2011.2 endpoint, the CustomerContactList sublist is no longer supported. You can use the CustomerContactRoleList instead. In addition, you can add or update contacts through the attach/detach operations, and you can retrieve contact names and roles for an entity through an advanced search on the entity record and its associated contacts. This advanced search technique is described in [Returning a Contact List for a Customer](#bridgehead_N3641393).

## CustomerCreditCardsList {#bridgehead_N3641660}

The creditCardsList field is a list field that lets you provide multiple credit card entries for a customer. The customer can then use these entries for payments. These fields are all mapped to the Financial subtab in the UI.

When working with credit card data, be aware of the following security features:

-   When adding a credit card, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## CustomerCurrencyList {#bridgehead_N3641673}

This list enables you to define multiple currencies that can be used for a customer's transactions, in addition to the primary currency set for a customer. This list is available when the Multiple Currencies feature is enabled. For details about using this feature, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

This list's Currency field maps to the Currency field on the Currencies subtab on the Financial subtab of the standard customer record in the UI.

## CustomerAddressbookList {#bridgehead_N3641702}

The addressBookList field is a list field that lets you provide multiple addresses for a customer. These fields are all mapped to the Address subtab in the UI.

When you work with the addressbookList on customer records in the 2009.2 endpoint and beyond, be sure to use **internalId** as the key. Do not use **label**. For the 2009.1 and lower endpoints, the addressbookList is not a keyed sublist, but you can use label to identify records.

Important:

Sales territory assignments are based on customers' default billing addresses. If you do not set defaultBilling to True for a customer address, it is not assigned to a territory automatically.

## CustomerSalesTeamList {#bridgehead_N3641735}

This list is only available when the Team Selling feature is enabled.

## CustomerDownloadList {#bridgehead_N3641748}

The Sell Downloadable Items feature must be enabled in an account to provide downloads for customers in the Customer Center.

## SubscriptionsList {#bridgehead_N3641762}

The subscriptionsList sublist on the customer record can be updated. Use the replaceAll flag to update specific lines in this sublist, using **subscription** as the key. Be aware that SOAP web services updates to this sublist follow the logic that is permitted in the NetSuite UI. After an entity is unsubscribed from a category, only the entity itself can re-subscribe.

## Tax Registrations Sublist {#bridgehead_1544450444}

The tax registrations sublist is available when the SuiteTax feature is enabled at _Setup > Company > Setup Tasks > Enable Features_, on the Tax subtab.

Whenever you change the Tax Registration Number value on a sublist line, it triggers the regeneration of the value of a hidden ID field, and the values of ID fields are regenerated on all sublist lines. The ID field is hidden in the UI, but it is visible through SOAP web services. The ID field is searchable, so you can access the updated values through SOAP web services.

For information about working with tax registration in the UI, see [Assigning Tax Registrations to an Entity in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4513820587.html).

### Related Topics

-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3639664.html)
-   [Entity Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3650214.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
