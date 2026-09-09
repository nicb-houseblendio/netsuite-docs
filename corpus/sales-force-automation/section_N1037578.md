---
id: "section_N1037578"
type: "section"
title: "Setting Up Team Selling"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Team Selling > Setting Up Team Selling"
parent: "section_N1037318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037578.html"
anchors: ["bridgehead_N1037602", "procedure_N1037631", "bridgehead_N1037970", "procedure_N1038030"]
sha256: "87055c434a040287b504a69bf1b7f8a5a827345110153feec601287bae3e542a"
---

You create sales teams to include all of the employees who work together to close deals. You assign each member of a sales team a sales role that describes what they do in the sales process.

## Creating a Sales Role {#bridgehead_N1037602}

Before you create a sales team, you need to create sales roles and assign them to your employees.

Note:

Team Selling includes the Sales Rep sales role, by default. If you let sales team contributions go over 100%, you also need to create an adjustment rep sales role. For more information about overassignment, see [Overassignment and Adjustment Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038328.html).

#### To create a sales role: {#procedure_N1037631}

1.  Go to _Customers > Other > CRM Lists_.
    
2.  Click **Sales Role**.
    
3.  Enter a name and description for the role.
    
4.  If this is a role assigned to sales reps, check the **Sales Rep** box.
    
    Employees with sales rep roles appear on sales reports and KPIs.
    
5.  Click **Save**.
    

Next, select the role in the Sales Role field on the **Human Resources** subtab of each employee's record.

## Creating a Sales Team {#bridgehead_N1037970}

After you assign sales roles, you can create a sales team record.

Sales teams in NetSuite are groups of employees. Each employee has a set contribution percentage. A member's contribution percentage determines how much of a transaction's total counts for commission, quota, and sales forecast.

For example, a sales rep has a 10% contribution percentage in their sales team. When a sale closes, they earn 10% of the commission they'd get if they were the only rep on the deal.

When you create a sales team, you choose the primary sales member when you check the Primary box next to the member's name. Only the primary sales rep can edit the sales forecast for team transactions. Additionally, the primary sales rep shows up on sales reports in the Primary Sales Rep column.

#### To create a sales team: {#procedure_N1038030}

1.  Go to Setup > Sales > Sales Management > Sales Teams > New.
    
2.  Enter the name of the sales team.
    
3.  Select the owner of the group.
    
4.  If this group has an email alias in your email application, enter that address in the **Email** field.
    
5.  On the **Members** subtab, do one of the following to add members to this group:
    
    -   To add individual members, enter the member's name in the **Name** column, or search from the list. Select a member, and then click **Add**. Repeat these steps for each member.
        
    -   Click **Add Multiple,** and then press and hold CTRL to select more than one member from the list.
        
    -   Click **Add With Search** to enter search criteria for the members you want to add.
        
6.  In the **Access Level** column, select how much access each member has to the group's calendar and events.
    
7.  The employee's sale role appears in the **Sales Role** column, but you can change it for this sales team.
    
8.  Check the box in the **Primary** column if this employee is the lead for this team.
    
9.  In the **Contribution %** column, enter each member's default contribution percentage.
    
    Note:
    
    You can use the Allow Overassignment in Sales Team preference. Go to _Setup > Sales & Marketing Automation > Sales Preferences_.
    
    You can adjust a team member's contribution percentage later in the **Contribution %** column on individual sales transactions or customer records.
    
10.  Click **Add**.
     
11.  Repeat these steps for each member of the group.
     
12.  If you allow contribution overassignment, select an adjustment rep for each manager on the team. For more information, read [Overassignment and Adjustment Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038328.html).
     
13.  Click **Save**.
     

Now you can assign this sales team to customers and sales transactions.

### Related Topics

-   [Overassignment and Adjustment Reps](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038328.html)
-   [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html)
-   [Split Commission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1148007.html)
-   [Estimates and Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1047809.html)
-   [Opportunities and Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1048674.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
