---
id: "section_N2304987"
type: "section"
title: "Simple Inventory Distribution"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Inventory Management Setup > Distributing Inventory > Simple Inventory Distribution"
parent: "section_N2304534"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304987.html"
anchors: ["procedure_N2305049"]
sha256: "9ae13015b14ad2b2174b1b57bc2f75a58ffb7875f1fede3666588be9f4351029"
---

A Simple Inventory Distribution is the simplest way to distribute inventory. All of your inventory is distributed to a single location and transfer requests are created for inventory that needs to be relocated. No details are entered to distribute particular items and amounts to specific locations. It is intended that these details are to be entered at a later date.

Using the Simple method is ideal if you want to get started with inventory transactions right away and you are able to wait to specify particular quantities for each location.

You can alternatively choose to enter a Manual Inventory Distribution. For more information, read [Manual Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305248.html).

Warning:

You should not delete or change inventory transactions dated prior to an inventory distribution, as this can cause difficulties maintaining accurate inventory data.

#### To enter a Simple Inventory Distribution: {#procedure_N2305049}

1.  Go to _Transactions > Inventory > Distribute Inventory_.
    
2.  Click **Simple**.
    
3.  The **Date** field autofills with the current date. You can select or enter another date.
    
    Note:
    
    If you postdate this distribution transaction, be sure that the date you choose is after the date of any other postdated inventory transactions, especially transactions not associated with locations.
    
4.  Select the posting period you want to post this distribution to. If a period is closed, you cannot post to that period.
    
5.  In the **Ref. No.** field, enter information to identify this distribution in a list of other transactions. If you have enabled auto-generated numbering, this will autofill.
    
    Auto-generated numbering is enabled at _Setup > Company > Auto-Generated Numbers_. On the **Transactions** subtab, check the box in the **Allow Override** column next to **Inventory Distribution**.
    
6.  In the **Variance Account** field, select an account for this distribution. Usually, an expense account for inventory distribution is selected here.
    
7.  In the **Location** field, select the one location you are distributing ALL items into.
    
8.  Select a **Department** or **Class** if you track them.
    
9.  In the **Memo** field, enter a memo to identify this inventory distribution.
    
10.  In the item list shown, you can review the items and quantities that will be distributed. You cannot make changes to this list.
     
     Click the arrow in the field above the **Total Stock** column to select additional items to review.
     
11.  Click **Save**.
     

After you save a distribution, you can enter inventory transactions.

It is important to enter a Manual Inventory Distribution at a later point in time if choose to do a Simple Distribution to maintain accurate inventory records for all of your locations.

### Related Topics

-   [Multi-Location Inventory Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html#bridgehead_162032472912)
-   [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html)
-   [Manual Inventory Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2305248.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
