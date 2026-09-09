---
id: "section_N1039705"
type: "section"
title: "Sales Rules"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Sales Rules"
parent: "chapter_N1035717"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039705.html"
anchors: ["procedure_N1039764"]
sha256: "fcfd74da28d8ed0a814674530f1335fa35e16da39d9cc88fa68730a699efabd8"
---

A sales rule is a set of parameters for how NetSuite assigns potential customers to sales reps. Sales rules are based on standard and custom fields on lead, prospect, and customer records. For example, name, address, and phone number.

NetSuite doesn't assign a potential customer who doesn't match your sales rules, but you can assign them manually, or you can distribute them with the default Round Robin sales territory. Customers are automatically processed through the sales rules when their records are added or updated.

For example, if you have three sales reps in one city, you can make a sales rule for the city and a sales rule for each customer status. When you create the three sales territories, you can select the city rule for each sales rep in that area, but choose a different customer status for each sales rep. Now, one sales rep will be assigned leads for that city, one will be assigned prospects, and the other will be assigned customers.

#### To create a sales rule: {#procedure_N1039764}

1.  Go to _Setup > Sales & Marketing Automation > Set Up Sales Rules > New_.
    
2.  On the Select a Customer Rule Field page, click the name of the field on which you want to base this rule.
    
    The type of field you select determines what kind of criteria you can set.
    
3.  On the Customer Field Rule page, enter a name and description for this rule.
    
    The field you base this rule on is shown below the description.
    
4.  Set the criteria you want for this rule and add multiple subcriteria if needed. For example, you want to create a zip code rule that includes multiple zip codes.
    
    The criteria you can set depend on the type of field you base the rule on:
    
    -   **Numerical fields** - criteria and subcriteria based on numeric ranges
        
    -   **Text fields** - criteria and subcriteria based on number and letter content
        
    -   **Box fields** - criteria based on whether the box is checked (is Equal To) or not checked (is Not Equal)
        
    -   **List fields** - criteria based on the inclusion or exclusion of choices in preexisting lists, for example, Lead Source or State
        
    -   **Custom fields** - criteria based on the information entered in custom fields
        
5.  Set the rules for whether customers need to match all or any of the criteria and subcriteria. Availability of these options depends on the type of field you base the rule on:
    
    -   Choose **Match All Conditions** if you want customers to be assigned by this rule only if they match all criteria and subcriteria.
        
    -   Choose **Match Any Condition** if you want customers to be assigned by this rule if they meet any of the criteria or subcriteria.
        
6.  If you can select subcriteria, set them at the bottom of the page, and then click **Add/Edit**.
    
7.  Click **Save**.
    

After you create the sales territory assignment rules, group those rules into territories, and then assign the territories to sales reps. Go to _Setup > Sales > Sales Management > Sales Territories > New_.

### Related Topics

-   [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html)
-   [Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html)
-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
