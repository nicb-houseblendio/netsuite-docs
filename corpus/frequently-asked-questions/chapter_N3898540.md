---
id: "chapter_N3898540"
type: "chapter"
title: "FAQ: SFA & Marketing"
branch: "frequently-asked-questions"
category: "additional-resources"
breadcrumb: "Additional Resources > Frequently Asked Questions > FAQ: SFA & Marketing"
parent: "book_N3895042"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3898540.html"
anchors: ["bridgehead_N3898553", "bridgehead_N3898570", "question_N3898583", "question_N3898620", "question_N3898658", "bridgehead_N3898686", "question_N3898703", "bridgehead_N3898733", "question_N3898750", "bridgehead_N3898775", "question_N3898792", "question_N3898838", "bridgehead_N3898863", "question_N3898880", "question_N3898914", "question_N3898952", "bridgehead_N3898980", "question_N3899002", "question_N3899070", "question_N3899196", "question_N3899918", "question_N3899955", "bridgehead_4297960564", "bridgehead_3891067203", "bridgehead_3891066856", "question_N3900159", "question_N3900187", "question_N3900220"]
sha256: "5ee3d90b538207fa1b6f1d63b00ca0c13279d12ac1b222f8c7671d1c815f439a"
---

## Sales Force Automation {#bridgehead_N3898553}

See the questions and answers below for information on Sales Force Automation.

## Sales Territories {#bridgehead_N3898570}

### How do sales territories route my leads? {#question_N3898583}

When leads are entered into NetSuite, they are compared to the criteria in your sales territories. If a lead matches a territory's criteria, it is assigned to the territory.

Leads are compared to territories in the order you set. To prioritize your sales territories, go to Setup > Sales > Sales Territories. On the Manage Customer Territories subtab, click on a territory, and drag it up or down to change the priority of a territory.

For information on setting up sales territories, see [Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html).

### How do I reassign leads, prospects and customers after I update my territories? {#question_N3898620}

To reassign customers, you first create a group containing the customers you want to reassign at Leads > Groups > New. Then, go to Setup > Sales > Sales Territories, and click the Reassign Existing Customers subtab. Select the group of customers you want to reassign. You can clear the box in the Reassign column next to any customers you do not want to reassign. Click Save.

After reassigning leads, prospects and customers, new territories show on the record, and they are assigned to sales reps in that territory.

For more information, see [Reassigning Customers to Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1042981.html).

### Why don't my reps appear in the Sales Rep field? {#question_N3898658}

Only employees that are marked as sales reps on their employee records appear in the Sales Rep field on transactions, customer records, quotas, commission schedules and sales territories.

To mark an employee as a sales rep, a Sales Administrator can go to _Lists > Employees > Employees_. Click Edit next to an employee that is a sales rep. On the employee record, click the Human Resources subtab. Check the Sales Rep box, and click Save.

For more information, [Marking an Employee as a Sales Rep](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039206.html).

## Quotas {#bridgehead_N3898686}

### How do I view a list of quotas? {#question_N3898703}

You can view a list of quotas at Forecast > Establish Quotas > List. Be sure to set filters at the bottom of the page to **All** to see all the quotas assigned to your reps.

For more information, see [Quotas](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1043179.html).

## Opportunities {#bridgehead_N3898733}

### Who should use opportunities? {#question_N3898750}

Opportunities are most useful for those companies that have a longer sales cycle that involve multiple estimates and offerings. Opportunities allow you to log all the activity (meetings, phone calls, e-mail messages, etc.) associated with a deal. If your sales process is efficient and straightforward or if you rarely create multiple estimates for a single deal, you probably do not need to use opportunities.

For more information on opportunities, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).

## Forecasting {#bridgehead_N3898775}

### Why aren't my opportunities showing on forecast reports? {#question_N3898792}

Forecast reports include estimates and opportunities that have **expected close dates** within the date range of the report, not transaction dates.

Additionally, make sure that the probability of the estimate or opportunity exceeds the minimum forecast probability set by your Sales Administrator at _Setup > Sales > Preferences > Sales Preferences_. This company preference determines which estimates and opportunities are included in your company's forecast reports.

