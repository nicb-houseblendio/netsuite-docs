---
id: "section_N1483457"
type: "section"
title: "Expense Allocation Overview"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Expense Allocation Overview"
parent: "chapter_N1468455"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html"
anchors: []
sha256: "40290856cc17d4dfa16debb2ca23eaf8077a7db682545eeba50d4721a287aec0"
---

The Expense Allocation feature lets you account for fixed expenses without having to split them among individual departments or locations in advance of incurring the expenses. Later, you can transfer expenses into different accounts and assign the expenses to specific departments, classes, or locations. An administrator can enable the Expense Allocation feature at _Setup > Company > EnableFeatures_ > Accounting subtab.

The Accounting Periods feature must be enabled to use Expense Allocation.

Important:

Your user role must have Full level of the Create Allocation Schedules permission to use Expense Allocation.

Expense allocation is managed by allocation schedules. You set up allocation schedules to allocate, or transfer, balances from expense accounts into one or more other accounts. You can choose the date and frequency with which expenses are allocated on an ongoing basis. You create an allocation schedule at _Transactions > Financial > Create Allocation Schedules_. For more information, see [Creating Expense Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483674.html).

Note:

When you use NetSuite OneWorld in conjunction with the Expense Allocation feature, you can create an intercompany allocation schedule. Intercompany schedules allocate a balance from one source subsidiary to multiple destination subsidiaries for costs that are shared between subsidiaries on a regular basis, such as rent utilities. For more information, see [Creating Intercompany Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html).

For each scheduled allocation, a journal entry is automatically created. For more information, see [Creating Expense Allocation Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484411.html).

You can be reminded when allocations are due in the Reminders portlet on your dashboard. To set a reminder for allocation schedules that are due, go to the Home tab and click Customize this Page. In the Add Content panel, click or drag and drop the Reminders Item. In the Reminders portlet, click the Set Up link. In the Set Up Reminders dialog, check the Allocation Schedules Due box, and click Save. Click the reminder in the portlet to view and approve allocation journal entries.

If you've enabled both the Statistical Accounts and the Dynamic Allocation features, you can assign any statistical account to any allocation schedule. The weight for the allocation, based on the balance of that statistical account through statistical journals or as an absolute value, is dynamically calculated when the allocation journal is generated. This is useful in advanced costing such as Activity Based Costing and Usage Based Costing, and when you're running cost centers and profit centers. To calculate statistical weight, NetSuite uses the flat amount for each destination line in the allocation schedule, rather than dividing by the total amount entered in all of the destination lines.

Note:

You can control the period of time that NetSuite uses to calculate the balance (weight timeline) by specifying the timeline end date through the Next Date field. This end date can be the date on which the schedule runs (system date), or a past or future date. When you select the weight basis (specific date, period to date, quarter to date, or year to date), your weight timeline is relative to the date you enter in the Next Date field. This is useful when you want an allocation schedule to calculate a statistical account balance for a period of time prior to or after the run date. For example, you want to run your allocation schedule on March 3, 2015 (system date) for the February previous period, February 1 through 28, 2015. You also specify the Next Date field as February 28, 2015 to synchronize the source and weight basis timeline to February 1 - 28, 2015. With the new synchronized weight enhancement, the source timeline, created journals, and the weight timeline are driven by the value in the Next Date field. For more information, see [Working with Allocation Schedules Weighted by the Balance of a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3866895958.html).

### Related Topics

-   [Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1468455.html)
-   [Journal Entries Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1468996.html)
-   [Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469391.html)
-   [Making Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1469880.html)
-   [Journal Entry Approval Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471271.html)
-   [Reversing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1471552.html)
-   [Viewing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472027.html)
-   [Printing Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472381.html)
-   [Importing a Journal Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1472877.html)
-   [Journal Entries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1475513.html)
-   [Bad Debt Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481280.html)
-   [Writing Off Customer Overpayments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483085.html)
-   [Period End Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531269686.html)
-   [Balancing Segments and Journals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157358611227.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
