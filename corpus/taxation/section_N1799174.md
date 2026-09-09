---
id: "section_N1799174"
type: "section"
title: "Editing and Deleting Tax Periods"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Working with Tax Periods > Editing and Deleting Tax Periods"
parent: "section_N1797157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799174.html"
anchors: ["bridgehead_4637272969", "bridgehead_4637273248", "bridgehead_4637273497", "bridgehead_4637273701", "bridgehead_4637274137"]
sha256: "89de4853b8eb447c12cc93d22c75e1108faab826e7dba16e4cfe3670d532b0bf"
---

-   [Editing Tax Periods](#bridgehead_4637272969)
    
-   [Deleting a Closed Tax Period](#bridgehead_4637273248)
    
-   [Deleting a Tax Base Period](#bridgehead_4637273497)
    
-   [Deleting a Tax Quarter](#bridgehead_4637273701)
    
-   [Deleting a Tax Year](#bridgehead_4637274137)
    

## Editing Tax Periods {#bridgehead_4637272969}

-   On any tax period page, you can edit the **Period Name**, **Start Date**, **End Date**, and **Sub-period of** fields. The Edit Tax Period page provides an activity history of changes made to the period name and dates.
    
-   For closed tax periods, you can edit the **Period Name** field, **Sub-period of** field, and **Is Posting** box. You can't edit the dates.
    
-   You can change a period from posting to non-posting only if the period doesn't have transactions associated with it.
    
-   You can change a period from non-posting to posting only if the period doesn't have sub-periods.
    
-   You can't make months (base) periods non-posting because months (base) periods can only be posting. They don't have the Is Posting box.
    
-   If you're using the Multiple Calendars feature, you can edit the **Fiscal Calendar** field of a tax period record.
    

## Deleting a Closed Tax Period {#bridgehead_4637273248}

-   You can delete a closed period only if it has no transactions.
    

## Deleting a Tax Base Period {#bridgehead_4637273497}

-   You can delete a base period only if the period is open and has no transactions.
    
-   If you're using the Multiple Calendars feature, deleting a base period deletes it from all fiscal calendars.
    

## Deleting a Tax Quarter {#bridgehead_4637273701}

-   Without the Multiple Calendars feature enabled, you can delete a quarter only if it doesn't have any sub-periods, or if its base periods don't have any transactions. Deleting a quarter also deletes the base periods attached to it.
    
-   If you're using the Multiple Calendars feature, deleting a quarter reassigns its base periods to the parent year.
    

## Deleting a Tax Year {#bridgehead_4637274137}

-   Without the Multiple Calendars feature enabled, you can delete a year if there is no transaction posting to this period. Deleting a year will also delete all periods under it.
    
-   If you're using the Multiple Calendars feature, you can't delete a year if there are sub-periods under it, even if there is no transaction posting to this period.
    

### Related Topics

-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html)
-   [Tax Periods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454154841.html)
-   [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html)
-   [Closing Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1798849.html)
-   [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html)
-   [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html)
-   [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html)
-   [Reporting by Tax Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
