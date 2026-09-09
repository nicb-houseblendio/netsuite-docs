---
id: "section_N1484654"
type: "section"
title: "Creating Intercompany Allocation Schedules"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Expense Allocation Overview > Creating Intercompany Allocation Schedules"
parent: "section_N1483457"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html"
anchors: ["svg_1", "svg_1background", "svg_1Layer_1", "svg_1Straight_Thin", "svg_1Node_1_", "svg_1Node"]
sha256: "53e1181d0ae685d007b287520017db21f9cebfe903fcc8df64ab8ddd03f7776e"
---

If you've enabled the Expense Allocation feature in your NetSuite OneWorld account, expense allocations can be made within a single subsidiary. When you create an allocation schedule, the subsidiary you select applies to both the source and the destination of the allocation.

Important:

Your user role must have Edit or Full level of the Create Allocation Schedules permission to use Expense Allocation.

Note:

If the subsidiary you select is an elimination subsidiary **and** the intercompany elimination accounts use the same elimination algorithm **and** the accounts are in balance, NetSuite automatically marks the intercompany journal lines as elimination. You can manually unmark the lines as elimination on the respective intercompany journal entry.

If the subsidiary you select is an elimination subsidiary **and** the intercompany elimination accounts **don't** use the same elimination algorithm **and** the accounts **aren't** in balance, NetSuite doesn't automatically mark the intercompany journal lines as elimination. You can manually mark the lines as elimination on the respective intercompany journal entry.

Intercompany allocation schedules distribute a balance from one source subsidiary to multiple destination subsidiaries for costs that are shared between subsidiaries on a regular basis such as rent. If the source subsidiary or any destination subsidiary is assigned to one or more shared vendor records, you can specify that the source and destination belongs to any of the vendors to which the selected subsidiaries are assigned. On the Source and Destination subtabs respectively, select the shared vendor from the Name field. For more information about shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).

If you've enabled both the Statistical Accounts and Dynamic Allocation features (_Setup > Company > EnableFeatures_ > Accounting under Advanced Features), you can assign any statistical account to any allocation schedule. The weight for the allocation, based on the balance of that statistical account through statistical journals or as an absolute value, is dynamically calculated when the allocation journal is generated. This is useful in advanced costing such as Activity Based Costing and Usage Based Costing, and when you're running cost centers and profit centers. To calculate statistical weight, NetSuite uses the flat amount for each destination line in the allocation schedule, rather than dividing by the total amount entered in all of the destination lines.

Note:

You can control the period of time that NetSuite uses to calculate the balance (weight timeline) by specifying the timeline end date through the Next Date field. This end date can be the date on which the schedule runs (system date), or a past or future date. When you select the weight basis (specific date, period to date, quarter to date, or year to date), your weight timeline is relative to the date you enter in the Next Date field. This is useful when you want an allocation schedule to calculate a statistical account balance for a period of time prior to or after the run date. For example, you want to run your allocation schedule on March 3, 2015 (system date) for the February previous period, February 1 through 28, 2015. You also specify the Next Date field as February 28, 2015 to synchronize the source and weight basis timeline to February 1 - 28, 2015. With the new synchronized weight enhancement, the source timeline, created journals, **and** the weight timeline are driven by the value in the Next Date field. For more information, see [Working with Allocation Schedules Weighted by the Balance of a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3866895958.html).

You can streamline your month-end close process by using allocation schedules to automatically create advanced intercompany journal entries that allocate shared costs or revenues.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       

For example, Subsidiary A must allocate part of a $1,000 rent expense to two other subsidiaries that are separate legal entities who share space and are responsible for their portion of the rent. For an allocation based on a percentage of square footage, an intercompany schedule can be set up to keep 50% of the $1,000 rent expense for Subsidiary A, allocate 25% to Subsidiary B, and allocate 25% to Subsidiary C.

The following are intercompany allocation schedule details:

Rent Bill Received and Paid by Subsidiary A:

Rent Expense $1,000

Cash $1,000

You enter the following intercompany allocation schedule:

-   Values are percentages = True
    
