---
id: "section_N268759"
type: "section"
title: "Elimination Subsidiaries"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiaries in OneWorld > Elimination Subsidiaries"
parent: "section_N268563"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268759.html"
anchors: []
sha256: "534eb36196d230263ab23c0fe2442bb4e4897842030d240eb548e21beb380f03"
---

When subsidiaries transact, you may have to eliminate the revenue and expenses at the consolidated level to remove the effect of transactions between subsidiaries.

For example, intercompany transaction balances may require elimination for the following reasons:

-   Sales and services between subsidiaries
    
-   Inventory transfers between subsidiaries
    
-   Loans between subsidiaries
    

You use elimination subsidiaries to post journal entries that balance consolidated books. These journal entries, called elimination journal entries, reverse the impact of the intercompany transactions. Each elimination journal entry posts to an elimination subsidiary.

Note:

Only journal entries post to elimination subsidiaries. No other transactions post to elimination subsidiaries. See [Elimination Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475762.html).

You create an elimination subsidiary (as a child of the parent subsidiary) for any subsidiary that has child subsidiaries. Set the currency to the same currency as the base currency of the parent subsidiary.

The following illustration shows a sample subsidiary hierarchy that includes an elimination subsidiary.

![Diagram of a sample subsidiary structure that includes an elimination subsidiary.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/NetSuiteOneWorld/UnderstandingSubsidiaries.png)

You create elimination subsidiaries the way you create other subsidiaries except that you check the Elimination box on the subsidiary record. For more information, see [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html).

License fees for subsidiaries do not include charges for elimination subsidiaries, and elimination subsidiaries do not count toward the maximum of 250 subsidiaries.

Note the following about elimination subsidiaries and transactions:

-   An elimination subsidiary must use the same base currency and country combination as their direct parent subsidiary.
    
-   With consolidated exchange rates, an elimination subsidiary must use a consolidated exchange rate of 1 to its direct parent subsidiary.
    
-   You can select an elimination subsidiary **only** for journal entries, not for other transactions.
    
-   A journal entry that is associated with an elimination subsidiary is a normal journal entry, not an advanced intercompany journal entry. It posts to a single elimination subsidiary. For more information about journal entries in OneWorld, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html).
    
-   Elimination transactions post only to the elimination subsidiary and do not affect the general ledger.
    
-   The system can automatically generate elimination journal entries if you enable the Automated Intercompany Management feature. See [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html).
    
-   You can't select an elimination subsidiary on a bank account record or a credit card account record.
    
-   You can't select an elimination subsidiary on item records.
    

### Related Topics

-   [Subsidiary Hierarchy Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269084.html)
-   [Multiple Currencies in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269257.html)
-   [Nexuses and Taxes in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html)
-   [NetSuite Editions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N270055.html)
-   [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
