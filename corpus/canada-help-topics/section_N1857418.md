---
id: "section_N1857418"
type: "section"
title: "Enabling Canada Tax Lookup"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Tax Topics For Accounts Without SuiteTax > Enabling Canada Tax Lookup"
parent: "section_156941156434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857418.html"
anchors: ["bridgehead_3784670425"]
sha256: "e602335130742aa390f66471dc57a4267f6548f422c45635a0e0299cf6fa50c3"
---

You can choose to have NetSuite determine the proper tax code automatically when a sales transaction is entered manually or through your website.

#### To enable the tax lookup for Canada:

1.  Go to _Setup > Accounting > Taxes > Set Up Taxes_.
    
2.  If you are using a OneWorld account, click the **Canada** subtab.
    
3.  Check the **Enable Tax Lookup on Sales and Purchases** box.
    
4.  Click **Save**.
    

To determine the proper tax code to use for an item on a sales transaction record, the system looks for certain values in the following order:

1.  **Tax Item** field on the customer record
    
2.  Customer's shipping address on the transaction record
    
3.  **Tax Code** field on the item record (required for most item types). For accounts with Advanced Taxes enabled, the field is labeled **Tax Schedule**.
    

The following fields also affect how tax codes are determined:

1.  **Province** field on the tax code record
    
2.  Fields on the Set Up Taxes page:
    
    -   Tax Code for Out-of-Province Sale
        
    -   Tax Code for International Sale
        
    -   Default Tax Code (required)
        
3.  **PST Exempt** box on the customer record (available only for customers associated with a Canadian subsidiary)
    
4.  Nexus and sales tax code on the tax schedule record (in accounts with Advanced Taxes enabled)
    

## Canada Tax Lookup {#bridgehead_3784670425}

1.  To determine the tax code to use for a transaction, NetSuite first looks at the tax item on the customer record. If there is a tax group in the **Tax Item** field of the customer record, then the system uses that customer's tax group for the items on the transaction record.
    
2.  If there is no tax group in the **Tax Item** field of the customer record, and the **PST Exempt** box isn't checked, then the system looks at the shipping address on the transaction record:
    
    1.  If the province in the customer's shipping address is the same as yours, or you have a nexus in the customer's province, then:
        
        | With Advanced Taxes | The system uses the tax schedule on the item record. |
        | --- | --- |
        | Without Advanced Taxes | The system uses the tax code (tax group) on the item record. |
        
    2.  If the customer's shipping address is different from yours and you don't have a nexus in the customer's province, then (with or without Advanced Taxes):
        
        | If the customer's shipping address is outside of Canada | The system uses the tax code in the **Tax Code for International Sale** field on the Set Up Taxes page for Canada. If the **Tax Code for International Sale** field is empty, then the system uses the tax code selected in the **Default Tax Code** field. |
        | --- | --- |
        | If there is **only one** active tax group applicable for the customer's province | The system uses the tax group for that province. |
        | If there is no tax code or there is more than one tax code applicable for the customer's province | The system uses the tax code in the **Tax Code for Out-of-Province Sale** field on the Set Up Taxes page for Canada. If the **Tax Code for Out-of-Province Sale** field is empty, then the system uses the tax code selected in the **Tax Code for International Sale** field. If the **Tax Code for International Sale** field is empty, then the system uses the tax code selected in the **Default Tax Code** field. |
        
3.  If the **PST Exempt** box is checked on the customer record, the system uses the tax code in the **Tax Code for Out-of-Province Sale** field of the Set Up Taxes page for Canada. If the **Tax Code for Out-of-Province Sale** field is empty, then the system uses the tax code selected in the **Tax Code for International Sale** field. If the **Tax Code for International Sale** field is empty, then the system uses the tax code selected in the **Default Tax Code** field.
    
    Note:
    
    In the **Tax Item** field of the customer record, if you select a tax code with 0% rate, the customer won't be charged any tax.
    

### Related Topics

-   [Setting Tax Preferences for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856454.html)
-   [Creating Tax Codes - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1856762.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
-   [Viewing Canadian Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1860262.html)
-   [Processing Goods and Services Tax (GST) Refunds - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859567.html)
-   [Paying Provincial Sales Tax - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1859840.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
