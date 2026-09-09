---
id: "section_N1804737"
type: "section"
title: "Creating Tax Schedules"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Advanced Taxes > Creating Tax Schedules"
parent: "chapter_N1803438"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804737.html"
anchors: ["procedure_N1804791", "bridgehead_N1804850", "bridgehead_N1804885"]
sha256: "52695e9478573671e4ca33bfcad3ca110b4243b1c9b6ea77ae8742e857fdfb45"
---

Tax schedules are required in accounts with the Advanced Taxes feature enabled. Tax schedules determine how NetSuite calculates taxes for items in each nexus. The **Tax Schedule** field on an item record is located on the **Accounting** subtab, under Tax/Tariff Information.

For most countries, goods and services are charged at the same rate across the country, so there is no need for tax schedules to be set up. For the U.S. and Canada, some goods and services are not taxable in certain states or provinces, so in this case a tax schedule is useful.

In accounts without Advanced Taxes enabled, the tax treatment for an item is determined by the tax code assigned to it. For U.S. editions without Advanced Taxes, instead of a tax code, the **Taxable** box determines whether an item should be taxed or not.

#### To create a tax schedule: {#procedure_N1804791}

1.  Go to _Setup > Accounting > Tax Schedules > New_.
    
2.  In the **Product** field, enter the name of the tax schedule that you want to associate with a product or item.
    
    When you create or edit item records, you can select the name of the tax schedule on the **Accounting** subtab of standard item forms.
    
3.  Enter a description for this tax schedule.
    
4.  If you have nexuses in the United States, click the **US Nexuses** subtab, and then check the box in the **Taxable** column next to each state where these items are taxable.
    
    ## US Nexuses Subtab {#bridgehead_N1804850}
    
    ![Screenshot showing the US Nexuses subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/2011_2_USNexusesTab.png)
5.  If you have Non-U.S. nexuses, click the **Non US Nexuses** subtab, and select the sales and purchase tax codes to be used when charging customers with shipping addresses in those countries.
    
    ## Non US Nexuses Subtab {#bridgehead_N1804885}
    
    ![Screenshot showing the Non US Nexuses subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/2011_2_NonUSNexusesTab.png)
6.  Click **Save**.
    

You can create or edit an item record and choose the tax schedule that applies to the item. For more information about item records, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

Please note, REST web services don't support legacy tax features. To work with taxation through REST web services, you must have the SuiteTax feature enabled. For more information, see [Overview of SuiteTalk REST Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1540391670.html).

### Related Topics

-   [Enabling Advanced Taxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803739.html)
-   [Creating Tax Nexuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804264.html)
-   [Nexuses and Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1804037.html)
-   [Tax Accounting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1791910.html)
-   [General International Tax Topics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1813074.html)
-   [Managing Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1805198.html)
-   [Enabling and Setting Up Taxation Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1794679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
