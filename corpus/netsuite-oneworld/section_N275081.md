---
id: "section_N275081"
type: "section"
title: "Using Subsidiary-Specific Transaction Auto-Numbering"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiary Setup > Using Subsidiary-Specific Transaction Auto-Numbering"
parent: "section_N272210"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275081.html"
anchors: ["procedure_N275124"]
sha256: "055d447734e59f1a62f50efd4d345d2673169bd13ffc48da5f3bd3852a7fc854"
---

With NetSuite OneWorld, each subsidiary can use individual numbering sequences for transactions. For example, transactions associated with Subsidiary A can use the numbering prefix SubA.

Numbering transactions by subsidiary is useful for users with access to only one subsidiary because they do not encounter numbering gaps for another subsidiary's transactions.

Be aware that some countries require unique numbering without gaps for each legal entity.

Note:

A transaction inherits its subsidiary from its entity (customer or vendor). See [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html).

#### To set up or update auto numbering for a subsidiary: {#procedure_N275124}

1.  Go to _Setup > Company > Subsidiaries_.
    
2.  Click **Edit** next to the subsidiary record.
    
3.  In the **Transaction Number Prefix** field, enter the prefix.
    
    For example, for Subsidiary A, enter **SubA**.
    
4.  If you use auto-generated numbering by subsidiary for specific transactions, click the **Transaction Numbers** subtab to specify the initial number for each transaction type.
    
    Note:
    
    To enable auto-generated numbering by subsidiary for specific transactions, go to _Setup > Company > Auto-Generated Numbers_. Click the **Transactions** subtab and then check the **Use Subsidiary** box for any transaction that should use the subsidiary's numbering.
    
    Important:
    
    If you choose to auto-number by subsidiary, you can't auto-number by location.
    
5.  Click **Save**.
    

### Related Topics

-   [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html)
-   [Editing Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273122.html)
-   [Deleting Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3760056730.html)
-   [Adding or Removing Nexuses from a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273510.html)
-   [Locking Transactions by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273734.html)
-   [Control Employee Access to Subsidiaries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278097.html)
-   [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
