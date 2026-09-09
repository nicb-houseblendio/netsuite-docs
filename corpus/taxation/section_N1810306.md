---
id: "section_N1810306"
type: "section"
title: "Creating a Tax Group (All Countries Except US and Canada)"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Groups Overview > Creating a Tax Group (All Countries Except US and Canada)"
parent: "section_N1809948"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810306.html"
anchors: ["procedure_N1810339"]
sha256: "fd5d1f85e6c0310db999a30b669ab28d8b6499d8d344b4949721a22c7b69ae65"
---

Note:

For US, see [Creating a Tax Group (United States)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039890.html). For Canada, see [Creating Tax Groups - Canada](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1857206.html).

Changes made to tax groups are captured in system notes. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

#### To create a tax group (all countries except US and Canada): {#procedure_N1810339}

1.  Go to _Setup > Accounting > Taxes > Tax Groups > New_.
    
2.  If you're using NetSuite OneWorld, select a country in the **Item type** column.
    
3.  On the Tax Group page, enter an abbreviation in the **Tax Name** field.
    
4.  Enter a description of the tax group.
    
5.  If you're using NetSuite OneWorld:
    
    1.  Select one or more subsidiaries from the dropdown list.
        
    2.  Check the **Include Children** box if you want to apply this tax group to the children of the subsidiaries.
        
6.  Select a tax type.
    
7.  In the **Name** column, select a tax code and then click **Add**. You can select as many tax codes as applicable. The tax code rate and tax type are automatically populated from the selected tax code. The sum of the tax code rates will be the tax group rate and it'll appear in the tax group's **Rate** field.
    
    Important:
    
    To make this tax group selectable on a sales transaction, make sure the tax codes in the tax group have Sales or Both in the **Available on** field of the tax code record. For purchase transaction, the tax codes in the tax group should have Purchases or Both.
    
8.  Enter a value in the **Basis** column for each tax code. By default, it's 100, which represents the full rate. If the tax rate is 10% and the basis is 100, then 10% is added to the tax group rate. If the tax rate is 10% and the basis is 50, only 5% gets added.
    
9.  Click **Save**. You can now select this tax group when you create a transaction record.
    

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
