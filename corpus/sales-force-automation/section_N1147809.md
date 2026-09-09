---
id: "section_N1147809"
type: "section"
title: "Sales Effective Date"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Commissions > Employee Commission Plans > Sales Effective Date"
parent: "section_N1146679"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147809.html"
anchors: []
sha256: "3397e8b13febed0452fff116e51e795b480c463e1042f83b5f9cbbb92c836da4"
---

The sales effective date determines how NetSuite applies credit transactions with regards to commission. This date appears on transactions and you can edit it.

Note:

On commission reports, the sales effective date is the same date as the commission effective date.

You can have the sales effective date on the credit transaction default to the date of the related sales transaction. Go to Setup > Sales > Preferences > Sales Preferences > General subtab. Clear the **Default Sales Effective Date to Linked Sales Effective Date** box to make the sales effective date the same as the credit transaction date. Keep this box checked to make the sales effective date default to the date of the sales transaction. NetSuite enables this preference by default.

To illustrate: an invoice is entered on 11/11/2018 for $100. The sales rep on the deal received a 10% commission, or $10. The sales rep's manager received $2 commission. The sales effective date on the invoice is 11/11/2018. On 06/03/2019, the customer advised that they would not be able to pay, so a credit memo was issued for $100.

Note:

If you use this preference and you change the credit transaction date, NetSuite changes the sales effective date to the credit transaction date.

The commission is recalculated in one of the following ways, depending on the sales effective date on the credit transaction:

-   If the credit memo date is set to the invoice date (11/11/2018), the sales rep and manager would be issued negative commission amounts. These negative commission amounts would be $10 for the sales rep and $2 for the manager.
    
-   If the credit memo date is set to the current date (06/03/2019), NetSuite calculates the commission based on the plan which used that current date. In addition, the sales rep's current manager as of 06/03/2019 would be issued the negative commission amount of $2.
    

### Related Topics

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
-   [Employee Commission Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146679.html)
-   [Creating an Employee Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1146859.html)
-   [Assigning Sales Reps to a Commission Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147232.html)
-   [Recalculating Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147526.html)
-   [Split Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1148007.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
