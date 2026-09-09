---
id: "section_N2185383"
type: "section"
title: "Creating Item Coupons"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Creating Item Coupons"
parent: "chapter_N2180614"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185383.html"
anchors: ["procedure_N2185416"]
sha256: "b0a3da46c170af1085e55d87c4f56e078fb14aec26fb39cb38f90ec0dfc016c5"
---

You can offer coupon codes for specific items when you enable the Promotion Codes feature.

Note:

An administrator can enable this feature on the Transactions subtab at _Setup > Company > Setup Tasks > Enable Features_.

#### To create an item coupon: {#procedure_N2185416}

1.  Go to _Lists > Accounting > Items > New > Discount_ to set up the discount amount for the coupon.
    
    The dollar or percentage amount you enter in the **Rate** field is the discount amount.
    
    For more information about creating discount items, see [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html).
    
2.  Go to _Lists > Marketing > Promotion Codes > New to set up a promotion code for this coupon._ to set up a promotion code for this coupon.
    
    For more information about promotion codes, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html).
    
3.  In the **Promotion Code** field, enter the code you want customers to use for the discount. Customers on your website will enter this code in the **Coupon Code** field at checkout.
    
4.  In the **Discount** field, select the name of the discount item you created for this coupon.
    
5.  In the **Apply Discount To** field, select **First Sale Only** to let this coupon be used one time per customer.
    
    Select **All Sales** to let the code be used multiple times.
    
6.  In the **Start Date Promotion** field, enter the date this coupon starts.
    
7.  In the **End Date Promotion** field, enter the date this coupon expires.
    
8.  Check the **Available to All Customers** box to make this coupon code public.
    
    If you clear this box, only customers linked to partners you select on the **Partners** subtab can use this code.
    
9.  On the **Items** subtab, select and add each item that you want this discount to apply to.
    
10.  Check the **Exclude Items** box to have this discount apply to all items **except** the ones you select.
     
11.  Click **Save**.
     

You can now give customers this code to use as a coupon for the items you selected.

Discounts only apply to eligible items. For example, if a coupon gives $10 off all cables, and someone buys a cable for $9 and speakers for $40, only $9 is discounted. Discounts are applied before tax and shipping.

### Related Topics

-   [Setting Up Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181018.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)
-   [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html)
-   [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html)
-   [Updating Item Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184312.html)
-   [Updating Item Purchase Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184741.html)
-   [Swapping Prices Between Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185052.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
