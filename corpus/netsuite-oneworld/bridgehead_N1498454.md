---
id: "bridgehead_N1498454"
type: "bridgehead"
title: "Key Points for Running Intercompany Elimination"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Intercompany Elimination Overview > Key Points for Running Intercompany Elimination"
parent: "section_N1498385"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498454.html"
anchors: []
sha256: "48f2972755f1bf9ac1f266003c769150e0fb6d1013634498a388aacb7f470b4b"
---

-   You can run intercompany elimination only from the Period Close Checklist.
    
-   You can run intercompany elimination for all accounting books, the primary accounting book, and any secondary accounting book.
    
-   You can run intercompany elimination multiple times for a period.
    
-   You can drill down from elimination results to view the elimination journal entries' details.
    
    Note:
    
    If you use the Use Journal Entry Summarization on Intercompany Elimination accounting preference, similar elimination journal entries are grouped into a single, summarized journal entry. See [Summarized Intercompany Elimination Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4813074258.html).
    
-   You must have the administrator role or a financial user role with period closing privilege at the parent-level to run intercompany elimination.
    
-   When you run intercompany elimination, the system runs the process for all subsidiaries in your organization. You can't eliminate intercompany transactions by subsidiary.
    
-   In multiple level hierarchies and elimination subsidiaries, NetSuite posts elimination journal entries to the elimination subsidiary for the least common parent node of both subsidiaries.
    
    -   If one subsidiary is a parent subsidiary of another, NetSuite uses the elimination subsidiary under the parent subsidiary.
        
    -   If two subsidiaries do not have a parent-child relationship, NetSuite uses the elimination subsidiary for the first level parent they have in common.
        
-   NetSuite eliminates reversal advanced intercompany journal entries (AICJE) in the same period in which they post. If you post an AICJE and its reversal AICJE in the same period, the **net** amount from the pair of elimination journal entries is 0.
    

### Related Topics:

-   [Cumulative Translation Adjustment-Elimination (CTA-E)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1498539.html)
-   [Intercompany Elimination Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498982.html)
-   [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
