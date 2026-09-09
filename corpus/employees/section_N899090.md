---
id: "section_N899090"
type: "section"
title: "Employee Locations"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Employee Information Management > Employee Locations"
parent: "chapter_N894090"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899090.html"
anchors: ["subsect_158801222420", "subsect_158801223669"]
sha256: "0a0e726ab04c145751ef2fb185a2ecb57b4d3ada3dc1f49fcba4f854126c6246"
---

This section contains the following topics:

-   [Associating an Employee with a Location](#subsect_158801222420)
    
-   [Restricting Employee Access by Location](#subsect_158801223669)
    

## Associating an Employee with a Location {#subsect_158801222420}

You can associate employees with a specific location to ensure that employees have access to only the information associated with that location. For example, you can restrict access for warehouse personnel who handle item receipts or fulfillments at a single location. You can also refine employee reports and searches by location.

#### To associate an employee with a location:

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the employee to whom you want to assign a location.
    
3.  Under Classification in the **Location** field, select the location of this employee.
    
    For more information, see [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html).
    
4.  Click **Save**.
    

To search for employee records based on location, go to _Lists > Employees > Employees >Search_. In the **Location** field, choose the company location whose employee records you want to access, and click **Submit**. A list of employee records for that location appears.

## Restricting Employee Access by Location {#subsect_158801223669}

Use the following procedure to restrict employee access by location.

#### To restrict employee access by location:

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_.
    
2.  Click **Customize** next to the role you would like to restrict.
    
3.  Click the **Restrictions** subtab.
    
4.  Click the blank line in the list and select **Location** from the **Segment** column.
    
5.  From the **Restrictions** column, choose a level of access for the location field on transactions and records.
    
6.  In the **Location Restrictions** field, choose a level of access for the location field on transactions and records.
    
    -   **None - default to own** - There is no restriction on what can be selected. The default selection is the location set on the user's record.
        
        All transactions and records are accessible.
        
    -   **Own, subordinate, and unassigned** - Users are restricted to records with their own location, children records of their location, and records with unassigned location field.
        
    -   **Own and subordinates only** - Users are restricted to records with their own location and children records of their location.
        
        Users can access only those transactions and records with their location or sublocations selected in the **Location** field.
        
7.  Check the **Allow Viewing** box to allow users logged in with this role to see, but not edit, data. This applies to data for employees to which the role does not have access.
    
    Important:
    
    This setting doesn't allow viewing of employee payroll or commissions data. Also, users can't view non-subordinate employee records other than their own record when the **Restrictions** column is set to **own and subordinates only**.
    
8.  Check the **Apply to Items** box to apply the department restrictions defined here to item records, in addition to transaction, employee, or partner records.
    
9.  Click **Save**.
    

### Related Topics

-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Adding Employees by Importing a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322503072.html)
-   [Editing Employee Records Using CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322804075.html)
-   [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html)
-   [Assigning a Supervisor to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898466.html)
-   [Viewing and Editing an Employee Record with Effective Dating](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494510731.html)
-   [Rehiring a Terminated Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160763200766.html)
-   [Searching for Effective-Dated Changes to the Employee Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503337187.html)
-   [Viewing an Employee's Timeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156216462597.html)
-   [Creating an Employee Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899487.html)
-   [Working with Employee Social Security Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html)
-   [Printing Mailing Labels for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N916939.html)
-   [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
