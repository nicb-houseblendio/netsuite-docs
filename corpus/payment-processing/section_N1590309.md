---
id: "section_N1590309"
type: "section"
title: "Setting Up Bank Records"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Electronic Bank Payments > Setting Up Electronic Bank Payments > Setting Up Bank Records"
parent: "section_3831186542"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590309.html"
anchors: []
sha256: "a3161ecfe0b945a3feba938b305c51419f014481afd665cad9bc353036d2bdc2"
---

You need to set up the bank account records of the following entities before you can use the Electronic Bank Payments feature:

Note:

By default, only Administrators can set up bank records for companies and entities. You can enable this set up task for any of the records, for other users assigned with the Custom EFT Role. For more information, see [Setting Up Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1586829.html).

| Entity | Description |
| --- | --- |
| Company/Subsidiary | Set up the bank account details that your company or subsidiary can use to send and receive electronic bank payments. You also need to set up bank account details that your company or subsidiary can use for Positive Pay. |
| Vendor | Set up the bank account details of each vendor to whom you want to send electronic bank payments. You can set up multiple bank accounts for each vendor. |
| Employee | Set up the bank account details of each employee to whom you want to send electronic bank payments. You can set up multiple bank accounts for each employee. |
| Customer | Set up the bank account details of each customer to whom you can send customer refund payments. You can set up several bank accounts for each customer. You also need to set up the bank account details of each customer from whom you want to receive direct debit payments. You can set up several bank accounts for each customer. |
| Partner | Set up the bank account details of each partner to whom you can send commissions. You can set up several bank accounts for each partner. |

Note:

New record guidelines:

-   When creating new records, ensure that the following options are cleared on the Entity Bank Details record type:
    
    -   Enable Inline Editing
        
    -   Allow Child Record Editing
        
-   To create a record, go to _Customization > List, Records, & Fields > Record Types_.
    
-   You shouldn't change the payment file format after saving entity bank details. By doing this, the data from the previous file format fields may impact the validations and electronic payment processes resulting in errors. You should change the previous entity bank detail's status to inactive or deleted and create new entity bank details with new file formats.
    
-   Electronic Bank Payments SuiteApp doesn't provide **Save and Copy** and **Make Copy** options on Entity Bank Details page in NetSuite.
    
-   Bank Detail records are unlocked to for you to make customizations. However, you shouldn't change the default properties of the fields in the Bank Detail record to avoid bundle update issues.
    
-   You can track the status of a deleted, removed, or reassigned entity bank by using the **Bank Details Logs** column in the **Bank Details** subtab.
    
-   Entity bank detail can be created only from one of the following:
    
    -   A parent entity
        
    -   By providing a unique parent ID when using SuiteScript, CSV import, web services.
        
-   After you create an entity bank, you can't change the parent entity of the bank detail record by attaching it to another bank detail record. This feature is disabled to prevent functional impact.
    

To set up the bank records for your company, subsidiaries, vendors, employees, customers, and partners, click the country-specific set up instructions below:

-   [Austria Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1592839.html)
    
-   [Australia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1595666.html)
    
-   [Brazil Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1604270.html)
    
-   [Belgium Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1598164.html)
    
-   [Canada Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1608729.html)
    
-   [Czechia Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3983337126.html)
    
-   [France Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1611157.html)
    
-   [Germany Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1614186.html)
    
-   [Global Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664266.html)
    
-   [Hong Kong Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4121609908.html)
    
-   [Hungary Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1617944.html)
    
-   [Ireland Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1620105.html)
    
-   [Isle of Man Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048051055.html)
    
-   [Italy Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1623115.html)
    
-   [Japan Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1627002.html)
    
-   [Luxembourg Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1630311.html)
    
-   [Netherlands Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1636146.html)
    
-   [New Zealand Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1640223.html)
    
-   [Singapore Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1642722.html)
    
-   [South Africa Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1648257.html)
    
-   [Spain Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1651883.html)
    
-   [UK Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1656390.html)
    
-   [U.S. Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1659055.html)
    
-   [Global Payment Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1664266.html)
    

### Related Topics

-   [Setting Up Electronic Bank Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3831186542.html)
-   [Setting Up Payments Tab Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1589991.html)
-   [Creating Folders in the NetSuite File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1590174.html)
-   [Setting Up Payment Aggregation Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1592660.html)
-   [Importing Electronic Bank Payments Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3739634016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
