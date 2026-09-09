---
id: "section_N645835"
type: "section"
title: "Tips for Defining Simple Search Filters"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining a Simple Search > Tips for Defining Simple Search Filters"
parent: "section_N645582"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N645835.html"
anchors: ["bridgehead_N645984"]
sha256: "f823bd295b43805339d791b2417c6b3acd54fa4a17ec0d8543da1cc340444e35"
---

NetSuite provides many dropdown lists and popup windows to help you set up filters. For additional information, see the following tips.

-   Search date filters provide many options. For more information, see [Defining Search Date Filters](#bridgehead_N645984).
    
-   To avoid seeing multiple lines for each transaction in transaction searches, add a filter of **Main Line is True** or click **Yes** for the **Main Line** field. For more information, see [Main Line in Transaction Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4459563851.html).
    
-   Select **any of** to include all the values you select and **none of** to exclude them.
    
-   For fields with multi-select boxes, hold Ctrl to select more than one value.
    
-   For some text fields, select **starts with** or **contains** if you know only part of the name or title.
    
-   For searches that support keywords, use **OR** (in uppercase) to search for more than one text string at the same time.
    
-   When you enter text, use **%** to match any group of characters and **\_** for a single character. For example, searching for **aa%r fra%i** finds Aaron Frankenstein and Frangelica Aardvark.
    
-   If you enter only numbers, you only get advanced matches unless you add the % wildcard.
    
-   In some fields, select **\-Unassigned-** to find transactions not linked to an employee **\-Mine-** for transactions linked to you, or **\-My Team-** for yours and your team's.
    
-   When you select the **ANY** operator for a field, this filter isn't used in the search.
    
-   If you add a value when **ANY** is selected, the operator changes to 'has keywords' for text fields or 'equal to' for number fields by default.
    

## Defining Search Date Filters {#bridgehead_N645984}

NetSuite provides three types of date filters: a named time period, like **last fiscal year**, a custom date range with specific start date and end date, and a relative date range based on a quantity of days, weeks, months, quarters, or years **ago** or **from now**.

Some date fields let you add specific times of day in custom date ranges or named time periods like today, tomorrow, and yesterday. You can't use relative date range filters for these fields.

-   In the first **Date** dropdown list, select the search logic. You can apply any of the options to a named time period, but select **within** or **not within** for custom or relative date ranges.
    
-   In the second dropdown list, select a named time period, or select **custom** to define start and end dates in the **From** and **To** fields, or select **relative** to set a relative date range.
    
-   To set a custom date range, click the calendar icons to enter a starting date in the **From** field and an ending date in the **To** field.
    
-   To add specific times of day in custom range or named date filters like today, tomorrow, and yesterday, select the times in the **From** and **To** dropdown lists, or type them in the fields next to the dropdown lists.
    
    Note:
    
    The times that you enter for date filters adjust automatically for each user's time zone.
    
-   To set a relative date range, enter the start and end numbers and select the units (days, weeks, months, quarters, or years; ago or from now) from the dropdown lists in the **From** and **To** fields.
    
    Be sure to set the earlier date (for example, **90 days ago** ) in the **From** field, and the later date (for example, **0 days ago** ) in the **To** field.
    

### Related Topics

-   [Defining a Simple Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N645582.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
