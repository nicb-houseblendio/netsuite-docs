---
id: "chapter_N3924743"
type: "chapter"
title: "CSV Import FAQ"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > CSV Import FAQ"
parent: "book_4470700566"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3924743.html"
anchors: ["question_N3925311", "question_N3925466", "question_N3925636", "question_N3925736", "question_N3925880", "question_N3925980", "question_N3926068", "question_N3926210", "question_N3926457", "question_N3926559", "question_N3926659", "question_N3926804", "question_N3926948", "question_N3927025", "question_N3927172", "question_N3927355", "question_N3927478", "question_N3927650", "question_N3927815", "question_N3927950", "question_N3928041", "question_N3928118", "question_N3928270"]
sha256: "68466726915a6a38f247c8b72174c17bd6e2531ded6d09bc2af031911c077842"
---

See the questions and answers below for information about CSV Import.

### Can I use the Import Assistant for all data imports into NetSuite? {#question_N3925311}

The Import Assistant works with most commonly imported record types and is the best way to move small to medium-sized data sets from other applications into NetSuite. For information about record types that the Import Assistant supports, see [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html).

NetSuite REST and SOAP Web Services import tools are another option for record types that CSV import doesn't support, or for big or ongoing data migrations. For information, see the SOAP Web Services Platform Guide.

NetSuite also supports specialized imports. See [Importing a Peachtree CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N463422.html).

Related Topics

-   [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html)
    

### What is the preferred order for importing data into NetSuite? {#question_N3925466}

The following order is preferred for data imports:

1.  Chart of Accounts
    
    Note that you should enter opening balances as journal entries on 'go live', using the specialized journal entry import process. See [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html).
    
2.  Classifications
    
    Departments, Classes, Locations - supported by Import Assistant
    
3.  Entities
    
    Employees, Vendors, Partners, Customers (including Leads, Prospects, and Customers), Contacts - supported by Import Assistant
    
4.  Items
    
    Assembly/BOM Item, Lot Numbered Assembly/BOM Item, Serialized Assembly/BOM Item, Inventory Item, Lot Numbered Inventory Item, Serialized Inventory Item, Kit/Package Item, Non-Inventory Item for Sale, Non-Inventory Item for Resale, Non-Inventory Item for Purchase, Service Item for Sale, Service Item for Resale, Service Item for Purchase, Other Charge Item for Sale, Other Charge Item for Resale, Other Charge Item for Purchase - supported by Import Assistant
    
5.  CRM Records
    
    Notes, Issues, Solutions, Topics - supported by Import Assistant
    
    Cases, Events, CRM Tasks, Messages - not yet supported, need another method
    
6.  Transactions
    
    Cash Sales, Customer Payments, Estimates, Invoices, Opportunities, Purchase Orders, Sales Orders, Vendor Bills, Vendor Payments - supported by Import Assistant
    
    Credit Memos, Return Authorizations - not yet supported, need another method
    

Related Topics

-   [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### How do I set up a CSV file for use by the Import Assistant? {#question_N3925636}

The Import Assistant imports by record type, so place data for each type in its own CSV file.

First, export your data from your current app to a CSV file. Then, you might need to add columns that NetSuite requires. You can see which fields you need and set default values for them on the Import Assistant's Field Mapping page.

To get the most out of the Import Assistant's automatic mapping, change your CSV column names to match NetSuite field names. You can find these names on the Field Mapping page.

It's a good idea to include unique IDs from your current app in the CSV, rename the column to 'External ID,' and import those into NetSuite. These IDs help uniquely identify each record and can be used as primary keys for matching and linking.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### What is sublist data and how do I import it? {#question_N3925736}

Most records in NetSuite include sublists. Each record's sublist can include a list of references to other records. For example, a transaction record can include an items sublist, and a customer record can include an address sublist.

The Import Assistant enables you to import sublist data at the same time that you import other record type data. For more information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).

