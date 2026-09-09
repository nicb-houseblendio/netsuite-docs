---
id: "section_N432599"
type: "section"
title: "Creating Transaction Saved Searches for Reimport"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Creating Transaction Saved Searches for Reimport"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N432599.html"
anchors: ["procedure_N432654"]
sha256: "3e74378e408e583f4a16cf3326eda3ee5f69f2750f1d1d5b6ea2bd77d03b063e"
---

This process enables mass update transaction record types by exporting data into an external application for updates and then reimporting them into NetSuite with the Import Assistant.

The most straightforward method to make NetSuite data available to other applications is to create a saved search and export the saved search results as a CSV orXLSX file.

For general information about NetSuite saved searches, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).

Because transaction ID values aren't unique, use internal ID or external ID as the unique identifier when reimporting transactions data. Be sure to include one or both of these fields as results columns for your saved search.

#### To create a transaction saved search for reimport: {#procedure_N432654}

1.  Go to _Transactions > Management > Saved Searches > New_.
    
2.  Select the Transaction search type.
    
3.  On the Saved Search definition page, enter basic search information, such as title.
    
4.  On the Criteria subtab, enter filters for your search data:
    
    -   Specify a filter for the type of transaction. Select Type in the filter list, and set it to be the transaction you want.
        
    -   For transactions that include line items, eliminate data that isn't attached to item costs, including main line, taxes, and shipping costs, because this data can result in 'Item Not Found' errors when you reimport. Specify filters like the following:
        
        -   Select Main Line in the filter list, and set it to False. For more information about main line data, see [Main Line in Transaction Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4459563851.html).
            
        -   Select Item in the filter list, and set it to 'Type is any of Assembly/Bill of Materials, Description, Discount, Download Item, Gift Certificate, Inventory Item, Item Group, Kit/Package, Markup, Non-inventory Item, Other Charge, Payment, Service, Subtotal.'
            
            Your list may vary, depending on your available item types.
            
    -   For more information about defining search filters, see [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html).
        
5.  On the Results subtab, enter the results fields that you want to include.
    
    -   Make sure you include the field you want to use as a unique identifier, either internal ID or external ID, in the results.
        
    -   Include all fields that you want to modify in the external application. For example, if you want to modify the quantities of line items, include the quantity field.
        
    -   You can include joined item fields if you want to modify them. Scroll down in the Field list to Item Fields..., and select a field from the Item Field list.
        
    -   For more information about defining search results fields, see [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html).
        
6.  Define any additional search options that you require.
    
    For information about available options, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
    
7.  Click Save & Run to run your saved search.
    
    -   If the search results don't meet your needs, click the Edit this Search button to modify the definition.
        
    -   If the search results are satisfactory, click Export - CSV or Export - Microsoft Excel.
        
    
    You can then edit the data in the external application.
    

After editing the data in the external application, you can reimport the file using the CSV Import Assistant.

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
