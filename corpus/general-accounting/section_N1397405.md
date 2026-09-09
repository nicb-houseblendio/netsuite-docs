---
id: "section_N1397405"
type: "section"
title: "Assigning Currencies to Entities"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Currency Management > Multiple Currencies > Assigning Currencies to Entities"
parent: "section_N1395463"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397405.html"
anchors: ["procedure_N1397588"]
sha256: "b999e42655046e35dd7fe049c6f0aec42d15f6e419b787e4dc814713d64ede39"
---

An entity is a record that defines people or organizations. This topic applies to entities that can have multiple currencies.

If you use the Multiple Currencies feature, you can assign multiple currencies to a single customer or vendor record. You can add currencies to a customer or vendor record at any time. This ability lets you record transactions in the currency your customer or vendor prefers. Prospect records, which can be converted to customer records, also support multiple currencies. For information about these record types, see [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html).

Note:

The Multiple Currencies feature includes capabilities that were historically separate features. The Multi-Currency Customers and Multi-Currency Vendors features have been combined in the Multiple Currencies feature. If the Multi-Currency Customers and Multi-Currency Vendors features are available in your account and not enabled, your customer and vendor records can have only one currency.

NetSuite OneWorld requires that you assign entities to subsidiaries. An entity inherits the subsidiary's currency as its primary currency. For more information, see [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html).

#### To assign currencies to an entity: {#procedure_N1397588}

1.  Create a new entity record or edit an existing record.
    
    For example, go to _Lists > Relationships > Customers > New_ to create a new record, or go to _Lists > Relationships > Customers_ and click **Edit** next to an existing record.
    
2.  In NetSuite OneWorld, select the **Subsidiary** if not already selected.
    
3.  Click the **Financial** subtab.
    
4.  In the **Primary Currency** field, select the entity's primary currency.
    
    By default, the system selects the entity's company or subsidiary currency.
    
    Note:
    
    If you change the primary currency, the system removes any credit limit previously set on the entity record. Credit limits vary with the exchange rates of foreign currencies.
    
5.  To add multiple currencies for the entity, complete the following steps:
    
    1.  On the **Currencies** subtab, select another currency for use by the entity.
        
        If you don't have a **Currencies** subtab, your account has the older implementation of the Multiple Currencies feature, and multiple currencies isn't enabled for the current entity. For details, see [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html).
        
        For a screenshot that shows the Currencies subtab, see [Customer Balances in Transaction Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1400109.html#subsect_161610274695).
        
    2.  Click **Add**.
        
6.  To customize the currency format to be used on screen and for printed documents for a customer or prospect, complete the following steps:
    
    1.  On the **Currencies** subtab, select a currency row.
        
    2.  In the **Format** column, click the Edit ![Edit icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/EditIcon.png) icon.
        
    3.  Edit the following fields as appropriate:
        
        -   In the **Symbol** field, enter a symbol for the currency. Include spaces if you want to separate the symbol from the amount.
            
        -   For **Symbol Placement**, select **Before Number** or **After Number** to indicate where the currency symbol appears.
            
        
        The **Format Sample** field displays the currency format with your changes.
        
7.  Click **Save**.
    

### Related Topics

-   [Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395463.html)
-   [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html)
-   [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html)
-   [Setting a Base Currency](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1397082.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
