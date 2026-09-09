---
id: "section_N1483674"
type: "section"
title: "Creating Expense Allocation Schedules"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Expense Allocation Overview > Creating Expense Allocation Schedules"
parent: "section_N1483457"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483674.html"
anchors: ["procedure_N1483932"]
sha256: "a838e95cdd253e806d30573d6bdb4c08fbae06ad4280418e7756df62067c5786"
---

You create allocation schedules to manage the allocation of expenses after they're incurred. Allocation schedules distribute expenses across departments, locations, classes, and custom segments, saving you the time required to enter complex journal entries.

Important:

Your user role must have Edit or Full level of the Create Allocation Schedules permission to use Expense Allocation.

With Expense Allocation, you can allocate:

-   from one account or from multiple accounts
    
-   to specific department, class, or locations within expense accounts
    
-   from one account to multiple accounts
    

The Dynamic Allocation feature extends the existing fixed rate revenue and cost allocation capability. With fixed rate allocation, you must specify the fixed allocation weight for the entire life cycle of any allocation schedule. Dependent upon the Statistical Accounts feature, Dynamic Allocation lets you assign any statistical account to any Single or Intercompany Allocation Schedule. Statistical account assignment is useful in advanced costing such as Activity Based Costing and Usage Based Costing, and when you're running cost centers and profit centers. The weight for the allocation, based on the balance of that statistical account through statistical journals or as an absolute value, is dynamically calculated when the allocation journal is generated. To calculate statistical weight, NetSuite uses the flat amount for each destination line in the allocation schedule, rather than dividing by the total amount entered in all of the destination lines.

Note:

You can control the period of time that NetSuite uses to calculate the balance (weight timeline) by specifying the timeline end date through the Next Date field. This end date can be the date on which the schedule runs (system date), or a past or future date. When you select the weight basis (specific date, period to date, quarter to date, or year to date), your weight timeline is relative to the date you enter in the Next Date field. This is useful when you want an allocation schedule to calculate a statistical account balance for a period of time prior to or after the run date. For example, you want to run your allocation schedule on March 3, 2015 (system date) for the February previous period, February 1 through 28, 2015. You also specify the Next Date field as February 28, 2015 to synchronize the source and weight basis timeline to February 1 - 28, 2015. With the new synchronized weight enhancement, the source timeline, created journals, **and** the weight timeline are driven by the value in the Next Date field. For more information, see [Working with Allocation Schedules Weighted by the Balance of a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3866895958.html).

Important:

If you intend to create dynamic allocation schedules based on a statistical account, the segments you define in the statistical account are the only segments that can be used in the allocation schedule. For example, if you want to allocate cost by subsidiary and department, the statistical account must also be segmented by subsidiary and department.

When you're creating an expense allocation schedule, keep in mind the following questions to set up a schedule to best meet your needs:

-   Is the amount being allocated from one account or several accounts?
    
    On the Source subtab, you can choose one or more accounts from which to take an amount.
    
-   When you allocate the amount from this source, do you want to move the amount or allocate for reporting purposes?
    
    -   To add the amount to the destination account **and zero the balance in the source account**, only select an account in the Account field on the Source subtab. **Don't** choose a Credit Account.
        
        When you don't select a credit account, an offsetting credit **isn't** created, so the amount is transferred out of the source account.
        
    -   To add the amount to the destination account **and leave the balance in the source account**, select an account in the Account field on the Source subtab **and** choose a Credit Account.
        
        Selecting a credit account creates an offsetting credit so the amount isn't transferred out of the source. Doing so lets you look at the expense multiple ways on the Income Statement. For example, you can allocate portions of one rent expense (source) account into several departments (destination). This lets you view expense reports by department for budget planning, but leaves the actual expense amount in the source account. For example, to allocate $10,000 from the Rent Expense account to several departments.
        
        Whether you choose a credit account determines what happens to the amount you allocate from the source account:
        
        -   When you **do** choose a credit account, $10,000 is allocated to the appropriate destination accounts **and** the $10,000 balance remains in the Rent Expense account because an offsetting credit is created.
            
        -   When you **don't** choose a credit account, $10,000 is allocated to the appropriate destination accounts to credit the rent expense and the source account balance is reduced to zero.
            

-   Is the amount being allocated into one account or several accounts?
    
    On the Destination subtab, you can choose one or more accounts into which to add an amount.
    
-   If the Multi-Book Accounting feature is provisioned in your account, you can create an expense allocation schedule for a secondary accounting book. NetSuite first calculates the source balance to obtain the destination balance in the secondary book. Then, after the allocation schedule runs, NetSuite sets the source balance to zero. When you create an expense allocation schedule for all active accounting books, NetSuite generates book-specific allocation journal entries for open accounting periods for all active accounting books.
    
