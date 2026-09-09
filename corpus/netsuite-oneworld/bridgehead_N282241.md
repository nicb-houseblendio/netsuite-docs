---
id: "bridgehead_N282241"
type: "bridgehead"
title: "Authorize Commissions in OneWorld"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > OneWorld CRM > Employee and Partner Commission in OneWorld > Authorize Commissions in OneWorld"
parent: "section_N281296"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N282241.html"
anchors: []
sha256: "f684a234f55a0d457dffce4572379b1d6eaa821871b6fcfa4177cbdb8d52e84b"
---

The Authorize Commission page has a subsidiary list that filters the display based on the subsidiary of the employee or partner.

The accounts you select on this page must be accessible to the selected subsidiary.

When you authorize commission in bulk, the currency rate used is the most recent transaction currency in the currency exchange rate table. For example, if a Canadian rep earns commission on a U.S. commission schedule, the schedule generates the commission transaction in U.S. dollars. This commission must be posted to the Canadian subsidiary's books in Canadian dollars. The rate used for this conversion is based on the rate stored in the consolidated exchange rate table.

The currency rates used during authorization are the most recent exchange rates in the currency exchange rate table. To view currency exchange rates, so to _Lists > Accounting > Currency Exchange Rates_.

The **By Transaction** and **By Period** subtabs on the individual commission pages include the following columns:

-   **Currency** - This is the currency of the commission transaction. It is the same as the currency of the subsidiary assigned to the employee or partner.
    
-   **Subsidiary** - This is the subsidiary to which NetSuite posts the commission transaction.
    
-   **Exchange Rate** - This column appears only for partner commission. It determines the rate from the base currency of the subsidiary assigned to the partner to the partner's transaction currency.
    
    For example, you have a partner that is paid in Canadian dollars. The partner is assigned to a U.K. subsidiary that sells for a U.S. subsidiary. The commission schedule would be in U.S. dollars. The exchange rate on each line of the commission transaction would use a rate to convert the amount from USD to GBP. The exchange rate in the header would convert the amount from GBP to the partner's currency, CAD.
    

### Related Topics

-   [Consolidated Exchange Rates With Commissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281410.html)
-   [Quota-Based Commission Schedules in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N281858.html)
-   [Employee and Partner Commission in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N281296.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
