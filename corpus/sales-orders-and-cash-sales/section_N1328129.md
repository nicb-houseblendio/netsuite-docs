---
id: "section_N1328129"
type: "section"
title: "Importing Contracts"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Contract Creation Process > Importing Contracts"
parent: "section_N1325604"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1328129.html"
anchors: ["procedure_N1328145"]
sha256: "d54723a4a1bd1921eb058e1d9f76484d5d306425f6d6092adc58dc681033befa"
---

You can import your existing contract and contract items using the CSV Import Assistant. For information about CSV files, see [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)

To import contracts into your NetSuite account, you must import both contracts and the associated contract items.

#### To import contract records: {#procedure_N1328145}

1.  Prepare a CSV file with your contract data.
    
    These contract fields are required:
    
    -   Name
        
    -   End User
        
    -   Bill To Customer
        
    -   Contract Start Date
        
    -   Contract End Date
        
    -   Currency (if the Multiple Currencies feature is enabled)
        
    -   Renewal Terms
        
    
    For more information about contract fields, see [Contract Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4460975456.html).
    
2.  Go to _Setup > Import/Export > Import Tasks > Import CSV Records_.
    
3.  In the **Import Type** field, select **Custom Records**.
    
4.  In the **Record Type** field, select **Contract**.
    
5.  Select the CSV import file with your contract data.
    
6.  Click **Next**.
    
7.  Follow the rest of the steps in Import Assistant. For more information, see [CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4470700566.html).
    

#### To import contract item records:

1.  Prepare a CSV file with your contract item data.
    
    These contract item fields are required:
    
    -   Bill To Customer
        
    -   End User
        
    -   Contract
        
    -   Item
        
    -   Contract Item Start Date
        
    -   Contract Item End Date
        
    -   Quantity
        
    -   Original List Rate
        
    -   Owner
        
2.  Go to _Setup > Import/Export > Import Tasks > Import CSV Records_.
    
3.  In the **Import Type** field, select **Custom Records**.
    
4.  In the **Record Type** field, select **Contract Item**.
    
5.  Select the CSV import file with your contract item data.
    
6.  Click **Next**.
    
7.  Follow the rest of the steps in Import Assistant. For more information, see [CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4470700566.html).
    

Important things to note when importing transactions for contract renewals:

-   When an imported sales order record (of Import Type: Transactions) includes conflicting contract term and end date values, the contract term value overwrites the end date's value with the calculated value. For information about contract term, see [Contract Term Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4582083020.html).
    
-   In transaction imports, line items for non-Perpetual item categories must have contract term and end date values to generate the end date for each item. If the values are missing, the import fails. The end date value can be mapped for a line item if the date is prior to or the same as the contract's end date.
    
-   In transaction imports, line items' List rate is required if Custom price level is used.
    

### Related Topics

-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Creating a New Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325805.html)
-   [Scripting Contract and Contract Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1329149.html)
-   [Adding Transaction Fields to a Web Service Request for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4539453728.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)
-   [Editing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448152522.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