For more information, see [Opportunities in the Forecast and Pipeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047903.html).

### How do I set a default probability for opportunities and estimates? {#question_N3898838}

An administrator or sales administrator can set the probability that appears by default on new estimates and opportunities at Setup > Sales > Sales Preferences. The probability can be changed from the default on an individual transaction basis.

For more information, see [Sales Force Automation Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035924.html).

## Commissions {#bridgehead_N3898863}

### How do I know which transactions determine commission amounts? {#question_N3898880}

View the Commission Overview Report at Reports > Commissions > Commission Overview.

For more information, see [Commission Overview Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1154819.html).

### Can I import commission data from other applications? {#question_N3898914}

Yes. To import commission amounts, click Import on the Authorize Commissions page. A dialog appears with a link to download the CSV template you can use to import commission with.

When you want to import the commission amounts, click the Import button, select the file on your computer, and the amounts are listed for authorization.

For more information, see [Importing Employee Commission Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1154345.html).

### How do I set default commission expense accounts? {#question_N3898952}

All authorized employee and partner commission transactions must post to an expense account. The expense account drop-down field on the Transactions > Commissions > Authorized Employee/Partner Commissions page will default to the first available expense account if a default account is not specified.

To setup a default expense account, go to Setup > Sales > Commissions. Choose expense accounts in the Default Employee/Partner Commissions Expense Account fields, and click Save.

For more information, see [Commission Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1122601.html).

## Marketing Automation {#bridgehead_N3898980}

### What kinds of groups can I create? {#question_N3899002}

A group is a set of employees, contacts, customers, partners or vendors. You can create static or dynamic groups:

-   A **static group** is created by selecting members form a list or by performing a search. New members can be manually added to the group or a mass update can be performed to update the group members.
    
-   A **dynamic group** is created from a saved search. Group members are automatically updated based on the current results of the saved search.
    
    For example, you can create an employee group of all sales reps. A new employee who is created as a sales rep is automatically added to the group. An existing employee who switches positions and is no longer a sales rep is removed from the group. You do not need to manually maintain the group.
    

To create a group, go to _Commerce > Marketing > Personalization > Groups > New_.

For more information, see [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html).

### How do I create a group? {#question_N3899070}

There are several ways to create a group:

-   **From List** - Select group members from a list of records in your account.
    
    For example, if you click Select Customers under the From List heading, you choose individual customers from your customers list to be included in the group.
    
    Groups created with the From List options are static groups.
    
-   **With New Search** - Search for group members by selecting criteria for the people you want to include in the group.
    
    For example, you can click Search Customers and search for customers assigned to a certain sales rep. Then, you can make a group of all customers that were returned from the search.
    
    You can create either static or dynamic groups from the With New Search options.
    
-   **With Existing Saved Search** - Create a group from an existing saved search in your account.
    
    Groups created from saved searches are dynamic and constantly updated every time a new record is entered that matches the criteria of the search.
    

For example, if you have an existing saved search for customers with a certain sales rep, you can click Saved customer Search and create a group based on the search results. Any new customer who is assigned to that sales rep is then automatically added to the group.

For more information, see [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html).

### How do I perform a letter merge with Microsoft Word 2002/XP? {#question_N3899196}

The Mail Merge feature in NetSuite can be used to create form letters from information in your NetSuite account. The merge creates a zip file containing the individual letters.

To perform a letter merge, download the sample source file from NetSuite, and use it to create your letter template. Then, you can upload your template and perform the merge in NetSuite.

For more information, see [Merging Letters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525062.html).

### How do I perform a bulk email merge? {#question_N3899918}

The Mail Merge feature allows you to send personalized email in bulk to those you do business with. Messages can include CRMSDK tags which will be replaced with information from the recipients record when the email is merged and sent.

To perform a bulk email merge, first create an email template you want to use to generate the email you send. Then, create a group of recipients. Finally, go to Documents > Mail Merge > Bulk Merge.

For more information on email merge, see [Merging Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html).