On the first page of the Import Assistant, you can choose whether to use a single file or multiple files to import data. If you choose to use a single CSV file, this one file includes all sublist data as well as other record type data. If you choose to use multiple CSV files, the Import Assistant enables you to specify a primary file for record type data and separate files for each sublist. See [Select a File for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344348.html).

Sublist data fields are listed at the bottom of the Import Assistant Field Mapping page, within separate folders for each sublist. You can click the add new button (+) to the right of the sublist folder name to add instances of the sublist to be imported. You need to map sublist fields on this page for sublist data to be imported. See [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html).

Import Assistant updates of sublist data vary according to whether sublists are keyed or non-keyed. Keyed sublists have individual sublist lines that can be searched for and updated.

Related Topics

-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### Why is my import job processing so slowly? {#question_N3925880}

Your import might be slow if you run it at a busy time or if it has a lot of records.

You can save your import to run later. See [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html).

You should break up big CSV files into smaller ones and import them as separate jobs to speed things up. There's a 25,000 record limit per file, but making your files even smaller can help the imports run faster.

If you import project or employee entry data, you can also enable the Asynchronous Project Plan Recalculation preference at _Setup > Company > General Preferences_. For more information, see [Asynchronous Project Plan Recalculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html#bridgehead_4532423110).

Related Topics

-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### Where are email messages regarding a CSV import job sent? {#question_N3925980}

Email notifications about the status of a CSV import job, including information about post-processing errors, go to the email address used to log in to the session that initiated the import job.

For example, if you log in as jsmith@companyx.com and start an import, you'll get all related email notifications at that address.

Related Topics

-   [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html)
    
-   [CSV Import Error Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    

### Are there any special requirements for importing data into OneWorld accounts? {#question_N3926068}

If you're using NetSuite OneWorld, set up your subsidiaries in NetSuite before you start importing data. For instructions, see [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html).

For NetSuite OneWorld accounts, the Subsidiary field is a required field for the following record types: Chart of Accounts, Contacts, Customers, Employees, Jobs (Projects), Leads, Partners, Prospects, and Vendors. For imports of these record types, you must include in your CSV file a field that can be mapped to the NetSuite Subsidiary field, and map this field on the Import Assistant Field Mapping page. If you try to import or update records without a subsidiary, the import will fail.

CSV file values for subsidiaries should be hierarchical names, in the format **grandparent : parent : child**, for example, **Consolidated Parent Company : UK Subsidiary : Euro Subsidiary**.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [OneWorld Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N266701.html)
    
-   [Set up NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268052.html)
    
-   [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html)
    

### How can I use the Import Assistant to update existing NetSuite records? {#question_N3926210}

To update records with the Import Assistant, select either the **Update** or the **Add or Update** data handling option on the Import Options page. See [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html).

Your CSV file should include data for a primary key field that can be used to match CSV file records with existing NetSuite records and correctly update them.

-   For best results, use the Internal ID field as the primary key, include a column of NetSuite Internal ID values in your CSV file, and map this column to the Internal ID field.
    
    You can get Internal IDs by running a saved search in NetSuite with Internal ID as a results column, then export the results to CSV. For instructions on how to do this for transactions, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).
    
-   If you don't have Internal IDs, use External ID as the primary key, add a column of unique IDs to your CSV and map it to the External ID field.
    
    If your external source application has unique identifiers, place them in a column called External ID in your CSV.
    
    External ID values aren't visible or editable in the NetSuite UI, but you can change them with CSV import, SuiteScript, SOAP or REST Web Services, and you can get them in saved searches.
    
-   The last possibility is to use a name field as a primary key.
    
    This option is not preferred, as name formatting can be complex, and key matching for updates can be difficult and error-prone if CSV file name values are formatted incorrectly.
    
    For example, customer names are mapped to the Customer ID field and should have the format **Parent : Child**, such as **ABC Medical : A1 Bandages**.
    
    Also, for names that contain spaces, HTML rendering can sometimes distort the number of spaces included, causing mismatches between CSV file values and existing records, that result in import errors. To verify the number of spaces in names, you can create a saved search with a list of names and export it.
    

The info above is for updating body fields. Sublists have their own key fields you need to use for updates, but not all sublists can be updated this way; only a subset of the sublists supported for import are keyed.

When updating data, pay attention to the Advanced Options, Overwrite Missing Fields and Overwrite Sublists. See [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html). Also, make sure you know how sublist data gets updated.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
    

### Why does my import keep returning invalid reference key errors? {#question_N3926457}

These errors usually pop up when you use names instead of internal or external IDs as the primary key or reference type, and some names in your CSV don't match what's already in NetSuite.

Using names as primary keys or reference types is not preferred, as name formatting can be complex, and matching for updates can be difficult and error-prone if CSV file name values are formatted incorrectly. For example, customer names are mapped to the Customer ID field and should have the format **Parent : Child**, such as **ABC Medical : A1 Bandages**.

Also, for names that contain spaces, HTML rendering can sometimes distort the number of spaces included, causing mismatches between CSV file values and existing records, that result in import errors. To verify the number of spaces in names, you can create a saved search with a list of names and export it.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)
    

