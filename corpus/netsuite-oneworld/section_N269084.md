---
id: "section_N269084"
type: "section"
title: "Subsidiary Hierarchy Planning"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiaries in OneWorld > Subsidiary Hierarchy Planning"
parent: "section_N268563"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269084.html"
anchors: []
sha256: "f03e7a6f9b6e3e7994dbee51b7558d6907220c4864b859c26288184ded41880c"
---

Before you create subsidiary records you should plan the structure of your organization's subsidiaries. For each subsidiary record you create, you must define its parent, and as you create subsidiaries, NetSuite automatically defines a hierarchical structure.

Important:

NetSuite enables you to modify your subsidiary hierarchy structure if your company requires modification. Be aware that a modification may damage your data and reporting. For information about modifying your subsidiary hierarchy and possible consequences, see [Subsidiary Hierarchy Structure Modification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157252074629.html).

You should diagram the parent-child relationships in your subsidiary hierarchy, starting at the top with the root subsidiary. This visual representation can help you consider how you want to organize and consolidate data, for both accounting and reporting purposes.

As you diagram your subsidiary hierarchy, it is a good idea to record the country, base currency, and tax nexuses for each subsidiary.

-   The country you enter on a subsidiary record automatically determines the first tax nexus and NetSuite edition associated with that subsidiary.
    
-   A base currency is the currency in which a subsidiary manages its financials. After you define and save a base currency on a subsidiary record, you can't change it.
    
-   A nexus is a tax jurisdiction. You can add and change nexuses on subsidiary records.
    

After you diagram a hierarchy of subsidiaries, you should include one elimination subsidiary as a child of each parent subsidiary. The elimination subsidiary should use the same base currency as the parent subsidiary.

Use the subsidiary hierarchy diagram as a roadmap for setting up subsidiaries. You can refer to the base currency listed for each subsidiary to ensure that all necessary currencies are set up in NetSuite. See [Multiple Currencies in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269257.html). You can refer to the country listed for each subsidiary to ensure that all tax nexuses are set up and linked to the appropriate country. See [Nexuses and Taxes in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N269581.html).

Use your diagram to reference the order in which to create subsidiary records, in top-down order, beginning with the root. Be aware that you can't change several fields on the subsidiary record after you create and save the record for the first time. See [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html) and [Editing Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273122.html).

If you enable the GL Audit Numbering feature, you can apply gapless numbering sequences to all general ledger posting transactions. These numbering sequences enable companies to meet international auditing requirements. The feature also enables you to specify that a subsidiary's transactions are locked to the general ledger. This option permits NetSuite to automatically generate journal entries when changes are made to a transaction that posted to the general ledger. See [GL Audit Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3735573963.html) and [GL Impact Locking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4725785967.html).

### Related Topics

-   [Elimination Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268759.html)
-   [NetSuite Editions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N270055.html)
-   [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
