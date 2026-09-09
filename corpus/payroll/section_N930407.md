---
id: "section_N930407"
type: "section"
title: "Updating Payroll Information"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > SuitePeople U.S. Payroll > Payroll Setup > Updating Payroll Information"
parent: "chapter_N917379"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930407.html"
anchors: ["svg_1", "svg_1background", "svg_1Arrows", "svg_1Straight_Thin", "svg_1Swoopy_2", "svg_1Swoopy_3", "svg_1Straight_Thin_2_", "svg_1Boxes", "svg_1Node_1_", "svg_1Node", "svg_1Straight_Thin_1_", "svg_1cLOUD", "svg_1Text", "procedure_N930431"]
sha256: "c4d194138d943548e7c86737f605819e68b0da89ac2e38e93ebb85c3bc9d43af"
---

When you use SuitePeople U.S. Payroll, changes or updates made to the Set Up Payroll page must be committed to the payroll tax engine. The same is true for changes made to the employee, workplace, or payroll item records.

The Update Payroll Information page is a guide for issues that need to be resolved. It is also a reference for what changed since your last update. You must complete these steps often during setup, and anytime you change records that affect payroll.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           

To view the history of any employee payroll changes, such as pay rate increases, go to the [Employee Payroll Item History Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3814113937.html).

#### To commit payroll changes and updates: {#procedure_N930431}

1.  Go to _Setup > Payroll > Update Payroll Information_.
    
2.  If you have a NetSuite OneWorld account, select a subsidiary from the list in the **Subsidiary** field. For more information, see [Payroll Setup in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275739.html).
    
3.  On the Update Payroll Information page, review the information shown on the following subtabs:
    
    -   **Updated Records** - This subtab lists any records that have been updated since you last updated your payroll information. The record types listed may include your company record, payroll items, employees, and workplace records. You can click the name of a record in the Name column to verify any changes that you have made.
        
    -   **Employees Excluded from Payroll** - This subtabs lists employees for whom the **Include In Payroll** box is clear on the **Payroll** subtab on the employee record. You should review the list and make sure you don't want to pay these employees using NetSuite. For example, employees who work outside of the United States should appear on this list.
        
        To add an employee to your payroll, click the **Name** of the employee. Then, check **Include in Payroll** box on the **Payroll** subtab of the employee record.
        
    -   **To Resolve** - This subtab contains a list of error codes and messages for payroll-related errors that currently exist in your account. To resolve an issue, click the name of the record in the Record column.
        
    
    Important:
    
    All issues listed on this subtab must be resolved before you can run payroll.
    
4.  Read the statement that begins **I have reviewed all information...**, and then check the **Agree** box.
    
5.  Click **Commit Updates**.
    
6.  After committing your updates, check the **To Resolve** subtab again. If there are no items to resolve, you can run payroll. For more information about issues that may need to be resolved, see [Payroll Errors During Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930704.html).
    

### Related Topics

-   [Enabling Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N917966.html)
-   [Entering Company Information for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918232.html)
-   [Entering Workplace Records for Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N918520.html)
-   [Payroll Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N920073.html)
-   [Retirement Plan Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162558111263.html)
-   [Payroll Items Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N930985.html)
-   [Payroll Setup for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N921632.html)
-   [Running Test Payroll Batches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944846.html)
-   [Setting up Year-To-Date Information From Your Previous Payroll System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N944369.html)
-   [Entering a Payroll Start Date](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N945629.html)
-   [Payroll Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N917379.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