### Should I import account balances as part of the Chart of Accounts import? {#question_N3926559}

You should not include account balances as part of your Chart of Accounts import. This import should include account numbers, names, and descriptive information like type, description, and currency.

Since the Chart of Accounts is the foundation for all your company data, do this import first when setting up your account. Don't import account balances until you're ready to go live.

You can use the NetSuite journal entry import process to import balances as journal entries. This import uses a template rather than the Import Assistant. See [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Chart of Accounts Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N357847.html)
    

### How do I create template files for CSV imports? {#question_N3926659}

You do not need to create template files for CSV import, as the Import Assistant is not template-based. You can use any CSV file for an import; you do not need to start with a template file provided by NetSuite.

If you want to set up your own standard CSV file columns for particular record type imports, you can obtain information about NetSuite fields to which you can map CSV file fields in the following ways:

-   Walk through the Import Assistant for an import of the selected record type and review the fields listed in the NetSuite Fields pane on the Field Mapping page. You can use these field names as column names in your CSV file to facilitate automatic mapping.
    
-   Another way to understand these fields is to review carefully the form in the NetSuite user interface for the selected record type. You can click each field label to get help that describes each field.
    
-   For more descriptions of fields, review the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html) for details about fields for each record type. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).
    
-   Be aware that, by default, mappable NetSuite fields are those available on your preferred form for the selected record type. Fields can be mapped for the import job if they are displayed (not hidden) and not disabled on your preferred form. For example, when you import customer records, the fields that you can map to be imported are those that you can edit on the NetSuite customer form.
    
    If these fields do not include all of the data you want to import, for some record types, you can specify a custom form that includes the fields you need, as an Advanced Option in the CSV Import Assistant. This specification changes the NetSuite fields listed on the Field Mapping page. See [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).
    

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
    

### How do I complete an import if my CSV file does not include values for a required field? {#question_N3926804}

Required NetSuite fields are marked as (Req) on the Field Mapping page and usually are automatically placed in the center pane to remind you to map them. If you don't map all required fields, you can't move past this page.

If you do not have any values to import for a required field, you can do one of the following:

-   Include a column with blank values in your CSV file and map this column to the required NetSuite field.
    
-   Click the edit icon next to the required field and set the value for the required field to be NULL.
    
-   Click the edit icon next to the required field and select a default value for the required field. (This is possible only if values are set up in NetSuite).
    

Note:

You do not need to map required fields for a sublist unless you are importing data for the sublist. See [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html)
    
-   [Assign Null Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350094.html)
    

### What is a reference type? {#question_N3926948}

