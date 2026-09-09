---
id: "section_N1195767"
type: "section"
title: "Project Task Attributes Table"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Tasks > Project Task Attributes Table"
parent: "section_N1192913"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1195767.html"
anchors: []
sha256: "03c9186a2952c37a432c77182b11948d5bafc3fdfb2ef99058f670977a7f39b1"
---

The table below explains how some project task record fields work differently at different stages of the project.

For each project task field below, you'll see how it works at the following stages:

-   Before Baseline - This is the planning stage of a project before a baseline is set.
    
-   After Baseline - This is the planning stage of a project after a baseline is set, but before a task starts.
    
-   Active Project Stage - This is when work has begun on project tasks.
    
-   Project Task Completion - This is when the project task is marked complete.
    

| Task Field Name | Field Data Function |
| --- | --- |
| **Start Date** |  |
| Before Baseline | The estimated start date for the project task. You can change it at this stage, but it may affect dependent task start and end dates for Fixed Start constraint tasks. Otherwise, this date depends on other task dependencies and work. |
| After Baseline | The estimated start date for the project task. If you change this date (or change dependent tasks in a way that impacts this date) after the baseline is set, it's still only an estimate. It won't change the baseline date for which variance will be recorded. Note: If you set a new baseline, the value in the Start Date field will replace this value and all previous history will be lost. |
| Active Project Stage | The actual date the project task started. After time is entered against the task, this field is set to the date of the first time entry against the task. |
| Project Task Completion | The actual date the project task started. After time is entered against the task, this field is set to the date of the first time entry against the task. |
| **Baseline Start Date** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The value in the Start Date field when the baseline is set. Start date variance will be recorded against this field. Note: If you set a new baseline, the value in the Start Date field will replace this value and all previous history will be lost. |
| Active Project Stage | The value in the Start Date field when the baseline is set. Start date variance will be recorded against this field. Note: If you set a new baseline, the value in the Start Date field will replace this value and all previous history will be lost. |
| Project Task Completion | The value in the Start Date field when the baseline is set. Start date variance will be recorded against this field. Note: If you set a new baseline, the value in the Start Date field will replace this value and all previous history will be lost. |
| **Start Date Variance** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The difference between the Baseline Start Date and the estimated Start Date. |
| Active Project Stage | The difference between the Baseline Start Date and the estimated Start Date. |
| Project Task Completion | The difference between the Baseline Start Date and the estimated Start Date. |
| **End Date** |  |
| Before Baseline | The estimated end date for a project task. This date is derived from the estimated work and other task dependencies. |
| After Baseline | The estimated end date for a task. You can change this date only by changing one of the following:
-   the amount of work
-   resources assigned
-   dependency relationships for a certain task
-   changing other tasks that have dependencies with this task

 |
| Active Project Stage | The estimated end date for a project task. You can change this date only by changing one of the following:

-   the amount of work
-   resources assigned
-   dependency relationships for a certain task
-   changing other tasks that have dependencies with this task

 |
