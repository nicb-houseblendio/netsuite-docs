---
id: "section_N439528"
type: "section"
title: "Supported Sublist Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Sublist Data Import > Supported Sublist Imports"
parent: "section_N439392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html"
anchors: []
sha256: "55a504e960fefe8afb681b5768f8acce63aad800f2821680b6e10e36377925b3"
---

The following table shows the sublists for which you may be able to add or update data through CSV imports. These sublists depend upon the features enabled in your account. You can see the sublists available in your account for a particular record type on the Import Assistant's Field Mapping page.

Note:

Some related data may be structured as a subrecord rather than as a sublist of a record type. If you don't see a sublist in the table below, see [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html) to check if the data is set up as a subrecord instead.

| Record Type | Sublist | Notes |
| --- | --- | --- |
| **Accounting: Chart of Accounts** | Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
|  |  |  |
| **Accounting: Expense Categories** | Rates | Sublist available to OneWorld accounts only. Selectively updatable based on the Subsidiary field. |
|  |  |  |
| **Accounting: Price Book** | Price Book Lines | When SuiteBilling feature enabled. Selectively updatable based on the Subscription Plan Line field. |
|  |  |  |
| **Accounting: Price Plan** | Pricing | When SuiteBilling feature enabled. Selectively updatable based on the Above Quantity field. |
|  |  |  |
| **Activities: Events** | Attendees | Selectively updatable based on the Attendee field. |
| \- | Resources | Selectively updatable based on the Resource field. For more information, see [Event CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3757027142.html). |
| \- | Time Track | \- |
|  |  |  |
| **Activities: Phone Calls** | Contacts | Selectively updatable based on the Participant or Contact key field. |
| \- | Time Tracking | When Time Tracking feature enabled. |
|  |  |  |
| **Activities: Tasks** | Contacts | Selectively updatable based on the Company/Project or Contact key field. |
|  | Time Tracking | When Time Tracking feature enabled. |
|  |  |  |
| **Classification: Class** | Class Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
|  |  |  |
| **Classification: Department** | Department Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
|  |  |  |
| **Classification: Location** | Location Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
|  |  |  |
| **Classification: Merchandise Hierarchy Node** | Hierarchy Versions | The **Included in Version** box on the Hierarchy Versions subtab indicates if the hierarchy node is assigned to a hierarchy version. You can assign a node to multiple versions. |
|  |  |  |
| **Custom Records: Translations** | Translations | When Multi-Language feature is enabled. |
|  |  |  |
| **Customization: Custom Lists** | Custom List Values | Selectively updatable based on the ID field. For more information, see [Custom List CSV Multiple File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N365834.html). |
| \- | Custom List Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
|  |  |  |
| **Employees: Employees** | Payroll Accrued Times | Selectively updatable based on the Payroll Item key field. When Payroll feature enabled. |
| \- | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Payroll Contributions | Selectively updatable based on the Payroll Item key field. When Payroll feature enabled. |
| \- | Payroll Deductions | Selectively updatable based on the Payroll Item key field. When Payroll feature enabled. |
| \- | Direct Deposit | Selectively updatable based on the Internal ID key field. When Direct Deposit feature enabled. |
| \- | Payroll Earnings | Selectively updatable based on the Payroll Item key field. When Payroll feature enabled. |
| \- | Education | \- |
| \- | Emergency Contacts | \- |
| \- | Roles | \- |
| \- | Subscriptions | Selectively updatable based on the Subscriptions key field. |
|  |  |  |
| **Employees: Expense Reports** | Expenses | Available when Expense Reports feature is enabled. Selectively updatable based on the Line Id or Ref No. field. For more information, see [Expense Report CSV Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746675443.html). |
| \- | Accounting Book Detail | Available when the Multi-Book Accounting feature is enabled, and when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Items** | Bin Numbers | When Bin Management or Advanced Bin/Numbered Inventory Management feature enabled. Selectively updatable based on the Bin Number key field. For Assembly/BOM Item and Inventory Item imports. Note: If you're importing bin records, complete this import before you import items with associated bin numbers. See [Bin Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394777.html). |
| \- | Locations | When Multi-Location Inventory feature enabled. Selectively updatable based on Internal ID, External ID, or Location. For Assembly/BOM Item and Inventory Item imports. For more information, see [Updating Locations on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html#bridgehead_N372898). |
| \- | Members | For Assembly/BOM Item, Item Group, and Kit/Package Item imports. |
| \- | Merchandise Hierarchy | For Inventory Items, Lot Numbered Inventory Items, and Serialized Inventory Items. Available when the Merchandise Hierarchy feature is enabled. |
| \- | Pricing | When Multiple Prices, Quantity Pricing, or Multiple Currencies features are enabled. Selectively updatable based on Currency, Quantity, and Level fields, depending on enabled features. (See [Keys for Item Pricing Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html#bridgehead_N377525).) |
| \- | Related Items | When Web Site feature enabled. Not available for Non-Inventory Item for Purchase, Service Item for Purchase, or any Other Charge Item imports. For more information, see [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html). |
| \- | Site Category | When Web Site feature enabled. Not available for Non-Inventory Item for Purchase, Service Item for Purchase, or any Other Charge Item imports. For more information, see [Site Category Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433181.html). |
| \- | Task Templates | When Project Management feature enabled. For Service Item for Sale imports. |
| \- | Translations | When Multi-Language feature enabled. Selectively updatable based on the Language key field. |
| \- | Vendors | When Multiple Vendors feature enabled. Selectively updatable based on the Vendor. For Inventory Item, Non-Inventory Item for Resale or Purchase, Service Item for Resale or Purchase, and Other Charge Item for Resale or Purchase imports, and Assembly/BOM Item when Allow Purchase of Assembly Items preference is enabled. For more information, see [Updating Vendors on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html#bridgehead_N372857). |
|  |  |  |
| **Items: Subscription Plan** | Subscription Plan Members | When SuiteBilling feature enabled. |
|  |  |  |
| **Relationships: Contacts** | Address | Selectively updatable based on Internal ID or Label key field. Available for Contacts Only imports. Not available for Customers and Contacts Together, Leads and Contacts Together, or Prospects and Contacts Together imports. |
| \- | Subscriptions | Selectively updatable based on Subscription key field. |
|  |  |  |
| **Relationships: Customers** | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Contact Access | Available for updates of existing customers only, to add or update NetSuite access information for existing customer contacts. Selectively updatable based on the Contact key field. |
| \- | Credit Cards | Addition of new records is supported; update of existing lines isn't supported. |
| \- | Currencies | When Multiple Currencies feature enabled. For more information, see [Setting Multiple Transaction Currencies for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385568). |
| \- | Downloads | When Sell Files feature enabled. |
| \- | Group Pricing | When Multiple Prices feature enabled. |
| \- | Item Pricing | When Multiple Prices feature enabled. |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
| \- | Subscriptions | Selectively updatable based on Subscription key field. |
| \- | Tax Registrations | Available when the SuiteTax feature is enabled. |
|  |  |  |
| **Relationships: Groups** | Group Members | Can be updated using Internal ID, External ID or Names key field for the group member. |
|  |  |  |
| **Relationships: Jobs** | Address | When Project Management feature disabled. Selectively updatable based on the Internal ID or Label key field. |
| \- | Resource | When Project Management feature enabled. |
|  |  |  |
| **Relationships: Leads** | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Credit Cards | Addition of new records is supported. Update of existing lines isn't supported. |
| \- | Downloads | When Sell Files feature enabled. |
| \- | Group Pricing | When Multiple Prices feature enabled. |
| \- | Item Pricing | When Multiple Prices feature enabled. |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
|  |  |  |
| **Relationships: Partners** | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Contact Access | Available for updates of existing partners only, to add or update NetSuite access information for existing partner contacts. Selectively updatable based on the Contact key field. |
| \- | Promotion Codes | \- |
| \- | Subscriptions | Selectively updatable based on the Subscription key field. |
| \- | Tax Registrations | Available when the SuiteTax feature is enabled. |
|  |  |  |
| **Relationships: Prospects** | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Credit Cards | Addition of new records is supported. Update of existing lines isn't supported. |
| \- | Downloads | When Sell Files feature enabled. |
| \- | Group Pricing | When Multiple Prices feature enabled. |
| \- | Item Pricing | When Multiple Prices feature enabled. |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
|  |  |  |
| **Relationships: Vendors** | Address | Selectively updatable based on the Internal ID or Label key field. |
| \- | Roles | \- |
| \- | Subscriptions | Selectively updatable based on the Subscription key field. |
| \- | Tax Registrations | Available when the SuiteTax feature is enabled. |
|  |  |  |
| **Rules Setup: Foreign Currency Variance Posting Rule** | Criteria | Available when the Foreign Currency Variance Mapping feature is enabled. |
|  |  |  |
| **Supply Chain: Bill of Materials Revision** | Bill of Materials Revision Components | Available when the Advanced Bill of Materials feature is enabled. |
|  |  |  |
| **Supply Chain: Manufacturing Cost Template** | Cost Detail | At least one line item is required for new records. (See [Cost Template Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N396186.html).) |
|  |  |  |
| **Supply Chain: Manufacturing Routing** | Routing Steps | Selectively updatable based on the Operation Sequence key field. At least one line item is required for new records. (See [Routing Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N400811.html).) |
| \- | Component per Operation | \- |
|  |  |  |
| **Support: Solutions** | Solutions | \- |
| \- | Topics | \- |
|  |  |  |
| **Support: Support Cases** | Escalate to | \- |
|  |  |  |
| **Transactions: Advanced Intercompany Journal Entry** | Advanced Intercompany Journal Entry Line | Each imported intercompany journal entry must include at least 4 lines, with one debit and one credit each for originating and receiving subsidiary. Line debits and credits must balance. For more information, see [Advanced Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498465157.html). |
|  |  |  |
| **Transactions: Cash Sale** | Auth. Code | When Gift Certificates feature enabled. |
| \- | Billable Time | Selectively updatable based on related transaction ID (\*\*\*doc). |
| \- | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one line item is required for new records. (See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690).) |
| \- | Partners | When Team Selling feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
| \- | Shipment | When Multiple Shipping Routes feature enabled. |
|  |  |  |
| **Transactions: Check** | Accounting Books | When Multi-Book Accounting feature is enabled, and when more than one active accounting book exists. |
| \- | Expenses | Selectively updatable based on Line. |
| \- | Items | Selectively updatable based on Item. |
| **Transactions: Credit Card Charge** | Accounting Books | When Multi-Book Accounting feature is enabled, and when more than one active accounting book exists. Selectively updatable based on Line or Order Line. |
| \- | Expenses | Selectively updatable based on Line. |
| \- | Items | Selectively updatable based on Item. |
|  |  |  |
| **Transactions: Credit Card Refund** | Accounting Books | When Multi-Book Accounting feature is enabled, and when more than one active accounting book exists. Selectively updatable based on Line or Order Line. |
| \- | Expenses | Selectively updatable based on Line. |
| \- | Items | Selectively updatable based on Item. |
|  |  |  |
| **Transactions: Credit Memo** | Apply | For more information, see [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html). |
| \- | Items | For more information, see [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html). |
|  |  |  |
| **Transactions: Custom Transaction** | Accounting Books |  |
| \- | Lines | When Custom Transactions feature is enabled and at least one custom transaction type is created. Selectively updatable based on the Line and Account fields. Note that the Account field can be used as the key only when every line in the sublist has a unique value in the Account field. This behavior differs from SOAP web services, where you can use only Line as a key, even when every line has a unique Account value. For more information, see [Custom Transaction CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4271206853.html). |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Customer Payment** | Invoices | Selectively updatable based on the Invoice key field (and optionally Line key field). |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Estimate** | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one line item is required for new records. (See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690).) |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
| \- | Shipment | When Multiple Shipping Routes feature enabled. |
|  |  |  |
| **Transactions: Inbound Shipment** | Items | \- |
|  |  |  |
| **Transactions: Intercompany Journal Entry** | Intercompany Journal Entry Line | Each imported intercompany journal entry must include at least 4 lines, with one debit and one credit each for originating and receiving subsidiary. Line debits and credits must balance. For more information, see [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html). |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Inventory Cost Revaluation** | Cost Components | Available when Standard Costing feature is enabled. Selectively updatable based on the Component and Cost Category fields. |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Inventory Transfer** | Adjustments | \- |
| \- | Adjustments - Inventory Detail | Available with the Advanced Bin/Numbered inventory Management feature is enabled |
|  |  |  |
| **Transactions: Invoice** | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
| \- | Auth. Code | When Gift Certificates feature enabled. |
| \- | Billable Time | Selectively updatable based on related transaction ID (\*\*\*doc). |
| \- | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one line item is required for new records. (see [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690)) |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
| \- | Shipment | When Multiple Shipping Routes feature enabled. |
|  |  |  |
| **Transactions: Item Demand Plan** | Demand Planning | Fields vary according to type of demand plan: monthly, weekly, or daily. See [Demand Plan Sublist Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N415164.html). |
|  |  |  |
| **Transactions: Item Supply Plan** | Orders | \- |
|  |  |  |
| **Transactions: Journal Entry** | Journal Entry Line | Each imported journal entry must include at least 2 lines, with balancing debits and credits. For more information, see [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html). |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Opportunity** | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). |
| \- | Opportunity | \- |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
|  |  |  |
| **Transactions: Paycheck** | Contributions, Deductions, Earnings, Expenses, Taxes, Time | \- |

|  |  |  |
| --- | --- | --- |
| **Transactions: Period End Journal Entry** | Period End Journal Entry Line | \- |
|  |  |  |
| **Transactions: Purchase Order** | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one line item is required for new records. (See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690).) For more information, see [Purchase Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html). |
|  | Expenses | When Allow Expenses on Purchase Orders preference enabled. Expenses data must be in a separate CSV file. For more information, see [Purchase Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html). |
|  |  |  |
| **Transactions: Return Authorization** | Items | Selectively updatable based on Order Line or Item key field. |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Partner key field. |
| \- | Sales Team | When Team Selling feature enabled. Selectively updatable based on Employee key field. |
|  |  |  |
| **Transactions: Sales Order** | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
| \- | Auth. Code | When Gift Certificates feature enabled. |
| \- | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one line item is required for new records. (See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690).) |
| \- | Partners | When Multi-Partner Management feature enabled. Selectively updatable based on Internal ID, External ID, or Partner. |
| \- | Sales Team | When Team Selling feature enabled. |
| \- | Shipment | When Multiple Shipping Routes feature enabled. |
|  |  |  |
| **Transactions: Statistical Journal Entry** | Line | At least one line is required for new records (see [Statistical Journal Entry Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3983596075.html)). |
|  |  |  |
| **Transactions: Subscription** | Price Book Lines | When SuiteBilling feature enabled. |
|  |  |  |
| **Transactions: Subscription Change Order** | Subscription Change Order Items | When SuiteBilling feature enabled. Selectively updatable based on the Line Number field. |
|  |  |  |
| **Transactions: Transfer Order** | Accounting Books | \- |
| \- | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). |
|  |  |  |
| **Transactions: Vendor Bill** | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. selectively updateable based on the Accounting Book key field |
| \- | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one item line is required for new records (see [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690)). For more information, see [Vendor Bill Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N427250.html). |
| \- | Expenses | Expenses data must be in a separate file. For more information, see [Vendor Bill Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N427250.html). |
|  |  |  |
| **Transactions: Vendor Credit** | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one item line is required for new records (see [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690)). |
| \- | Expenses | Expenses data must be in a separate file. Selectively updatable based on the Line/Order Line key field. |
| \- | Apply | Apply data must be in a separate file. Selectively updatable based on the Apply or Line key field. |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Vendor Payment** | Bills | Selectively updatable based on the Bill key field (and optionally Line key field). |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Transactions: Vendor Return Authorization** | Items | Selectively updatable based on the Line/Order Line or Item key field (See [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)). At least one item line is required for new records (see [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690)). |
| \- | Expenses | Expenses data must be in a separate file. Selectively updatable based on the Line/Order Line key field. |
| \- | Accounting Book Detail | Available only when the Multi-Book Accounting feature is enabled, and only when more than one active accounting book exists. Selectively updateable based on the Accounting Book key field. |
|  |  |  |
| **Website: Site Category** | Presentation Items | \- |

### Related Topics

-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Sublist Data in a Single File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493384282.html)
-   [Multiline Sublists for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493796058.html)
-   [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html)
-   [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