-   Use Source/credit Accounts = True
    
-   Source Account: Rent Expense
    
-   Source Subsidiary: Subsidiary A
    
-   Intercompany Clearing Account
    
-   Destination Account: Same as source
    
-   Destination Subsidiary: Subsidiary A, Weighting: 50%
    
-   Destination Subsidiary: Subsidiary B, Weighting: 25%
    
-   Destination Subsidiary: Subsidiary C, Weighting: 25%
    
-   Intercompany Clearing Account: same as source
    

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In a later release, NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. Still later, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that aren't currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

The allocation would be created as below to ensure that the books for each subsidiary reflect the correct rent expense posting:

| Journal 1: Regular Journal, only one subsidiary |
| --- |
| Rent Expense | Subsidiary A | $500 |  |
| Rent Expense | Subsidiary A |  | $500 |

| Advanced Intercompany Journal 1: Allocates to Subsidiary B |
| --- |
| Intercompany Clearing Account | Subsidiary A | $250 |  |
| Rent Expense | Subsidiary A |  | $250 |
| Rent Expense | Subsidiary B | $250 |  |
| Intercompany Clearing Account | Subsidiary B |  | $250 |

| Advanced Intercompany Journal 2: Allocates to Subsidiary C |
| --- |
| Intercompany Clearing Account | Subsidiary A | $250 |  |
| Rent Expense | Subsidiary A |  | $250 |
| Rent Expense | Subsidiary C | $250 |  |
| Intercompany Clearing Account | Subsidiary C |  | $250 |

Create a new schedule at _Transactions > Financial > Create Allocation Schedules_. For important details about creating allocation schedules, see [Creating Expense Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483674.html).

On the schedule, select a subsidiary to indicate the source from which the amounts are taken. Then, enter details on the Source subtab.

Please note the following about the source:

-   You can identify source credits in the account, name, department, class, and location fields **or** specify accounts in the account list.
    
-   The Intercompany Account is the clearing account used.
    
-   Only accounts and segments/classifications available to the source subsidiary can be selected.
    
-   The currency of the source subsidiary is the currency used on resulting journals and intercompany journals created from the schedule.
    

On the Destination subtab, select one or more destination subsidiaries into which you want the amount allocated.

Please note the following about the Destination subtab:

-   If you have checked the **Values are percentages** box, then the total must be less than or equal to 100%.
    
    If the **Values are percentage** box is clear, NetSuite calculates the percentages based on the values supplied.
    
    For example, if you enter 100, 300, 400 on three lines, NetSuite calculates 12.5% (100/800), 37.5% (300/800), 50% (400/800), where 800 is the sum of 100+300+400.
    
-   If the total is less than 100%, an amount remains in the account and the allocation can be run again.
    
-   If you have checked the **Use source/credit account(s)** box, the account and intercompany account are used on all lines.
    

Note:

All destination subsidiaries must have access to the accounts to use this selection. Subsidiaries are given access when selected on the account record.

-   Only accounts and classifications available to the destination subsidiaries can be selected.
    

At each scheduled allocation, NetSuite automatically creates an advanced intercompany journal entry for each destination subsidiary and the appropriate amount posts to the specified account.

Please note the following about journal entries created for intercompany allocation:

-   A regular journal is created for lines with the same source and destination subsidiary.
    
-   An advanced intercompany journal is created for each destination subsidiary: one journal per subsidiary. This is the case even if there are multiple lines on the allocation schedule for the same subsidiary.
    
-   Each advanced intercompany journal entry posts at least four lines, two lines for the source and two for the destination.
    
-   The journal shows a **Created from** link to the allocation schedule detail.
    

Warning:

Journals created from allocation schedules can't be directly deleted. You must first open the allocation detail and delete it, which deletes all journal entries to which it's associated.

### Related Topics:

-   [Expense Allocation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html)
-   [Creating Expense Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483674.html)
-   [Creating Expense Allocation Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484411.html)
-   [Viewing the Details of Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869578910.html)
-   [Expense Allocation Assignment to Projects and Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1485952.html)
-   [Creating an Allocation Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867806074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
