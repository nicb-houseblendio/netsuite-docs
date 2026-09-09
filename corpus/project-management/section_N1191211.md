---
id: "section_N1191211"
type: "section"
title: "Classifying Time for Projects"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Managing Time and Expenses for Project Resources > Classifying Time for Projects"
parent: "section_N1190979"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1191211.html"
anchors: ["bridgehead_N1191527", "bridgehead_N1191561"]
sha256: "b8900d051bf773d803b0379728abb81eea46d6737f60b2ca6472c5c76c25c943"
---

You can set up how time entries are classified by default when resources enter time against projects they work on. This determines how project time is entered and used in calculations for project utilization and productivity.

Time that resources enter against a project can be classified as utilized time, productive time, or exempt. This helps you accurately calculate utilization and productivity for resources on projects.

For more information about utilization and productivity, read [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html).

The classification of time as utilized, productive, or exempt is sourced from the setting on the project record.

Note:

Time that's entered against a customer without a project is set as utilized and productive but not exempt, by default. Time entered without a customer is not utilized, not productive, and not exempt.

You can control how resource utilization is calculated for both the numerator and denominator, giving you more flexibility.

#### To classify time entered on project records:

1.  Go to Lists > Relationships > Projects.
    
2.  Click **Edit** next to a project in the list to open the record.
    
3.  Click the **Preferences** subtab.
    
4.  Check or clear the following boxes to set these defaults:
    
    -   **Classify Time as Utilized**
        
        When this box is checked, time entered on this project is marked as Utilized time by default.
        
    -   **Classify Time as Productive**
        
        When this box is checked, time entered on this project is marked as Productive time by default.
        
    -   **Classify Time as Exempt**
        
        When this box is checked, time entered on this project is marked as Exempt time by default.
        
        Any time that shouldn't be included in the denominator of utilization calculations should be identified as exempt.
        
    
    ![Preferences\_subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/Preferences_subtab.png)
5.  Click **Save**.
    

When you save these time settings for each project, they're used for all time entries associated with the project.

The following are available time classification data that are displayed in the [Utilization by Resource Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3748733226.html).

-   **Exempt hours**
    

Time that shouldn't be considered for utilization calculations in either the numerator or the denominator. Time included in this category generally includes vacations and holidays.

Companies have different ways of deciding what counts as Net Time in the denominator. Exempt time can provide flexibility in this area. Any time that shouldn't be included in the denominator can technically be marked exempt in the time entry.

-   **Net hours**
    

Time that can be utilized for productive activities.

Calculated as: \[Available time minus Exempt time.\]

-   **Utilized hours**
    

Time that's directly tied to revenue generation for a project. Examples are billable time or non-billable time on a fixed bid project.

-   **Utilization**
    

The percentage of utilization for project resources.

Calculated as: \[Utilized time / Net Time.\]

-   **Productive hours**
    

Time that isn't directly tied to generating revenue, but is important for the project. Examples are time investments for training, pre-sales support, and non-billable support roles.

-   **Productivity**
    

The percentage of productivity for project resources.

Calculated as: \[Productive time / Net Time.\]

## Customize Time Forms and Customer Records to Classify Time {#bridgehead_N1191527}

You can also customize time entry forms to show classification boxes and then classify each time entry individually. For more information about customizing time entry forms, see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

To see how individual time entries are classified on a project, you can customize the list view on the Schedule subtab of the Project record or the Time Tracking subtab of the Project Task record. You can add both the Utilized and Productive columns to either of these lists to view the time classification of individual tasks. For more information, see [Customizing List Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N496170.html).

## Assess Time Reports {#bridgehead_N1191561}

After resources enter time on projects, those entries are classified as productive or utilized based on your settings. This data is used in [Utilization by Resource Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3748733226.html), where you can assess time and expense management for your projects.

### Related Topics:

-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Entering Time Against Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1191698.html)
-   [Restricting Time Entry on Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192197.html)
-   [Entering Project Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192533.html)
-   [Approving Time and Expenses for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192683.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
