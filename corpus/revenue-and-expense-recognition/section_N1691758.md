---
id: "section_N1691758"
type: "section"
title: "Cases When a Revenue Recognition Schedule May Not Be Created"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Working with Revenue Recognition Schedules > Cases When a Revenue Recognition Schedule May Not Be Created"
parent: "section_N1689004"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691758.html"
anchors: []
sha256: "11c2f82bf39111bd5ee61a3be02e52460cd14201af2fc1b1a28eb8fb9ccb4dba"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For information about the current feature, see [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

There are cases when a revenue recognition schedule may not be created. You can identify these cases when a line on an invoice is indefinitely deferred because the transaction line shows the template name rather than a View link or a Revenue Recognition Schedule number (if auto-numbering is on). These cases, as described below, require you to take action to move them out of the deferred state.

-   The following cases apply if the Vendor Specific Objective Evidence (VSOE) feature **is** enabled, and either the transaction is marked as a VSOE bundle or the transaction has one or more item groups marked as a VSOE bundle, as shown in the cases below:
    
    -   An invoice **is** linked to a sales order and allocation isn't completed for the sales order. The lack of allocation from the sales order carries over to the invoice and all lines in the bundle are deferred indefinitely.
        
    -   An invoice **isn't** linked to a sales order and allocation isn't completed for the invoice. All lines in the bundle are deferred indefinitely.
        
    -   An invoice **is** linked to a sales order that includes one or more lines not marked as delivered. Those lines are indefinitely deferred.
        
    -   An invoice **isn't** linked to a sales order and the invoice includes one or more lines not marked as delivered. Those lines are indefinitely deferred.
        

For information about using a report to find deferred revenue transactions, read [Sales Order Revenue Forecast Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1700969.html).

### Related Topics

-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Reviewing the Revenue Recognition Schedules List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689265.html)
-   [Viewing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689644.html)
-   [Editing a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689901.html)
-   [Mass Updating Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690102.html)
-   [Deleting a Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1690402.html)
-   [Creating a Revenue Recognition Schedule Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0822023107.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