A reference type lets you map a column in your CSV to a NetSuite field that has list values, like dropdowns or multi-selects. You set reference types on the Field Mapping page by clicking the edit icon next to a mapped dropdown or multi-select field See [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### Can I use the Import Assistant to import pricing data for items? {#question_N3927025}

The Import Assistant lets you import item pricing data, including multiple price levels, quantity-based pricing, quantity pricing schedules, and multiple currencies. You can only import pricing data if one or more of the following related features are enabled: Multiple Prices, Quantity Pricing, and Multiple Currencies.

-   You should import multiple files, rather than a single file for item pricing, with pricing data in a separate file from other item data. For more information, see [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html).
    
-   Preferred column headers for item pricing CSV files vary, depending on whether you plan to upload a single file or multiple files. For more information, see [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html).
    
-   Pricing data can be selectively updated based on key field values. The key fields depend upon the pricing-related features that are enabled. For information, see [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html).
    

For more information, see [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    

### Why is the Individual field required for an import of customers, when all of my customers are companies, not individuals? {#question_N3927172}

NetSuite lets you set each customer, partner, or vendor as either an individual (person) or a company. The Field Mapping page always includes an Individual field for these, and it's required.

-   The Individual field is a Boolean indicating whether the entity is a company or a person.
    
-   It corresponds to the Type option buttons on the user interface forms for customers, partners, and vendors.
    
-   Unlike most radio button fields, an import of this field's data accepts all forms of True or False. For example, the following values are acceptable as a 'True' value: True, true, TRUE, T, yes, Yes, YES.
    
    -   True means it's an individual; False means it's a company.
        
    -   The Company Name field is required if the value kn the Individual field is False, but not if it's True.
        
-   You can set a default value for the Individual field by clicking its edit icon on the Field Mapping page. In the Default Value popup: choose Yes to default customer type to individual, choose No to default customer type to company.
    

Note:

Your account's settings for the Default Customer Type, Default Partner Type, and Default Vendor Type fields, at _Setup > Company > General Preferences_, may affect the value of the Individual field for imports.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Customers Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html)
    
-   [Partners Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N388987.html)
    
-   [Vendors Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N390628.html)
    

### What values should I import for the Global Subscription Status field for customers? {#question_N3927355}

The **Global Subscription Status** field on customer records determines whether a customer can receive email sent through campaigns and email merge operations.

-   There are four possible values: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but you can only set the soft values during import.
    
-   If you want to send campaign email to a customer, set this field's value to Soft Opt-In, because you cannot sent campaign email to users with Soft Opt-Out status, only opt-in email.
    
-   If you do not include this field in an import, its value is set based on the Unsubscribed to Marketing By Default option at Setup > Marketing > Marketing Preferences. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

Note:

The Global Subscription Status field replaces the previously used Unsubscribed field and enhances on its functionality.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Setting Up Campaign Subscriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995376.html)
    

### What is the difference between leads, prospects, and customers imports? {#question_N3927478}

When you import Lead, Prospect, or Customer data, it all goes into the Customer record in NetSuite. The Stage field shows whether it's a Lead, Prospect, or Customer. Leads can become Prospects, and Prospects can become Customers.

Specifically:

-   **Lead**: Lets you track everything you need to turn a lead into a customer. Leads don't have estimates, opportunities, or transactions. If you create an estimate or opportunity for a lead, it becomes a prospect. If you create a sales transaction, it becomes a customer.
    
-   **Prospect**: Lets you track everything you need to turn a prospect into a customer. Prospects don't have sales orders, invoices, or other sales transactions, but they can have opportunities and estimates. If you create a sales transaction or close an opportunity, the prospect becomes a customer.
    
-   **Customer**: Lets you track all the information about your current customers.
    

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Customers Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html)
    
-   [Leads Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N386282.html)
    
-   [Prospects Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N389753.html)
    

### Should I import customers and contacts together or separately? {#question_N3927650}

The Import Assistant lets you import customers (leads, prospects, or customers) and contacts separately or together.

