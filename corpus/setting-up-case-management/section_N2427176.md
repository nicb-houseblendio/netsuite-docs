---
id: "section_N2427176"
type: "section"
title: "Setting Case Escalation Rules and Assignments"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Case Escalation Rules and Assignments"
parent: "chapter_N2421072"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2427176.html"
anchors: ["subsect_162281450139", "procedure_N2427240", "subsect_162281497461", "procedure_N2427429"]
sha256: "23a167c8fbb84b6d7ad5f561c4e1f94279f72d1ebfba480f722ad3bf13d1d04b"
---

Set up escalation rules and assignments to ensure that high priority cases are routed to the correct person at the right time.

With escalation rules, you set criteria to search cases, then create escalation assignments to group these rules. When a case matches the criteria you set, it's automatically assigned to the person or group you selected for the escalation assignment.

For example, Wolfe Electronics sells a warranty plan that guarantees cases will be resolved within 24 hours. They set up an escalation rule that uses their custom warranty field on customer records, and another rule for cases open for 12 hours or more.

Note:

NetSuite processes case escalations every five minutes, so escalation rules based on shorter time periods may not be processed when expected.

## Case Escalation Rules {#subsect_162281450139}

To set up case escalation rules, an administrator must enable the Automated Case Escalation feature. Go to Setup > Company > Setup Tasks > Enable Features. On the CRM subtab, check the Automated Case Escalation box, and click Save.

#### To create a case escalation rule: {#procedure_N2427240}

1.  Go to _Setup > Support > Escalation Rules > New_.
    
2.  Choose the field on the case record or the customer's record you want to base your rule on.
    
    With escalation rules, you can base escalation on the following amounts of time:
    
    -   Since the case was created
        
    -   Since it was last modified by the customer
        
    -   Since it was last modified by someone in your account
        
3.  Create a name for your escalation rule. You will choose this name when you group rules into assignments.
    
4.  If needed, you can enter a brief description of this rule.
    
5.  In the **Criteria** field, select terms for your search.
    
    You may also need to make selections in the field(s) below based on the case record field you're using for this rule.
    
    You can select more than one choice in the list by holding CTRL while selecting additional options with your mouse.
    
6.  Depending on the case record field you're basing the rule on, you may be able to set subcriteria for this rule:
    
    1.  Select **Match All Conditions** if you want a case to meet all the subcriteria you set to be escalated based on this rule.
        
        Select **Match Any Condition** if you want a case to meet any one of the subcriteria you set to be escalated based on this rule.
        
    2.  In the **Sub-Criteria** column, select terms for your criteria.
        
    3.  In the next column, enter or select criteria, and click **Add**.
        
7.  Click **Save**.
    

For example, Wolfe Electronics has a group of customers who have purchased a warranty plan. If they submit a case, it will be resolved within 24 hours. Wolfe can set up an escalation rule that includes every customer in this group, and another for cases open for 12 hours or more. Then they create a case escalation assignment that includes both rules and assign it to a support team devoted to resolving high priority cases.

Note:

To exclude cases from escalation based on rules, you must create rules to include only open cases and cases created after today.

## Case Escalation Assignments {#subsect_162281497461}

Case escalation assignments use rules to determine how cases are escalated and who they're escalated to.

Before you set up an escalation assignment, you should create escalation rules. For more information, see [Case Escalation Rules](#subsect_162281450139).

For example, Wolfe Electronics creates a case escalation assignment with a rule for customers who have purchased a warranty, and a rule for cases open for 12 hours or more. They then assign it to a support team devoted to resolving high priority cases.

#### To set up a case escalation assignment: {#procedure_N2427429}

1.  Go to _Setup > Support > Manage Escalation Assignments > New_.
    
2.  On the Escalation Assignment page, enter a name for this assignment.
    
3.  Enter a description for this assignment.
    
4.  Select **Match All Rules** if you want cases to match the criteria in all rules you select to be escalated by this assignment.
    
    Select **Match Any Rule** if you want cases to match any of the criteria in the rules you select to be escalated by this assignment.
    
5.  On the **Configure Rule Definitions** subtab, select a rule, and click **Add**.
    
6.  Continue adding rules if needed, and click **Add** after each rule.
    
    Note:
    
    To exclude cases from escalation based on rules, you must create rules to include only open cases and cases created after today.
    
7.  On the **Escalation Assignment** subtab, select the person or group cases that fall into the rules for this assignment should be escalated to.
    
8.  Click **Add**.
    
9.  Continue adding individuals or groups if needed, and click **Add** after each.
    
    Cases are distributed evenly to all the individuals and groups listed.
    
10.  Click **Save**.
     

After you set up escalation assignments, you can set their priority. Priorities determine which assignment a case should be classified in if it matches rules for more than one assignment.

You can change the priorities on the Manage Escalation Assignments page by clicking the handlebars next to an assignment and dragging it up or down. The first assignment in the list is the first assignment a case is sifted through. To view the rules for an assignment or make changes to an assignment, click its name in the Territory column.

### Related Topics

-   [Creating Case Profiles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3914420072.html)
-   [Assignment Rules & Territories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2426488.html)
-   [Using Email Case Capture](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2427546.html)
-   [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html)
-   [Help Desk](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2430719.html)
-   [Customizing Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2430856.html)
-   [Customizing Support Notification Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2431043.html)
-   [Setting Up Customer Support in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2433348.html)
-   [Setting Up Case Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2421072.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