### How is bounced campaign email handled? {#question_N3899955}

There are many reasons email is not delivered successfully, or bounced. Hard bounces occur when the email address is invalid or because the recipient's email server is blocking NetSuite's server. Soft bounces are due to temporary issues. NetSuite tracks the reason an email message bounced on the campaign response record for each recipient.

When a message sent to an email address results in a hard bounce, that email address is marked as a hard bounce address. Hard bounced addresses are not sent email through marketing campaigns for a set period of time. To choose how long the bounce history of an email address is maintained, go to _Setup > Company > Email > Email Preferences_, and select the required number of days from the **Remove email addresses from Bounced Email Address list after** list.

## Display Bounce Warning on Campaigns {#bridgehead_4297960564}

NetSuite can automatically scan your marketing campaign list for previously hard bounced email addresses and provide real time notification of entities associated with a bounced email address (1). To set this preference, go to _Home > Set Preferences > Optimizing NetSuite_. Clear this box if you wish to restrict automatic scanning of hard bounced email addresses in your marketing campaign. If the preference is turned off, a bounced list button is enabled (2), allowing manual screening of hard bounced email addresses. Disabling this preference is useful if you have a large campaign distribution list. For large lists, automatic screening may cause performance issues when viewing campaign records.

![Display warning example on marketing campaign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AdditionalResources/FrequentlyAskedQuestions/FAQSFAMarketing_hard_bounce.png)

## Hard Bounce Reasons {#bridgehead_3891067203}

-   Unknown User
    
-   Bad Domain
    
-   Address Error
    
-   Account Closed
    
-   Hard Bounced - Other
    

## Soft Bounce Reasons {#bridgehead_3891066856}

-   Mailbox Full
    
-   Disabled Account
    
-   Greylisted
    
-   Server Too Busy
    
-   Soft Bounce - Other
    

### Related Topics

-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)
-   [Managing Bounced Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869562023.html)
-   [Merging Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html)

### How much storage space do I have in my NetSuite account? {#question_N3900159}

To view how much storage space you have, log in to NetSuite 360, and click the Storage Info tab.

If you wish to purchase additional storage space or have questions about your storage, please contact your account manager.

### How do I publish a knowledge base? {#question_N3900187}

You can publish a knowledge base to a tab or category in your external or intranet site. To do this, go to _Lists > Support > Knowledge Base_.

For more information, see [Publishing a Knowledge Base](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2448614.html).

### Why are my Outlook Integration buttons missing? {#question_N3900220}

If you have Outlook Integration installed and the Save in NetSuite buttons are missing, please attempt one or all of the following steps to try and resolve the problem:

1.  In Windows, navigate to Start > Settings > Control Panel > Add/Remove Programs.
    
2.  **Is Microsoft .NET Framework 2.0 installed?**
    
    **If so, uninstall Microsoft .NET Framework 2.0.**
    
3.  In Outlook, navigate to Help > About Microsoft Outlook.
    
4.  Click Disabled Items.
    
5.  **If Outlook Integration for NetSuite is listed, re-enable Outlook Integration.**
    
    In Outlook, go to Tools > Options. On the Other tab, click the Advanced Options button. In the Advanced Options dialog, click the COM Add-Ins button.
    
    In the COM Add-Ins dialog, check the box next to NetSuite for Outlook. (If NetSuite for Outlook is not listed, click the Add button, and enter the following path in the Add Add-In dialog: C:\\Program Files\\NetSuite\\Outlook\\NSAddinShimS, then click OK.)
    
    After you have checked NetSuite for Outlook, click OK.
    
6.  **Is the Outlook Integration for NetSuite listed?**
    
    **If so, make sure that the Outlook Integration for NetSuite is checked.**
    
    Note:
    
    Highlight Outlook Integration for NetSuite and take note of any information in the Location and Load Behavior field. This information will be useful should you need to call NetSuite customer support.
    
7.  If none of these suggestions fix the problem, try uninstalling and reinstalling Outlook Integration.
    

### Related Topics

-   [NetSuite for Outlook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html#bridgehead_1493220061)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