Setting up files for importing customers and contacts together can be complex. For instructions for importing customers and contacts together, see [Importing Entities and Contacts Together](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html). For information about how data is processed for these types of imports, see [Import Job Processing for Entities and Contacts Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html#bridgehead_N392616).

You may find it simpler to import contacts and customers separately. For tips on how to do this, see [Contacts Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383204.html). Especially review [Importing Contacts for Existing Entity Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383204.html#bridgehead_N383527) and [Importing Contacts and New Entities Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383204.html#bridgehead_N383540).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Customers Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html)
    
-   [Leads Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N386282.html)
    
-   [Prospects Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N389753.html)
    

### Can I use the Import Assistant to import project data? {#question_N3927815}

The Jobs import, a Relationships type import, lets you import core project data and project resource data into NetSuite. See [Projects (Jobs) Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N385885.html).

There's also a simpler Import Assistant for importing project tasks from Microsoft Project. See [Project Tasks Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N438898.html).

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
    

### What is the difference between the following advanced options: Overwrite Sublists and Overwrite Missing Fields? {#question_N3927950}

Both options apply to updates and are disabled by default, but one works at the sublist level and the other at the field level.

Overwrite Sublists applies to all data in sublists with mapped fields. When enabled, CSV file data for any sublists with mapped fields completely replaces any existing sublist data in NetSuite. If disabled, CSV file sublist data either selectively updates or appends to existing sublist data.

Overwrite Missing Fields works at the field level. When enabled, any mapped CSV file fields with null values overwrite existing data in NetSuite fields, blanking it out.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html)
    

### Why didn't my CSV import job that created new records trigger my workflow based on record creation or update? {#question_N3928041}

If a workflow is triggered when you create or update records in the NetSuite user interface, but is not triggered when a CSV import job creates or updates records, you probably need to enable the **Run Server SuiteScript CSV and Trigger Workflows** preference when performing the import. Workflows are treated as server-side SuiteScript, so they do not run if this preference is not enabled.

You enable this preference for the current import on the Advanced Options of the Import Assistant. Go to _Setup > Import/Export > Import Tasks > Import CSV Records_. On Step 2 of the Import Assistant, in the Advanced Options, check the Run Server SuiteScript and Trigger Workflows box. If the box is unavailable, you do not have permission to change the setting for the import, and the company setting will apply.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Setting CSV Import Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html)
    

### How can I import Price Level for transaction line items? {#question_N3928118}

On the Field Mapping page of the CSV Import Assistant, expand the Items folder in the NetSuite Fields pane on the right side. Double-click the Price Level field to display it in the middle pane.

You should include a Price Level column (with values) in your CSV file that can be mapped to the NetSuite Price Level field. If you are unable to add this column, you can still map the Price Level field on the Field Mapping page, and then click the edit icon and select Custom as the default value. However, this default is not guaranteed to be a valid level for all items.

Important:

If you do not map the Price Level field for a CSV import, the base price from each item record is used as the price for each transaction line item. This behavior is consistent with the behavior when you add transaction line items in the user interface.

Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    
-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)
    
-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
    

### How do I know what the number is for an imported journal entry? {#question_N3928270}

There are two methods for journal entry: a simple method you can use to import one journal entry at a time, and a more involved method you can use to import multiple journal entries.

If you use the simple method, available at Transactions > Financial > Make Journal Entries > Import, you do not have to provide the number for the journal entry in your CSV file. If you do not include this number, a default number is applied during the import process.

If you want to know the defaulted number for an imported journal entry, you can obtain it before you start the import from the View Mapping / Start Import page. Before you click the button to Run the import, do the following:

Click the Entry No. field in the right pane so that it appears in the center pane, then click its edit icon. The default value displays in the popup.

If you are importing multiple journal entries, you need to provide numbers in your CSV file.

### Related Topics

-   [CSV Imports Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N342646.html)
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Additional Import and Export Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N463253.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
