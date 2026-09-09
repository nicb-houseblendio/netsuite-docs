---
id: "section_N1038939"
type: "section"
title: "Mass Updating Sales Teams"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Setting Up SFA > Team Selling > Mass Updating Sales Teams"
parent: "section_N1037318"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038939.html"
anchors: ["bridgehead_4575379984"]
sha256: "f95fdaa392c76dd736f1dd65d1fddb1560271db868758aa4b89bfc4fcbf1a024"
---

Mass updates let you update a sales rep's membership of a sales team across multiple customer accounts. NetSuite uses mass updates on saved search criteria and applies updates to the employees list on the Sales Team submenu on Company records. There are three types of Sales Team Member updates and the setup process is the same for all of them. For an explanation of what each type of update does, see [Sales Team Member Mass Update Types](#bridgehead_4575379984).

Note:

Administrators should enable the Team Selling feature to use Sales Teams.

#### To perform a mass update of sales team members:

1.  Administrators, go to Lists > Mass Update > _Lists > Mass Update > Mass Updates_.
    
2.  Click **Sales Force Automation** to open the menu.
    
3.  Select the required type of **Team Member** mass update.
    
4.  Add a name for the update in the **Title of Action** field.
    
5.  Select the **Employee** you want the update criteria to apply to.
    
6.  Select a **Sales Role** from the list.
    
7.  On the **Criteria** subtab, add the required fields to filter your results.
    
8.  Complete fields from additional subtabs as needed.
    
9.  Click **Save**.
    
10.  Go to _Lists > Mass Update > Saved Mass Updates_
     
11.  Click **Preview** alongside the required saved mass update.
     
12.  Click **Perform Update** to update the selected records.
     

## Sales Team Member Mass Update Types {#bridgehead_4575379984}

There are three types of sales team related mass updates:

-   **Add Sales Team Member** - Adds an employee to the sales team assigned to customers
    
    NetSuite adds employees with sales rep roles as non-primary sales team members with 0% contribution percentage.
    
-   **Remove Sales Team Member** - Removes an employee from sales teams
    
    NetSuite removes employees with a sales rep role if their contribution percentage is 0%.
    
-   **Replace Sales Team Member** - Replaces an existing sales team member with another employee
    
    NetSuite gives the new employee the same contribution percentage, sales role, and primary or non-primary status as the member being replaced.
    
    When you perform this update, first select the team member to replace in the Replace Team Member field. This filters the search results to only show customers whose sales team includes the employee being replaced.
    
    NetSuite doesn't update if the employee replacing another team member is already on the sales team.
    

### Related Topics

-   [Team Selling](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1037318.html)
-   [Mass Updates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1103335211.html)
-   [Setting Up a Sales Team](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1039448.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