-   If you enable the **Values are percentages** option, you can enter a percentage as a Weight value for each destination account or custom segment, department, class, location, and custom segment.
    
-   If you enable the **Use source/credit account** option, the destination lines should be custom segments, departments, classes, locations, and custom segments within accounts specified on the Source subtab.
    
    Note:
    
    If you're creating a dynamic allocation schedule for a statistical account, the **Destination** subtab includes the **Update Sample Weights** button. Clicking this button calculates and displays the **Sample Weight** and **Balance** values for each destination line.
    

After you know the answer to these questions, follow the steps below to set up your allocation schedule.

When you use NetSuite OneWorld in conjunction with the Expense Allocation feature, you can create an intercompany allocation schedule. Intercompany schedules allocate a balance from one source subsidiary to multiple destination subsidiaries for costs that are shared between subsidiaries on a regular basis such as rent utilities. For more information, see [Creating Intercompany Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html).

#### To create an expense allocation schedule: {#procedure_N1483932}

1.  Go to _Transactions > Financial > Create Allocation Schedules_.
    
2.  In the Primary Information section:
    
    1.  Enter a name for this allocation schedule.
        
    2.  If you use NetSuite OneWorld, select the subsidiary with which this expense allocation schedule should be associated.
        
        Note:
        
        If the subsidiary you select is assigned to one or more shared vendor records, you can specify that the source account and destination account belong to any of the vendors to which the selected subsidiary is assigned. To do this, on the **Source** and **Destination** subtabs respectively, select the shared vendor from the **Name** field. For more information about shared vendor records, see [Assigning Subsidiaries to a Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4180576581.html).
        
    3.  If you use Multi-Book Accounting, select an accounting book from the list.
        
        You may select the primary book or any secondary book to which you have access.
        
    4.  In the **Frequency** field, choose how often you want to reallocate expenses from this account.
        
        You aren't required to enter a date in the **Next Date** field if you choose **End of Period** as the allocation frequency.
        
        Only those allocation schedules where the selected **Frequency** is **Run by Batch** can be included in an allocation batch. For more information, see [Creating an Allocation Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867806074.html).
        
    5.  In the **Next Date** field, enter the date of the next scheduled allocation.
        
        You can control the period of time that NetSuite uses to calculate the balance (weight timeline) by specifying the timeline end date through this field. This end date can be the date on which the schedule runs (system date), or a past or future date. When you select the weight basis (specific date, period to date, quarter to date, or year to date), your weight timeline is relative to the date you enter in the **Next Date** field.
        
    6.  In the **Subsequent Date** field, enter the date of the following allocation.
        
    7.  If you chose **Twice a Month** in the **Frequency** field, enter the day of the month that the second allocation occurs.
        
    8.  Choose one of the following:
        
        -   **Remind Forever** - Choose this option if you want to indefinitely reallocate based on this schedule.
            
        -   **Number Remaining** - Choose this option if you want to limit the number of times this schedule reallocates expenses. Enter the number of reallocations you want this schedule to make.
            
    9.  Select or clear the **Inactive** box to enable or deactivate the allocation.
        
        This option doesn't delete the allocation schedule.
        
    10.  In the **Allocation Mode** field, choose whether the schedule is a fixed allocation or dynamic allocation.
         
         If you choose **Dynamic Allocation**, complete the following fields:
         
         1.  In the **Weight Source** field, choose the statistical account upon which this dynamic allocation schedule is based.
             
             The **Unit Type** field displays the unit of measure type associated with the selected statistical account.
             
             The **Unit of Measure** field displays the base unit assigned to the **Unit Type**.
             
         2.  In the **Date Basis** field, choose the method by which the system should sum the statistical journals for weight calculation.
             
             Available options include:
             
             -   **As of Date** - The system sums all statistical journals from the beginning date to the day before the date you enter in the **Next Date** field.
                 
             -   **Period to Date** - The system sums all statistical journals from the first day of the Accounting Period to the day before the date you enter in the **Next Date** field.
                 
             -   **Quarter to Date** - The system sums all statistical journals from the first day of the quarter to the day before the date you enter in the **Next Date** field.
                 
             -   **Year to Date** - The system sums all statistical journals from the first day of the year to the day before the date you enter in the **Next Date** field.
                 
