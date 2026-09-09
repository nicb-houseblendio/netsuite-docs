---
id: "section_N1456591"
type: "section"
title: "Inventory Tasks on the Period Close Checklist"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Close > Inventory Tasks on the Period Close Checklist"
parent: "section_N1452509"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1456591.html"
anchors: ["bridgehead_N1456681", "procedure_N1456712", "bridgehead_N1456890", "procedure_N1456922", "bridgehead_0919021216", "bridgehead_N1456987", "procedure_N1457015", "bridgehead_N1457127", "bridgehead_N1457172", "procedure_N1457192", "bridgehead_4031311797", "bridgehead_4291874269", "procedure_4291874653", "bridgehead_4291872339"]
sha256: "832deb5ae1e4c5bac11a3ab995d65805064f1f392054863987ff7f2e67471dba"
---

If you use the Inventory feature, the Period Close checklist includes checks for inventory cost and quantity inconsistencies. When you close an accounting period, you can correct inventory with a negative count and run an inventory costing calculation.

To access the Period Close checklist, you can go to Manage Accounting Periods page at _Setup > Accounting > Manage GL > Manage Accounting Periods_. In the **Checklist** column, you can click the checklist icon to open the checklist for a period. Each checklist shows these inventory tasks, some of which may be available with additional features.

