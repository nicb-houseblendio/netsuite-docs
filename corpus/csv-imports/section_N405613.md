---
id: "section_N405613"
type: "section"
title: "Transactions Import Type"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type"
parent: "chapter_N356211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html"
anchors: []
sha256: "c80260decef8bf4e37b80c44b57ca2fa44c6fb3010f71fc6b3120a7a66720ae1"
---

Transactions imports support the addition or update of data for some transaction subtypes. Processed lines for some transaction types contribute to the Monthly Transaction Lines metric that counts toward maximum limits for your NetSuite service tier. For more information, see [Transaction Types Included in Monthly Transaction Lines Metric](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160311737279.html).

The Import Assistant supports the following transaction subtype imports:

-   [Advanced Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498465157.html)
    
-   [Bin Putaway Worksheet Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0717090855.html)
    
-   [Bin Transfer Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0319121833.html)
    
-   [Cash Refund Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0304033212.html)
    
-   [Cash Sale Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N407231.html)
    
-   [Check Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529578227.html)
    
-   [Credit Card Charge Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676571596.html)
    
-   [Credit Card Refund Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676571713.html)
    
-   [Credit Memo Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N408112.html)
    
-   [Custom Transactions Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4174435473.html)
    
-   [Customer Payment Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N410731.html)
    
-   [Estimate Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411251.html)
    
-   [Inventory Details on an Inbound Shipment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158136489199.html)
    
-   [Inventory Adjustment Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4676544313.html)
    
-   [Inventory Cost Revaluation Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3743317066.html)
    
-   [Inventory Transfer Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314530899.html)
    
-   [Invoice Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N411794.html)
    
-   [Item Demand Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N414602.html)
    
-   [Item Fulfillment Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0220095644.html)
    
-   [Item Receipt Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0220100422.html)
    
-   [Item Supply Plan Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N417879.html)
    
-   [Journal Entry Import and Intercompany Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N418118.html)
    
-   [Opportunity Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N421452.html)
    
-   [Order Reservation Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163171739670.html)
    
-   [Paycheck Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498459867.html)
    
-   [Period End Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550160681.html)
    
-   [Purchase Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N423495.html)
    
-   [Return Authorization Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N425745.html)
    
-   [Sales Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N426302.html)
    
-   [Statistical Journal Entry Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3899783100.html)
    
-   [Transfer Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1529583019.html)
    
-   [Vendor Bill Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N427250.html)
    
-   [Vendor Credit Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N428672.html)
    
-   [Vendor Payment Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N429286.html)
    
-   [Vendor Prepayment Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159462844377.html)
    
-   [Vendor Return Authorization Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N429795.html)
    
-   [Work Order Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1221125458.html)
    

Be aware of the following:

-   You can import transaction data in a single CSV file, or in multiple files-for example, with transaction header data in one file and item-level data in other files. For imports of new data, you should include external ID values to uniquely identify transactions. For updates, you can use internal IDs for this purpose. The unique ID should be included in every line of the CSV files. Note that the transaction ID isn't unique.
    
-   Warning:
    
    The **One File to Upload** option can't be used to import transactions that use the tax details override option and include group items or subscriptions (including multiple items). If you need to import these kinds of transactions, you must use the **Multiple Files to Upload** option during CSV import.
    
-   By default the Field Mapping page for a transactions import includes the NetSuite fields from your preferred form for the selected record type. Fields can be mapped for the import job if they're displayed (not hidden) and not disabled on your preferred form. These default mappable NetSuite fields may not match the fields that you need to import; you may want to include fields available on another record type form.
    
    To ensure that the appropriate fields are available for mapping, you can change the selection for Custom Form, in the Advanced Options area of the Import Assistant's Import Options page. For more information, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).
    
-   If auto-generated numbering is enabled, transaction numbers can still be set if the Allow Override option is enabled.
    
-   To maintain performance, you shouldn't submit transactions with more than 5000 lines through CSV import. (For journal entries, this limit is 10,000 lines per transaction.)
    
-   To avoid errors with imported transaction address data, use short names for state fields and full names for country fields. A dropdown list of country names is available from the edit icon on the Field Mapping page, to be set as default country field values. See [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html) and [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html).
    
-   To import a transaction with multiple line items, use the same transaction number field for each line item.
    
-   You should import entities and items data before you import transactions data.
    
    -   To reference entities such as customers in transaction CSV files, use the number if auto-generated numbering is enabled; otherwise, use the customer name.
        
    -   Item references in transaction CSV files must match the spelling and case of the item names in your NetSuite account.
        
    -   Account references in transaction CSV files should be account names rather than numbers.
        
    -   For sub-customers, sub-items, and sub-accounts, use hierarchical parent : child references. For more information, see [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html).
        
-   Use entity account names and numbers when importing transactions, not the chart of accounts number.
    
-   For Cash Sale, Estimate, Invoice, Purchase Order, Sales Order, and Vendor Bill imports, Items data is required for imports of new records, but not for imports that update existing records. You don't need Items data for Opportunity imports, and it's not relevant for Customer Payment and Vendor Payment imports. See [Required Items Sublist Fields for Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html#bridgehead_N451690).
    
    -   You can import values for custom transaction item options along with Items sublist data. The Item Options feature must be set up in your account, and transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_. For details, see [Importing Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html).
        
    -   If you don't map the Price Level field for any imported transaction items, the base price from the item record is used as that line item's price. To use a different price, map the Price Level field in your import, and either include a Price Level column with values in the CSV file, or on the Field Mapping page, click the edit icon for the mapped Price Level field and select Custom as the default. (Note that this default is not guaranteed to be a valid level for all items.)
        
-   Be aware of the following when you use the Import Assistant to update transaction records:
    
    -   As of Version 2010 Release 1, the Use Conditional Defaults option is no longer available. Now, imports always populate field values automatically when related field values are set, in the same manner that field values are populated in the user interface. For updates, be sure to include all necessary values in CSV files, to avoid inadvertently changing existing field values to defaults.
        
    -   Some transaction sublists are keyed and some are not. For non-keyed sublists, partial updates aren't supported; CSV file sublist data either completely replaces existing sublist data or is appended, depending on the setting for the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option. Also, for non-keyed sublists, you shouldn't update main transaction fields and sublist fields in the same import job. For a list of keyed and non-keyed transaction sublists supported for import, see [Supported Sublist Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html).
        
    -   The Import Assistant lets you update items data for the following types of transactions: Cash Sale, Estimate, Invoice, Opportunity, Purchase Order, Sales Order, and Vendor Bill. You can modify data for existing line items and add line items to existing transactions. The Items sublist for transactions uses either Line/Order Line or Item as a key field to determine how to update or add line items. For more information, see [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html).
        
    -   Complete deletion of sublist data currently isn't supported. Existing sublist data can only be overwritten with new CSV file sublist data, not with an absence of CSV file sublist data.
        
    -   You can use transaction import capabilities to perform mass updates of supported transaction subtype data. Create a saved search, export saved search results and modify them in an external application, then use the Import Assistant, with an Update data handling option, to reimport modified data. You need to set certain criteria for your saved search to generate an exported file with appropriate data for reimporting. For information, see [Creating Transaction Saved Searches for Reimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html).
        

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)

### Related Topics

-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
