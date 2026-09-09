---
id: "section_N525062"
type: "section"
title: "Merging Letters"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge > Merging Letters"
parent: "section_N523426"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525062.html"
anchors: ["bridgehead_N525184", "procedure_N525229", "bridgehead_N525401", "procedure_N525458"]
sha256: "46893355d5e5bee6f9255603feb3b48bb259f41f4df46ada5b7c9e6c332095a9"
---

Note:

This topic is unrelated to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

In NetSuite, the Mail Merge feature provides the following two merging capabilities:

-   [Merging Individual Letters](#bridgehead_N525184): creates a single letter to send to an individual.
    
-   [Merging Letters in Bulk](#bridgehead_N525401): creates letters to send to a group of customers or contacts.
    

## Merging Individual Letters {#bridgehead_N525184}

Before you can do a letter merge to an individual, you'll need to:

-   Create a letter template file in Microsoft Word. For information, see [Using Letter Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525773.html).
    
-   Create a letter template record in NetSuite.
    

#### To merge a single letter: {#procedure_N525229}

1.  Go to Lists > Relationships to find the recipient for your letter merge.
    
    Note:
    
    You can merge any type of relationship record except Groups and Competitors.
    
2.  Select the type of relationship.
    
3.  Enable **Edit** on the **List Page**.
    
4.  In the **New** column next to the recipient's name, select **Letter**.
    
5.  The Letter Merge popup window shows the recipient selected, by default.
    
6.  Click the **Template** tab.
    
7.  Select the template you want to use.
    
    Note:
    
    You must have an existing letter template. See [Using Letter Templates in Microsoft Word](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4235216905.html)
    
8.  In the **Subject** field, update the subject of this template, if required.
    
9.  Optional. Enter a memo for internal information. This recipient won't see this memo.
    
10.  Check the **Record Merge** box to have a record of this merge appear on the recipient's record at Communications > Messages.
     
11.  Click **Merge**.
     

After you click **Merge**, NetSuite downloads the merged letter to your computer. You can print or save the merged letter.

## Merging Letters in Bulk {#bridgehead_N525401}

Before you can do a bulk mail merge operation with your NetSuite data, you'll need to:

-   Create a letter template file in Microsoft Word. For information, see [Using Letter Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525773.html).
    
-   Create a letter template record.
    
-   Create a group record for the recipients of the letter. For more information, see [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html).
    

#### To perform a bulk letter merge: {#procedure_N525458}

1.  Go to Documents > Mail Merge > Bulk Merge.
    
2.  On the Select Output page, click **Letter**.
    
3.  On the **Recipients** subtab, in the **Group Type** field, select the type of group to send the letters to.
    
4.  In the **Group** field, select a group.
    
    Note:
    
    For groups with more than 100 members, NetSuite schedules and sends the bulk letter merge operations within an hour of submission. For groups with fewer than 100 members, NetSuite sends the bulk letter merge operations at submission. You can't send bulk letter merge operations to groups with more than 4000 members.
    
5.  Click the **Template** subtab.
    
6.  In the **Template** field, select the template you want to use for this merge.
    
7.  In the **Subject** field, enter the subject of the letters.
    
8.  Click **Actions** > **Merge**.
    
    The Mail Merge Confirmation page opens. To view Bulk Merge History, go to Documents > Mail Merge > Merge History.
    

After you complete a bulk letter merge, NetSuite sends an email message to your account with a link to download the file. You can also download the file from the Merge History Page. For more information see, [Viewing Bulk Merge History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4230927265.html).

### Related Topics

-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)
-   [Working with Mail Merge](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N523426.html)
-   [Viewing Bulk Merge History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4230927265.html)
-   [Using Letter Templates in Microsoft Word](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4235216905.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