| Project Task Completion | After the project task is marked complete, the end date becomes the actual end date, based on the last time entry. After that, the task won't appear as an option in time entry forms. |
| **Baseline End Date** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The End Date value when the baseline is set becomes the Baseline End Date. All end date variance is recorded against this date. Note: If you set a new baseline, the value in the End Date field will replace this value and all previous history will be lost. |
| Active Project Stage | The End Date value when the baseline is set becomes the Baseline End Date. All end date variance is recorded against this date. Note: If you set a new baseline, the value in the End Date field will replace this value and all previous history will be lost. |
| Project Task Completion | The End Date value when the baseline is set becomes the Baseline End Date. All end date variance is recorded against this date. Note: If you set a new baseline, the value in the End Date field will replace this value and all previous history will be lost. |
| **End Date Variance** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The difference between the baseline end date and the estimated end date. |
| Active Project Stage | The difference between the baseline end date and the estimated end date. |
| Project Task Completion | The difference between the baseline end date and the actual end date. |
| **Estimated Work** |  |
| Before Baseline | The estimated work for the project task. You can change it at this stage, but it may affect start and end dates for dependent tasks. |
| After Baseline | The estimated work for the project task. If you change this after the baseline is set, it's still only an estimate. The baseline work is still recorded for variance purposes. Note: If you set a new baseline, the value in the Start Date field will replace this value and all previous history will be lost. |
| Active Project Stage | The estimated amount of work for a project task. If you change this after task work has started, it affects the entire project schedule, such as dates for other tasks and variances. |
| Project Task Completion | After a project task is marked complete, the value in this field is set to the sum of all time entries entered against the task. |
| **Actual Work** |  |
| Before Baseline | This field doesn't have a value until time has been entered against a scheduled project task. |
| After Baseline | This field doesn't have a value until time has been entered against a scheduled project task. |
| Active Project Stage | The actual time entered against a scheduled project task. |
| Project Task Completion | The actual time entered against a scheduled project task. |
| **Baseline Work** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The value in the Estimated Work field at the time the baseline is set. |
| Active Project Stage | The value in the Estimated Work field at the time the baseline is set. |
| Project Task Completion | The value in the Estimated Work field at the time the baseline is set. |
| **Remaining Work** |  |
| Before Baseline | The estimated work minus the actual work. Until the task has started, this is equal to estimated work. |
| After Baseline | The estimated work minus the actual work. Until the task has started, this is equal to estimated work |
| Active Project Stage | The estimated work minus the actual work. |
| Project Task Completion | After a task is marked complete, this is always 0. |
| **Work Variance** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The difference between the baseline work and the estimated work. |
| Active Project Stage | The difference between the baseline work and the estimated work. Note: This doesn't update as work is completed, it's based on the overall task estimate. |
| Project Task Completion | The difference between the estimated work and the actual work. |
| **Percent Complete** |  |
| Before Baseline | N/A - Actual Work / Estimated Work = 0 |
| After Baseline | N/A - Actual Work / Estimated Work = 0 |
| Active Project Stage | Actual Work / Estimated Work |
| Project Task Completion | After a task is marked complete, this is always 100% |
| **Estimated Cost** |  |
| Before Baseline | The estimated cost of the labor associated with a task. This only has a value after work and resources are assigned. |
| After Baseline | The estimated cost of the labor associated with a task. Changing the amount of work or the resources assigned will affect this value. |
| Active Project Stage | The estimated cost of the labor associated with a task. Changing the amount of work or the resources assigned will affect this value. |
| Project Task Completion | The estimated cost of the labor associated with a task. Changing the amount of work or the resources assigned will affect this value. |
| **Actual Cost** |  |
| Before Baseline | This field doesn't have a value until time has been entered against a scheduled task. |
| After Baseline | This field doesn't have a value until time has been entered against a scheduled task. |
| Active Project Stage | The actual cost of the time entered against the task. |
| Project Task Completion | The actual cost of the time entered against the task. |
| **Baseline Cost** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The estimated cost of the labor resources \* the estimated work assigned to a task. |
| Active Project Stage | The estimated cost of the labor resources \* the estimated work assigned to a task. |
| Project Task Completion | The actual cost of the labor resources \* the actual work completed on a task. |
| **Estimated Cost Variance** |  |
| Before Baseline | This field doesn't have a value until a baseline is saved. |
| After Baseline | The difference between the baseline cost and the estimated cost. |
| Active Project Stage | The difference between the baseline cost and the estimated cost. |
| Project Task Completion | The difference between the baseline cost and the actual cost of the completed task. |

### Related Topics

-   [Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html)
-   [Project Task Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192913.html#bridgehead_N1192945)
-   [Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Scheduling Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199494.html)
-   [Assigning Resources to Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200642.html)
-   [Importing Project Tasks from Microsoft Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1200868.html)
-   [Including CRM Tasks in Project Totals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201405.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
