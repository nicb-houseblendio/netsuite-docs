---
id: "section_N557476"
type: "section"
title: "Line-Level Audit Trail for Transactions"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Managing Transactions > Reviewing Transaction History > Line-Level Audit Trail for Transactions"
parent: "section_N554247"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557476.html"
anchors: ["bridgehead_N557504", "procedure_N557524", "bridgehead_3705059130"]
sha256: "465344a7b3f4ed19e54b967aff8c3e62a9b06a7a214e8c06c0337bf25f5f2b87"
---

Note:

This topic applies to System Notes only. For information about System Notes v2, see [System Notes v2 Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158108495822.html).

The audit trail for transactions lets you track updates to individual line items. You can view the audit trail for individual line items directly from each transaction record's listings for items, expenses, and journal line items.

On a transaction record, each line item includes a **History** link that you can click to open a new window displaying all updates to that particular line item. Users with the Notes Tab permission can see this link.

Note:

The line-level audit trail only tracks updates to existing line items, not their creation or deletion.

## Export Line-Level System Notes Data {#bridgehead_N557504}

In the History window, you can use buttons to export line-level history data as a CSV or XLS file. For more information about the History window's contents, see [Transaction Line-Level History Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557750.html).

## Include Line-Level System Notes in Saved Searches {#procedure_N557524}

To review the history of multiple line items at one time, create a transaction saved search that includes one or more Line System Notes fields in its results. You can also use Line System Notes fields as transaction saved search filters to return only selected line-item history data.

Note:

The Log System Notes on Update Only preference prevents NetSuite from logging system notes when records are created. When this preference is set, system notes are logged only when records are updated. See [Setting General Account Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N243797.html). Before you set this preference in an account that existed before that release, you should first review any saved searches containing system notes fields, as these searches may use data from record creation system notes. If your account includes searches that rely on record creation system notes, you can either revise the searches before setting the Log System Notes on Update Only preference, or you can leave this preference not set.

For example, a case search may use record creation system notes fields to find dates when cases were first escalated. To make this search work with the Log System Notes on Update Only preference set, you would need to edit this search to use expressions and to return values for cases' Date Created field if the escalation date wasn't available through record update system notes fields.

For custom transaction body fields, if the Log System Notes on Update Only preference isn't set, and you have the View access level to a field, the default value of your custom transaction body field is displayed in system notes fields when you create a transaction search. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

## Other Ways to View System Notes {#bridgehead_3705059130}

-   You can view system notes for an individual transaction on the transaction record. Go to the System Information subtab, then click System Notes. For more information, see [Viewing Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555355.html).
    
-   To view system notes for multiple transactions, filtered by field values, go to _Transactions > Management > View Audit Trail_. For more information, see [Using the Transaction Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556825.html).
    
-   You can search system notes at Reports > New Search. The system note search includes system notes for records other than transactions. This search has different filters and more features than the transaction audit trail and enables you to export data, use advanced filters and results options, and create saved searches. For more information, see [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).
    

### Related Topics

-   [Reviewing Transaction History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554247.html)
-   [Transaction System Information and Communication Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554714.html)
-   [Granting User Access to Transaction History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555081.html)
-   [Viewing Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555355.html)
-   [Using the Transaction Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556825.html)
-   [Tracking Financial Account Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557197.html)
-   [Transaction Line-Level History Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557750.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
