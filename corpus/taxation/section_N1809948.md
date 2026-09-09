---
id: "section_N1809948"
type: "section"
title: "Tax Groups Overview"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Managing Tax Codes > Tax Groups Overview"
parent: "chapter_N1805198"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1809948.html"
anchors: ["bridgehead_N1809985"]
sha256: "415d86d348af64ae756ee537d26fe5f97eb48a93eb8544ed04828e9bbf14c521"
---

You can create a tax group to combine several tax codes for one transaction, even if the taxes are paid to different jurisdictions. The tax group rate is the sum of these separate tax codes.

Tax groups can track multiple tax control accounts. Each tax code in a tax group can have a different control account, allowing you to accurately account for taxes owed to each tax jurisdiction.

## Examples of when to use tax groups: {#bridgehead_N1809985}

-   In the United States, you can combine state tax, transit tax, and city tax into one tax group so that when you create a sales invoice, you can select the tax group to be applied to the transaction.
    
-   In Canada, each province has GST and PST, and rates vary for each province. You can create a tax group for each province, combining GST and PST.
    
-   In Australia, GST is added after applying wine equalisation tax (WET) to the price of wine. You can combine WET and GST in one tax group. For more information about WET, see [Using Wine Equalization Tax (WET)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3830143961.html).
    

Before using tax groups, go to _Setup > Accounting > Taxes > Set Up Taxes_. In the **Tax Code Lists Include** field, select **Tax Groups Only** or **Tax Groups and Tax Codes**. These selections allow you to select tax groups on transactions and on customer records.

Changes made to tax groups are captured in system notes. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

Note:

As you make the transition to using tax groups, set the tax code list to include both groups and codes. After you've set up the tax groups needed for your business, change the preference to show only tax groups.

To create tax groups, see [Creating Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810157.html).

### Related Topics

-   [Creating Tax Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810157.html)
-   [Creating a Tax Group (All Countries Except US and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810306.html)
-   [Tax Control Accounts Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1812226.html)
-   [Tax Types Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1810558.html)
-   [Tax Codes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805593.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
