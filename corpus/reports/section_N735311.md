---
id: "section_N735311"
type: "section"
title: "Scheduling a Report"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Working with Report Results > Scheduling a Report"
parent: "chapter_N717676"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html"
anchors: ["procedure_N735350"]
sha256: "fe9cc515aa643c18b6529fb053fa5c6aa69ee99a8a58296b6edfef7c962cfd01"
---

When you're viewing a report, click Schedule in the footer to set up automatic report emails. You can schedule standard and saved reports and send them to other users.

Depending on your company email settings, scheduled reports are sent using either your company or subsidiary email, or the email of the user who set up the schedule.

Important:

If the person who created the report schedule leaves the company, you can't change the "from" email. But you can recreate the schedule so reports will use your own email address. For more information about the from email addresses used for NetSuite forms, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html).

Clicking Schedule opens the Schedule Report page, where you can pick recipients, add a message, attach files, and set the report to run on a fixed schedule.

Note:

You're encouraged to run large reports during off-peak hours. If a report takes more than 3 minutes during peak hours, it's automatically disabled and you'll get an email if it times out. The report won't run again until it's edited to be faster or rescheduled for off-peak hours.

Go to _Reports > Scheduled Reports > Report Schedules_ to view a list of your scheduled reports. From the Report Schedules page, you can click Edit to revise or delete a saved schedule. For more information, see [Report Schedules Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735790.html). Expand/collapse settings are maintained for scheduled reports.

Scheduled reports in your production account aren't run in your Release Preview account, to avoid confusion. If you want a report to run on a schedule in Release Preview, you'll need to schedule it in that account.

Important:

Emails sent from NetSuite can't be bigger than 20MB. If your emailed report has non-ASCII characters, the limit might be lower due to encoding. To avoid this, narrow your results or send a link to the report.

#### To schedule a report: {#procedure_N735350}

1.  Go to Reports > Reports Overview and click the name of the report you want to schedule to run the report.
    
2.  In the footer of the report, click the Schedule button ![Footer schedule icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/FooterIconSchedule.png).
    
3.  On the Schedule Report page, enter a name for the schedule.
    
    This name will help you identify this schedule on the Report Schedules list.
    
4.  Enter the date for the report to run. If the report is to be run more than one time, then this date will be the date that the schedule becomes active.
    
5.  Enter the start time for the report. If the time you select is during peak hours, this will be indicated to the right of the time field. See the preceding note about scheduling reports during off-peak hours.
    
    ![Schedule Report page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Reports/schedule3.png)
    
    Note:
    
    The date and time are set according to your timezone, as set in _Home > Set Preferences_ > General, at the time of creating the schedule. Changing your timezone will not affect the timing of existing scheduled reports.
    
6.  Check the **Run Report More Than Once** box if you want the report to run multiple times. If you select this box the page will expand to reveal further scheduling options:
    
    1.  **Daily Event** - Specify the frequency: Repeat every **X** days (also counting weekend days) or Repeat every weekday (Monday-Friday).
        
    2.  **Weekly Event** - Specify the frequency: Repeat every **X** weeks and choose which days of the week it should run.
        
    3.  **Monthly Event** - Select day **X** of every **X** months or specify the (1st, 2nd, … last) (Sunday, Monday, … Saturday) of every **X** Months.
        
    4.  **Yearly Event** - Select the date or specify the (1st, 2nd, ... last) (Monday, Tuesday, ... Saturday) of (Jan, Feb ... Dec).
        
    5.  **Start At** and **End By** - Enter the date range you want to schedule the report for.
        
        If you are scheduling a single event, the report will be emailed on the date entered in the **Start At** field.
        
        If you are scheduling a repeat event, the report will be emailed according to the schedule you set starting on the date entered in the **Start At** field and ending on the date entered in the **End By** field.
        
    6.  **No End Date** - Check this box if you want the schedule to repeat indefinitely.
        
        This field is checked by default. Entering a date in the **End By** field automatically clears this box.
        
7.  On the **Recipients** subtab:
    
    1.  The **Recipient** field is pre-filled with your email address. You can change the primary recipient by selecting from the **Recipient** dropdown list.
        
        Note that if email notifications for the report schedule fail, timed-out reports and other notifications are sent to the primary recipient. The recipients in the Cc and Bcc lists do not receive these failure notification emails.
        
    2.  In the **Copy Others** dropdown list, select an additional recipient and choose whether to include in the Cc or Bcc list, and click **Add**.
        
        Important:
        
        For security reasons, you can only pick email addresses that are tracked in your NetSuite account as recipients for a scheduled report. If you want to send the report to an email address that's not in your account, you should create a **Contact** entity. You can also create Customer, Employee, Group, Partner, or Vendor entities, but Contact is the preferred option. If you create a Group entity, reports go to the group email by default. If you want the report sent to every group member, check the **All individual group members** box.
        
        For information about how to create each entity type, see the following topics:
        
        -   [Creating a Contact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161792162006.html)
            
        -   [Creating a Customer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161860867711.html)
            
        -   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
            
        -   [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html)
            
        -   [Creating a Partner Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1166599.html)
            
        -   [Creating a Vendor Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2362161.html)
            
        
    3.  Repeat step b for each additional recipient to be copied.
        
        Note that both primary and copied recipients can be an individual user or a group. Dropdown lists include any group that has a group email address.
        
8.  On the **Message** subtab:
    
    1.  Enter custom subject and body text for email messages.
        
    2.  Choose the **Sending Format** from the list.
        
9.  On the **Attachments** subtab:
    
    1.  In the **Attach File** field, select a file from your computer or File Cabinet to attach to the email, and click Add.
        
    2.  Repeat to attach additional files.
        
    3.  Check the **Zip attachments** box if you want to attach a zip file of all selected attachments.
        
10.  Click **Save**.
     

### Related Topics

-   [Working with Report Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N717676.html)
-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
