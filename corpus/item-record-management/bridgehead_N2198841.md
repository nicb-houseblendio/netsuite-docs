---
id: "bridgehead_N2198841"
type: "bridgehead"
title: "Inventory Costing Recalculations on Inventory Adjustments"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Costing > Inventory Costing Recalculations > Inventory Costing Recalculations on Inventory Adjustments"
parent: "section_N2197365"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2198841.html"
anchors: ["bridgehead_N2198871", "bridgehead_N2198913", "bridgehead_4031308600", "bridgehead_N2198943", "bridgehead_4550117824"]
sha256: "30c27f562d83f2fd5b997ae8feb1969d939d3eaee753d32f2ee48ff7ce336df9"
---

When you enter an inventory adjustment or inventory adjustment worksheet and use the current date, you don't need to recalculate inventory costing. However, if you back-date the adjustment, inventory costing recalculations may be required.

-   A back-dated inventory adjustment worksheet recalculates inventory costing on all items.
    
-   A back-dated inventory adjustment recalculates inventory costing only for the items on the adjustment.
    

How long the recalculation takes depends on how much data is affected by the change.

## Recalculation Time {#bridgehead_N2198871}

Typically, NetSuite can complete the calculations required to update the costing history for a particular item in as short as a few hours. This is true if you enter transactions on the same day that they occur. If you change information about a purchase at the beginning of the item's history, that change can affect the costing on all subsequent sales.

Usually, long-running recalculations happen when you edit a transaction from early in the item's history. Editing the transaction history of many different items also result to slow recalculations. In that case, the recalculation should go through all subsequent transactions for that item to evaluate what costing adjustments need to be made.

For example, you insert a transaction dated one year before the current date. There were many transactions entered between the date you added the transaction and today. These transactions need an inventory costing update. Another example, you changed a transaction from two years ago, but since then you only entered a few transactions with that item. In that case, there isn't much data to recalculate.

## Inventory Costing Recalculations and Reports {#bridgehead_N2198913}

When you run a report, you might see a message about inventory costing calculations.

If you change items on a transaction that have inventory impact and update costing history, NetSuite may need to recalculate the costing for those items. These calculations can run immediately or overnight.

When NetSuite runs these calculations, you'll see a message on any affected report. The message indicates that the report values might change when the calculations are complete.

After the inventory costing recalculations complete, the message no longer appears when you view the report.

Select **Display Title** from report **Options** to read the messages.

## Inventory Costing and Closed Accounting Periods {#bridgehead_4031308600}

If you reopen a previously closed accounting period and then edit an inventory transaction from that period, note the following. The costing changes you enter for items on the changed transaction carry over to all subsequent related transactions. Therefore, you should run a complete inventory costing recalculation.

Important:

Before you close the accounting period again, make sure the recalculation is done. If you close the period while inventory costing is still being calculated, it can affect costing accuracy and cause errors.

## Transaction Changes Trigger Inventory Costing Recalculations {#bridgehead_N2198943}

When you make certain changes to a transaction, NetSuite recalculates inventory costing for the items on that transaction. Here are some transaction changes that trigger an inventory costing recalculation:

-   changing an item
    
-   changing the item quantity
    
-   changing a unit price
    
-   changing serial or lot numbers
    
-   changing the date
    
-   changing the order total
    
-   changing the taxes charged
    

### Limit Inventory Costing Triggers {#bridgehead_4550117824}

To limit the inventory costing triggers, set the **Create and Edit Inventory Transactions Dated in Closed Periods** accounting preference.

This preference can prevent changes to transactions that would result in inventory costing calculations in closed periods.

-   If you clear this box, it prevents changes to transactions that would result in inventory costing calculations in closed periods.
    
-   If you check this box, it lets you make some changes to transactions that would trigger inventory costing calculations in closed periods. However, changes in some fields can trigger inventory costing calculations for an item even without posting to the general ledger. These changes can cause inventory costing errors and failures. Therefore, you should disable this preference.
    

An administrator can set this preference. For more information, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

You can also manage settings for accounting periods to block some changes to posting transactions after the period is locked.

The **Allow Non-G/L Changes** box only appears after you lock a period to transactions.

-   If you check this box, anyone with the **Allow Non G/L Changes** permission can make changes to posting transactions that don't affect the general ledger, even after the period is locked. These changes can trigger inventory costing recalculations. Examples of fields that don't trigger inventory costing changes include bin, class, department, and memo.
    
-   If you clear this box, you can't change posting transactions after the period is locked.
    
    Clearing this box helps prevent inventory costing problems by blocking closed period changes to fields on transactions that can impact costing.
    
    You also can't add or remove transaction lines.
    

For more information about the **Allow Non G/L Changes** setting for periods, see [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html).

### Related Topics

-   [Inventory Costing Recalculations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2197365.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
