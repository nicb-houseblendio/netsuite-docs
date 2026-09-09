---
id: "section_N1857206"
type: "section"
title: "Creating Tax Groups - Canada"
branch: "canada-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > Canada Help Topics > Canada Tax Topics For Accounts Without SuiteTax > Creating Tax Groups - Canada"
parent: "section_156941156434"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857206.html"
anchors: ["procedure_N1857226"]
sha256: "a4f7be1c56410943d24a9d0e7266e44f252aaa899e97acd196e7db91fc4ce9fe"
---

A tax group is a group of tax codes relevant to a transaction. For information, see [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html).

When a Canadian nexus is created, the following tax groups are also created, unless they already exist:

-   CA-S-\[Province\], for example CA-S-ON for Ontario
    
-   CA-PST-\[Province\], for example CA-PST-ON for Ontario
    
-   CA-GST only
    
-   CA-Zero
    
-   CA-E
    
-   .
    

Important:

Canadian tax groups **CA-GST only**, **CA-Zero**, **CA-E**, and **.** musn't be renamed. If you rename them, then when you create a new Canadian nexus, the system will recreate those tax groups. The duplicate tax groups will cause problems in your account.

![List of tax groups for Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/CountrySpecificFeatures/CanadaTaxGroups.png)

#### To create a tax group for Canada: {#procedure_N1857226}

1.  Go to _Setup > Accounting > Taxes > Tax Groups > New_.
    
2.  If you are using OneWorld, select **Canada** in the **Item Type** column.
    
3.  On the New Tax Group page, enter an abbreviation in the **Tax Name** field.
    
4.  Enter a description of the tax group.
    
5.  Select a province.
    
6.  If you are using OneWorld, do the following:
    
    1.  Select one or more subsidiaries.
        
    2.  Check the **Include Children** box if you want to apply the tax code to the children of the subsidiary.
        
7.  Select a GST/HST (Goods and Services Tax/Harmonized Sales Tax) code. The rate of the code you select automatically appears in the **Rate** field.
    
8.  Select a PST (Provincial Sales Tax) code. The rate of the code you select automatically appears in the **Rate** field.
    
9.  Check the **Piggy Back** box if you want this tax code to include GST in addition to the line item amount when calculating PST. If you don't check this box, PST is calculated for the line item amount only.
    
10.  Check the **Inactive** box if you want to inactivate this tax group. An inactivated tax group won't show up for selection in a transaction.
     
11.  Click **Save**.
     

Important:

The **Tax Type** field on the tax code record can no longer be changed if the tax code has already been added to a tax group.

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
