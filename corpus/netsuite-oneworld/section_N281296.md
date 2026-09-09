---
id: "section_N281296"
type: "section"
title: "Employee and Partner Commission in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > OneWorld CRM > Employee and Partner Commission in OneWorld"
parent: "section_N281005"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281296.html"
anchors: []
sha256: "18e682b1d02168b9db60d6dc4c5c1152c84892526ec6fa6da5032f43069df2ab"
---

With NetSuite OneWorld, employees and partners can earn commission for sales made for any subsidiary.

Commission schedules have a subsidiary field. Commission plans can include any commission schedules, regardless of the subsidiary chosen on those schedules.

If you base a commission schedule on a quota, you must have a quota entered for the selected subsidiary.

Transactions made for the selected subsidiary, or for any child subsidiaries, are used to calculate commissions for sales reps assigned to the commission schedule. Commission schedule amounts are entered in the base currency of the selected subsidiary. NetSuite uses the consolidated exchange rates table to calculate values for transactions for other subsidiaries with different base currencies.

When employees or partners make sales for an unassigned subsidiary, NetSuite generates commission based on the following:

-   You have a commission schedule in the currency of one subsidiary. A sales rep makes a sale for one of the child subsidiaries. NetSuite converts the commission calculation to the sales rep's currency through the consolidated exchange rate table.
    
-   NetSuite performs the commission calculation based on the currency of the subsidiary assigned to the commission schedule. All values on reports and KPIs display the commission in that currency, regardless of the currency assigned to the partner or employee's subsidiary.
    
-   The generated commission transaction is always in the base currency of the subsidiary assigned to the employee or partner (partner's vendor record). If necessary, NetSuite converts a commission for a schedule assigned to another subsidiary. NetSuite uses the exchange rates on the transaction to the currency of the employee or partner.
    
-   After a commission is approved, the commission expense and payable impact the accounting books of the subsidiary assigned to the employee or partner. This impact is true even if the transaction that generated the commission is related to a subsidiary different from the employee or partner. It is also true if the commission schedule is assigned to another subsidiary.
    

Sales reps from different subsidiaries can be assigned to sales managers from the same or other subsidiaries. The sales for subordinate sales reps roll up to the sales manager. NetSuite uses the consolidated exchange rates between the subsidiaries for the period in which the sales transaction is booked.

For more information about employee and partner commissions in NetSuite OneWorld, see the following help topics:

-   [Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1122333.html)
    
-   [Partner Commissions & Royalties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1169123.html)
    
-   [Consolidated Exchange Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1404834.html)
    

### Related Topics

-   [Consolidated Exchange Rates With Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281410.html)
-   [Quota-Based Commission Schedules in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281858.html)
-   [Authorize Commissions in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N282241.html)
-   [Consolidated Quotas and Forecasts in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281162.html)
-   [Subsidiaries on Online Customer Forms in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N282433.html)
-   [OneWorld CRM](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281005.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