1.  [Resolve Date/Period Mismatches](#bridgehead_N1456681)
    
2.  [Review Item Line/Inventory Detail Quantity Mismatch](#bridgehead_0919021216)
    
3.  [Review Negative Inventory](#bridgehead_N1456987)
    
4.  [Review Inventory Cost Accounting](#bridgehead_N1457172)
    
5.  [Review Inventory Activity](#bridgehead_4291874269)
    

You must mark each of these inventory tasks complete to proceed to subsequent tasks until you close the period.

## Resolve Date/Period Mismatches {#bridgehead_N1456681}

You can reconcile transactions that are not dated within the corresponding financial period. For example, the selected posting period could be January 2014 whereas the transaction date was December 2013. Having mismatched transaction dates can cause inventory issues.

Warning:

it's strongly recommended that all inventory posting transactions have the correct alignment of the transaction date and the accounting period. A misaligned date and accounting period on a transaction may lead to inconsistent asset and inventory costing values in the accounting period.

The Transactions with Date/Period Mismatch page enables you to resolve issues for mismatched transactions that are dated outside of the selected posting period. This helps ensure that transaction and period dates are properly aligned.

To open this task on the checklist, you must have already completed the **Lock All** task.

#### To resolve mismatched dates: {#procedure_N1456712}

1.  Go to _Setup > Accounting > Manage GL > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for a period.
    
3.  Click the **Go To Task** arrow icon next to **Resolve Date/Period Mismatches**.
    
4.  The Resolve Date/Period Mismatch page shows your progress for this task. The **System Notes** subtab displays a record of each change and the name of the user that entered it.
    
    The first time that any task is viewed, System Notes logs a Create entry.
    
5.  Click **Resolve Date/Period Mismatches**.
    
6.  On the Resolve Date/Period Mismatches page in the **Period** field, select a period for which you want to resolve mismatches.
    
    For example, if you select the period January 2014, the list shows any transactions that have a posting period during January 2014 but are dated outside of the period range, from January 1 through January 31.
    
7.  After you select a period, the page shows a list of transactions that have a mismatched posting period and transaction date.
    
    For each transaction, the following data shows:
    
    -   Transaction Type
        
    -   Transaction Number
        
    -   Transaction Date
        
    -   Period Name
        
    -   Period Start
        
    -   Period End
        
8.  Click **Edit** next to a transaction to modify.
    
    After the transaction opens, edit it to amend either the posting period or the transaction date so that the two correctly match.
    
9.  Save the transaction.
    
    Repeat all steps for any remaining mismatched transactions.
    

After you have matched the transaction date and posting period for all transactions on the Resolve Date/Period Mismatch page, you can mark the task complete.

## Completing the Task {#bridgehead_N1456890}

To mark the task complete, go to _Setup > Accounting > Manage GL > Manage Accounting Periods_ and click the **Go To Task** arrow icon next to **Resolve Date/Period Mismatches**. On the Task: Resolve Date/Period Mismatches page, click **Mark Task Complete**.

Note:

NetSuite permits you to mark the task complete even if transactions remain mismatched and are not dated within the corresponding financial period. If the task is marked complete when mismatched dates are left unreconciled, the Close Period Checklist logs the date and the user who marked the task complete.

## Mismatched Transaction Handling Preference {#procedure_N1456922}

To establish preventive measures to avoid transactions with mismatched dates, you can set a preference for handling mismatched transaction entry. Set the preference at _Setup > Accounting> Preferences > Accounting Preferences_ on the **General** subtab.

Select one of the following for **Allow Transaction Date Outside of Posting Period**:

-   **Disallow** - When you choose this setting, users are not allowed to save a transaction unless the transaction date is within the date range for the posting period selected.
    
-   **Warn** - When you choose this setting, users are warned when a transaction date isn't within the date range for the posting period selected, but they can click **OK** on the warning and save it anyway.
    
-   **Allow** - When you choose this setting, users can enter a transaction even if the date isn't within the date range for the posting period selected. No warning is given to the user before the transaction is saved.
    

## Review Item Line/Inventory Detail Quantity Mismatch {#bridgehead_0919021216}

If you use the Advanced Bin/Numbered Inventory Management feature, the Review Item Line/Inventory Detail Quantity Mismatch task is added to your Period Close Checklist. You must mark this task complete before you can proceed to the Review Negative Inventory task.

This task enables you view the list of transactions that have quantity mismatches between item lines and their inventory details. To open the list, on the task page, click **Review Item Line/Inventory Detail Quantity Mismatch**. From the list, you can click a transaction to open it. You can review or edit details on transaction lines or inventory details to resolve the mismatch. Any resolved transactions are removed automatically from the list. To complete the task, click **Back to Period Close** to return to the task page, and then click **Mark Task Complete**.

This task doesn't require mismatches to be resolved. However, you can avoid issues with inventory balances when you resolve them for each accounting period.

## Review Negative Inventory {#bridgehead_N1456987}

When closing a period, you must identify any negative inventory values that can be corrected by a positive adjustment. Reviewing negative inventory items is a required task for the period closing checklist.

This task doesn't create a physical count. A physical count should already be completed before you begin this task.

To open this task on the checklist, you must have completed the **Resolve Date/Period Mismatches** task.

#### To reconcile negative inventory: {#procedure_N1457015}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for a period.
    
3.  Click the **Go To Task** arrow icon next to **Review Negative Inventory**.
    
    The Review Negative Inventory page opens. This page shows your progress for this task. The **System Notes** subtab displays a record of each change and the name of the user that entered the change.
    
    The first time that any task is viewed, System Notes logs a Create entry.
    
4.  Click **Review Negative Inventory**.
    
5.  On the Review Negative Inventory page, in the **As of Date** field, enter the date through which you want to review inventory. For example, if you enter January 1, 2014, the list shows inventory that has a negative count as of January 1, 2014.
    
6.  If you use the **Multi-Location Inventory** feature, you can filter the list by location in the **Location** field.
    
7.  The list of inventory items that shows identifies any items that have negative inventory.
    
    Use the list to adjust the amounts for those items so they're no longer negative. For details about entering an inventory adjustment, see [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html).
    

After you have reviewed the negative inventory items and entered the necessary adjustments, you can mark the task complete.

## Completing the Task {#bridgehead_N1457127}

To mark the task as complete, go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_ and click the **Go To Task** arrow icon next to **Review Negative Inventory**. On the Task: Review Negative Inventory page, click **Mark Task Complete**.

Note:

NetSuite permits you to mark the task as complete even if some inventory counts remain negative. If the task is marked complete when inventory counts remain negative, the Close Period Checklist logs the date and the user who marked the task as complete.

You can also access the Review Negative Inventory page at _Transactions > Inventory > ReviewNegative Inventory_.

## Review Inventory Cost Accounting {#bridgehead_N1457172}

When closing a period, you must run the costing accounting process for the period close. To complete this task, ensure that there are no costing items to be corrected and that inventory costing calculations are not already currently running.

To open this task on the checklist, you must have already completed the **Review Negative Inventory** task.

#### To review inventory cost accounting: {#procedure_N1457192}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for a period.
    
3.  Click the **Go To Task** arrow icon next to **Review Inventory Cost Accounting**.
    
4.  Click **Review Inventory Cost Accounting**.
    
    Please note the following:
    
    -   To run inventory costing calculations, there must be no items on the Review Inventory Cost Accounting page in the list of outstanding items to be corrected. If any items show on the list, you must wait until they're resolved. If an item on the list can't be resolved, you're prompted to contact customer support.
        
    -   If inventory costing calculations are currently running or are deferred, you can't click the **Review Inventory Cost Accounting** button.
        
    -   If inventory costing calculations are currently deferred, you must wait until the scheduler runs inventory costing calculations.
        
    -   If inventory costing calculations are disabled, you're prompted to contact customer support.
        
5.  After the inventory costing calculations have finished running, click **Mark Task Complete**.
    

You can also reconcile transactions that are not dated within the corresponding financial period and set a preference for handling mismatched transaction entry. For details about this checklist requirement, read [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html).

## Inventory Costing and Closed Accounting Periods {#bridgehead_4031311797}

Be aware that if you open a previously closed period and then edit an inventory transaction from that previously closed period, the costing changes you enter for items on the changed transaction do propagate to all subsequent related transactions. This requires an inventory costing recalculation to run and be completed.

Note:

Before you go back and close the accounting period again, verify that the recalculation is complete. If you close the period during the time that inventory costing is being calculated, it can affect the accuracy of your costing and potentially cause errors.

For more information, read [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)

## Review Inventory Activity {#bridgehead_4291874269}

If you use NetSuite OneWorld, this task opens a version of the Inventory Activity Detail report that you can customize. This report provides a view of specific inventory values. The report details are based on the item level total inventory value in a specific subsidiary context.

Reviewing inventory activity is a required task for the period closing checklist.

To open this task on the checklist, you must have already completed the **Review Inventory Cost Accounting** task.

#### To review inventory activity: {#procedure_4291874653}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  Click the **Checklist** icon ![Checklist icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/PeriodCheckIcon.png) for a period.
    
3.  Click the **Go To Task** arrow icon next to **Review Inventory Activity**.
    
4.  Click **Review Inventory Activities**.
    
5.  Review the Inventory Activity Detail report, filtering and customizing the report, as needed. For information about using Report Builder to customize this report, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
    
    Filter the report by subsidiary context, location, and From and To date. By default, the dates reflect the accounting period that is being closed.
    
    The standard report includes the following columns:
    
    -   Item
        
    -   Transaction Type
        
    -   Date (of transaction)
        
    -   Document Number
        
    -   Description
        
    -   Qty. (item quantity remaining)
        
    
    The report rows are grouped first by inventory activity under the Item column. For example, you have an inventory activity group for Inventory Items. When you expand the Inventory Items group, you see the #10 Envelopes subgroup. Beneath this subgroup are rows for a variety of number 10 envelopes. The last row of the subgroup provides the total of #10 Envelopes you hold in inventory.
    
    Click **Refresh** to update the report.
    
6.  When you have completed your inventory review, exit the report and then complete the task.
    

## Completing the Task {#bridgehead_4291872339}

To mark the task as complete, go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_ and click the **Go To Task** arrow icon next to **Review Inventory Activity**. On the Task: Review Inventory Activity page, click **Mark Task Complete**.

### Related Topics

-   [Accounting Period Close](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452509.html)
-   [Non-Posting Transactions in Locked and Closed Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1452887.html)
-   [Using the Period Close Checklist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1455781.html)
-   [Unlocking Period Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457300.html)
-   [Reopening a Closed Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1457543.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