3.  Complete the **Source** subtab:
    
    1.  If you want to create an offsetting credit for the amount you're allocating, select the account for the offsetting credit to post to in the **Credit Account** field.
        
        -   If you **do** choose a Credit Account:
            
            The schedule creates an offsetting credit to balance the allocation so the amount remains in the source account and isn't transferred out of the source account by the allocation journal entry. The schedule adds the amount to the destination account for reporting purposes and leaves the actual balance in the source account.
            
        -   If you **don't** choose a Credit Account:
            
            The schedule zeroes the balance in the source account when the amount is transferred into the destination account by the allocation journal entry because an offsetting credit isn't created.
            
    2.  If you're creating an offsetting credit for the credit account selected, associate the offsetting credit with a project or entity by selecting them in the **Credit Name** field.
        
    3.  If you're creating an offsetting credit for the credit account selected, associate the offsetting credit with a department, class, and location by selecting them in the **Credit Location**, **Credit Class**, and **Credit Department** fields.
        
        To associate an offsetting credit with a department, class, and location, the **Allow Per-Line Classifications on Journals** preference must be enabled. See [Class, Department, Location Journal Entry Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1469649.html).
        
    4.  In the **Account** column, choose the account or the type of account you're allocating with this schedule.
        
        If you choose an account type instead of a specific account, all accounts of this type are allocated with this schedule.
        
    5.  In the **Name** column, select a customer, employee, project, or vendor to associate the allocation from the chosen account (d).
        
    6.  Choose the department, class, location, or custom segment to associate with allocation from the chosen account (d).
        
    7.  Click **Add**.
        
    8.  Repeat these steps for each account that you want to allocate with this schedule.
        
4.  Complete the **Destination** subtab:
    
    1.  If you want to allocate expenses into custom segments, departments, classes, and locations by percentage, check the **Values are percentages** box.
        
    2.  If you want to allocate to custom segments, departments, classes, and locations within the source account, check the **Use source/credit accounts** box. If you check this box, you can't choose destination accounts because the allocation distributes the expenses among custom segments, departments, classes, and locations rather than different accounts.
        
        If you're creating a dynamic allocation schedule for a statistical account, the **Destination** subtab includes **Update Sample Weights**. Clicking this button calculates and displays the sample weight and balance for each destination line.
        
        From the **Name**, **custom segment**, **Department**, **Location**, and **Class** fields you can select **\-Auto Populate-**. Rather than entering a fixed value, NetSuite searches all existing values at the time the allocation journal is generated and completes these fields according to the gathered information, resulting in one allocation journal destination line for each value in the field.
        
        For fixed allocations, if more than one field is set to **\-Auto Populate-**, NetSuite will generate a destination line for every possible combination of values for each segment, filtered by subsidiary restrictions and any other restrictions at the segment level. For example, if you select an account and select -Auto Populate- for Name, Department, and Location, NetSuite will generate destination lines for every possible valid combination of values from the Name, Department, Location fields. This could potentially create several destination lines that exceed NetSuite's 10,000 line limit, causing an error.
        
        For dynamic allocations, destination lines are created only for all existing combinations in the statistical account. Selecting -Auto Populate- for more than one field can still produce more than 10,000 destination lines; however, it's less likely than with fixed allocations.
        
        Note:
        
        If **Name**, **custom segment**, **Department**, **Location**, and **Class** aren't defined at the line level on the field set to **\-Auto Populate-**, NetSuite doesn't display the line because there is no assignment.
        
    3.  If you're entering values as percentages, you can use the following buttons to distribute the allocated amounts:
        
        -   **Normalize** - This button makes total weight add up to 100%.
            
        -   **Even Spread** - This button makes all the weights equal.
            
    4.  If you're allocating to other accounts, select an account in the **Account** column.
        
    5.  In the **Name** column, select a customer, employee, project, or vendor to associate the allocation to the account on this line.
        
    6.  Choose the location, department, class, or custom segment to which you want to allocate expenses.
        
    7.  In the **Weight** column, enter:
        
        -   a percentage, if you checked the **Values are percentages** box
            
        -   a flat amount that is divided by the total amount of all entered lines to determine allocation
            
            For example, if you enter 100, 300, 400 on three lines, the system would allocate the source amount to the destination lines based on the calculated percentage: 12.5% (100/800), 37.5% (300/800), 50% (400/800).
            
            Note:
            
            If you're creating a dynamic allocation schedule for a statistical account, NetSuite calculates the statistical weight using the flat amount for each destination line in the allocation schedule, rather than dividing by the total amount entered in all of the destination lines. The statistical weight is calculated when the allocation schedule is running and then used in allocation journal generation.
            
5.  Click **Save**.
    

After you create an expense allocation schedule, journal entries are created whenever you have a scheduled allocation. For more information, read [Creating Expense Allocation Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484411.html).

### Related Topics

-   [Expense Allocation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html)
-   [Creating Expense Allocation Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484411.html)
-   [Creating Intercompany Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html)
-   [Viewing the Details of Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869578910.html)
-   [Expense Allocation Assignment to Projects and Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1485952.html)
-   [Creating an Allocation Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867806074.html)
-   [Working with Allocation Schedules Weighted by the Balance of a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3866895958.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
