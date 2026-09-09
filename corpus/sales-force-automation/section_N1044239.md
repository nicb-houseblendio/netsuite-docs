---
id: "section_N1044239"
type: "section"
title: "Selling with Promotion Codes"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Selling with Promotion Codes"
parent: "chapter_N1035717"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1044239.html"
anchors: []
sha256: "ddf8ebaa01b4a13f041b100316cd11afa7dc169c43536c70d032ddce96fc12bc"
---

Promotions let you to track the source of revenue and offer discounts in the form of coupons. Each promotion has a promotion code that you can use on transactions and campaigns.

Administrators can enable the Promotion Codes feature at _Setup > Company > Setup Tasks > Enable Features_. The feature is on the Transactions subtab in the Sales section.

NetSuite tracks promotion codes based on the following:

-   **Transactions**
    
    Customers or sales reps can enter promotion codes on cash sales, invoices, sales orders, return authorizations, and refunds.
    
    You can assign discount items to promotion codes. When you select a promotion code with a discount on a transaction, the correct discount appears. When a customer checks out on your website, they can enter a promotion code in the Coupon Code field to receive a promotional discount. You can change the discount when you create or edit promotion codes. For information about creating discounts, see [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html).
    
    You can also set promotion codes to apply to only certain items, making them item coupons. Only customers who purchase the items attached to the promotion code can use the code to receive the discount.
    
    For information about promotions and transactions, see [Applying Promotions and Discounts to a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4692024512.html).
    
-   **Lead, Prospect, and Customer Records**
    
    NetSuite tracks promotion codes on lead, prospect, and customer records in hidden fields. When you track promotion codes on these records, you can use reports to determine which marketing campaigns bring new customers to your company.
    
    The Promotion Code field on customer records is set using online customer forms. To create an online customer form, go to _Setup > Sales & Marketing Automation > Online Customer Forms > New_.
    
    Ensure that you choose the Promotion Code field on the Fields subtab. When you link to this form, customers can enter the promotion code themselves. You can also pass this promotion code to the form by appending the URL with &promocode=\[promotion code\]. For example, the URL in the link could look like http://netsuite.onlinecustomerform.com&promocode=2019 Spring Sale.
    
    You can use the same tip to append a promotion code to a URL link to your site. If the promotion code is associated with a discount, the discount is applied to web orders when your store is accessed using the URL.
    
-   **Campaigns**
    
    If you use the Marketing Automation feature, you can track promotions offered with campaign events.
    
    For more information, see [Managing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N985526.html).
    
-   **Partner Records**
    
    You can link your promotion codes to partners. If a customer comes to your website from a partner website, that partner's code and promotion code are tied to that customer. The customer can then only use promotion codes associated with that partner.
    

To create a promotion code, go to _Opportunities > Other > Promotions > New_. For more information, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html).

### Related Topics

-   [Tracking Campaign Revenue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990329.html)
-   [Marketing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1017620.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
