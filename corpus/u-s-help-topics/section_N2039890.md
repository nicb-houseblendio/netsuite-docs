---
id: "section_N2039890"
type: "section"
title: "Creating a Tax Group (United States)"
branch: "u-s-help-topics"
category: "country-specific-features"
breadcrumb: "Country-Specific Features > U.S. Help Topics > Taxation Features For Accounts without SuiteTax > Creating a Tax Group (United States)"
parent: "section_156940239941"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039890.html"
anchors: ["procedure_N2039910"]
sha256: "fbdbe143fac7683c02b4984a428c28bbf6c7ee0aa4b81d3d01551cf628790dea"
---

A tax group is a group of tax codes relevant to a transaction. When you have set up your tax codes, you can combine them to create tax groups. For information, see [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html).

Note:

don't delete the system-generated tax group **Not Taxable** (ID: -8). This can cause errors when creating transactions.

#### To create a tax group (United States): {#procedure_N2039910}

1.  Go to _Setup > Accounting > Taxes > Tax Groups > New_.
    
2.  If you are using a OneWorld account, select **United States** in the **Item** type column.
    
3.  On the New Tax Group page, enter an abbreviation in the **Tax Name** field.
    
4.  Enter a description for this tax group.
    
5.  If you are using a OneWorld account:
    
    1.  Select one or more subsidiaries.
        
    2.  Check the **Include Children** box if you want to apply the tax code to the children of the subsidiary.
        
6.  Enter the county and town, and select the state from the dropdown list.
    
7.  Enter the zip codes that this tax group applies to.
    
8.  Check the **Default Code** box if this code is the default tax group to be selected on transactions. This tax code is selected if the customer's shipping address does not match another tax group.
    
9.  Check the **Inactive** box if you want to inactivate this tax group. An inactive tax group won't show up for selection in a transaction.
    
10.  In the **Name** column, select a tax code and then click **Add**. Select as many tax codes as applicable. The total tax code rate will be the tax group rate.
     
     Note:
     
     To add new tax codes to the list, see [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html).
     
11.  Click **Save**.
     

### Related Topics

-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Creating Tax Codes - U.S. Nexus](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2039577.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)
-   [Tax Groups Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
