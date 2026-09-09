---
id: "section_N1035924"
type: "section"
title: "Sales Force Automation Preferences"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Sales Force Automation Preferences"
parent: "chapter_N1035717"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1035924.html"
anchors: ["bridgehead_N1035962"]
sha256: "6d5678f7724f8bc4bf1f1d95bc97cc8b933a0964c9a273ac42ca90ca3aca268c"
---

The Sales Preferences page lets sales administrators set customer status preferences that specify how your company should use the Sales Force Automation. NetSuite applies your settings to everyone with access to your account.

## General SFA Preferences {#bridgehead_N1035962}

You can set the following customer status preferences on the General subtab at _Setup > Sales & Marketing Automation > Sales Preferences_.

-   **Lead Status** - Select the default status assigned to new lead records.
    
-   **Prospect Status - New** - Select the default status assigned to prospects who do not yet have a transaction associated with them.
    
-   **Prospect Status - Opportunity** - Select the default status assigned to prospects who have an opportunity created for them.
    
-   **Prospect Status - Estimate** - Select the default status assigned to prospects who have an estimate created for them.
    
-   **Customer Status** - Select the default status assigned to customers.
    
    You can create and view customer statuses to use as defaults or to select on customer, lead, and prospect records. For information, see [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html).
    

The following are additional general preferences:

-   **Standard Sales Roles** - Choose how much restriction you want to place on standard sales roles. Choose one of the following:
    
    -   **Unrestricted** - Sales reps and managers can view and edit any records and transactions they have access to, regardless of the records assigned to them.
        
    -   **Restrict Editing Only** - Sales reps and managers can view but not edit records and transactions that are not assigned to them or their subordinates. The standard Sales Person role has employee restrictions set to self and subordinates only. The standard Sales Manager role has employee restrictions set to self, subordinates, and unassigned.
        
    -   **Restrict Editing and Viewing** - Sales reps and managers can only view or edit records and transactions assigned to themselves or their subordinates.
        
-   **Restrict by Transaction Sales Rep Only** - Check this box to let sales reps see transactions for customers they are assigned to **if** they are the rep on the transaction.
    
    If you clear this box, each sales rep can see all customer transactions, even if they're not the rep on the transaction.
    
-   **Default Estimate Expiration (in days)** - Enter the number of days after you create an estimate that you want the estimate to expire, by default. You can also change the expiration date on each estimate.
    
-   **Default Sales Effective Date to Linked Sales Effective Date** - Check this box if you want the sales effective date on credit transactions to default to the sales transaction from which it is created. For example, when you create a refund from a cash sale, the sales effective date from the transaction defaults on the refund.
    
    If you clear this box, the sales effective date is set to the transaction date.
    
    Note:
    
    With this preference, if you change the transaction date of the credit transaction, the sales effective date updates to match. For more information, see [Sales Effective Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1147809.html).
    
-   **Consider 'Starts With' Matches in Lead Conversion** - Check this box if you want companies that begin with the same name as leads to show up as possible duplicates on the Convert Lead page. For more information, see [Lead Conversion](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086628.html).
    
-   **Allow Overassignment in Sales Teams** - Check this box to let the total contribution percentage for sales reps go over 100%.
    
    If you check this box, you can add Adjustment reps at the bottom of the page. For more information, see [Creating a Sales Team](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037578.html#bridgehead_N1037970).
    
-   **Preferred Lead Form** - Select the custom form you want to use by default when you enter a lead.
    
-   **Preferred Prospect Form** - Select the custom form you want to use by default when you enter a prospect.
    
    You can create new custom entry forms. For information, see [Creating a Sales Team](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037578.html#bridgehead_N1037970).
    

If you use the Alternate Sales Amount (ASA) feature, you can also set the following preferences:

-   **Default Alternate Sales Amount to First Year Revenue** - Check this box to automatically calculate ASA as the first year's revenue for a line item.
    
    If you don't use revenue recognition, NetSuite assumes that the sales amount entered is based on a 12-month term. In this case, the ASA matches the sales amount.
    
    If you use revenue recognition, first year revenue is based on the Rev. Rec. Start, Rev. Rec. End and Rev. Term in Months fields.
    
-   **Alternate Sales Amount Name** - Enter the name you want to use for alternate sales amounts. This name appears on transactions, quotas, forecasts, and reports with ASA.
    
    For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
    
-   **Show Intelligent Recommendations Button for Item Recommendations** - Check this box to see the Intelligent Recommendations button on sales orders, estimates and opportunity records.
    
    Intelligent Recommendations uses AI to calculate and display items your customer might want to buy. For more information, see [Intelligent Recommendations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158073815739.html) and [Add Recommended Items to Sales Orders, Estimates, and Opportunities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_165021068175.html).
    

### Related Topics

-   [Customer Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1036969.html)
-   [Sales Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039705.html)
-   [Sales Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1040011.html)
-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)
-   [Forecasting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1046772.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
