---
id: "bridgehead_N1321283"
type: "bridgehead"
title: "Setting Preferred Forms for Contract Renewals"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Initial Setup Tasks for Contract Renewals > Setting Preferred Forms for Contract Renewals"
parent: "section_N1321054"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321283.html"
anchors: ["procedure_N1321297"]
sha256: "46daafac6d55287d36ea5fae7f5cf3d3f8f0f232d728aba696cf19e6a5488bb2"
---

Before you begin using the Software Vertical Contract Renewals SuiteApp, set the custom forms you want to use as Preferred.

#### To set your preferred forms: {#procedure_N1321297}

1.  Go to _Customization > Forms > Entry Forms_.
    
2.  Check the box in the **Preferred** column for these entry forms (From Bundle: 187488):
    
    -   Customer Form - Contract Renewals
        
    -   Item Group - Contract Renewals
        
    -   Inventory Item - Contract Renewals (available only if the Inventory feature is enabled)
        
    -   Non-Inventory Item - Contract Renewals
        
    -   Project Form - Contract Renewals
        
    -   Vendor Form - Contract Renewals
        
3.  Click **Submit**.
    
4.  Go to _Customization > Forms > Transaction Forms_.
    
5.  Check the box in the **Preferred** column for these transaction forms (From Bundle: 187488):
    
    -   Cash Sale - Contract Renewals
        
    -   Credit Memo - Contract Renewals
        
    -   Invoice - Contract Renewals
        
    -   Opportunity - Contract Renewals
        
    -   Quote - Contract Renewals
        
    -   Return Authorization - Contract Renewals
        
    -   Sales Order - Contract Renewals
        
6.  Click **Submit**.
    

Alternatively, you can also create copies and customize these locked forms to meet the specific needs of your business. For more information, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

Note:

When you customize transaction forms, make sure that the **Renewals Exclusion** column is shown in the item sublist. On the **Screen Fields** tab on the custom transaction form, make sure that the **Show** box for **Renewals Exclusion** on the **Columns** subtab is checked. This field is used by the contract item creation script (R03) to determine whether to set the contract's **Renewals Exclusion** field to true or false.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
