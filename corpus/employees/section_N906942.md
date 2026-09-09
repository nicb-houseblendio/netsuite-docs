---
id: "section_N906942"
type: "section"
title: "Custom Fields in Time Tracking Pages"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Custom Fields in Time Tracking Pages"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906942.html"
anchors: ["subsect_158799483256", "subsect_158799485181", "subsect_156987203994"]
sha256: "1b3d04020a3fce7ff3ff6f206673a0be57f2809b45f4ce0448b7abfb1b0daa9d"
---

You can create a custom field that appears on time tracking pages. This gives you additional flexibility in tracking information that's important to your business.

You can add a custom field to the column area on time tracking pages.

## Adding a Custom Column Field to Time Transactions {#subsect_158799483256}

#### To add a custom column field to time transactions:

1.  Go to _Customization > Lists, Records, & Fields > Transaction Line Fields > New_.
    
2.  In the **Label** field, enter a name or description for this field. The name appears as a column heading on transactions.
    
3.  If you use custom code, enter a unique ID for this custom field.
    
    NetSuite enables you to enter custom JavaScript files to perform functions specific to your business. If you don't enter an ID now, NetSuite automatically assigns one. You can't edit this ID after it's been created.
    
4.  Select the owner of this field. Only the owner can edit this record.
    
5.  Enter a description for your custom field.
    
    This description appears next to the field on time tracking pages.
    
6.  Select the type of custom field you want to add.
    
7.  If you entered a custom list and you want to attach it to your transaction custom field, select the appropriate list in the **List/Record** field.
    
8.  The **Store Value** box is checked by default. This means that information entered in this custom field is stored in your NetSuite account.
    
    Clear this box to indicate that the information stored in this custom field is for display only. The information is not stored in your account.
    
9.  On the **Applies To** subtab, check the **Time** box.
    
10.  On the **Validation & Defaulting** subtab, check the **Mandatory** box to make this a required field on the transactions you select.
     
11.  Enter a **Default Value** for this field.
     
12.  If you selected **List/Record** in the type field and you want to assign a default value, assign the appropriate selection in the **Default Selection** field.
     
13.  Check **Default Checked** if you want this box to default to a checked state on the transactions pages you select.
     
14.  On the **Sourcing & Filtering** subtab, if you have entered an item custom field and want to attach it to your transaction custom field, select it in the **Source** field.
     
15.  Click **Save**.
     

Your custom field automatically appears on the Time Tracking page. When tracking weekly time, your custom field appears in the columns of Weekly Time Tracking or Weekly Timesheet pages.

If your company doesn't use the Combine Time Items on Invoices preference and you bill the cost of a time transaction back to a customer, you can choose to include your custom field on all custom invoices except finance charge invoices.

Warning:

NetSuite CRM+ users can't record billable time or invoice customers for billable time.

## Including your Transaction Custom Field on a Custom Invoice {#subsect_158799485181}

#### To include your transaction custom field on a custom invoice:

1.  Go to _Customization > Forms > Transaction Forms_.
    
2.  In the **Edit** column, choose one of two options:
    
    -   Click **Customize** next to the appropriate form name to create a new custom form.
        
    -   Click **Edit** next to the appropriate form name to include your custom field on an existing custom form.
        
3.  When the Custom Form page appears, enter a name for your form so it's recognizable when selecting it on the Invoice page.
    
4.  Click the **Printing Fields** subtab.
    
5.  Click the **Columns** subtab.
    
6.  Locate the name of your transaction custom field in the **Description** column.
    
7.  Check the corresponding **Screen** and **Print/Email** boxes.
    
8.  Click **Save**.
    

The information you enter in your transaction custom field on the Time Tracking page now appears on the corresponding invoice you create.

If your company uses the Combine Time Items on Invoices preference, you can't include transaction custom fields on invoices because the information you enter in these fields may be different for each time record.

If your company uses Weekly Timesheets, you can also add custom body fields to the top of timesheets.

## Adding a Custom Body Field to Weekly Timesheets {#subsect_156987203994}

#### To add a custom body field to weekly timesheets:

1.  Go to _Customization > Lists, Records, & Fields > Other Record Fields > New_.
    
2.  In the **Record Type** field, select **Timesheet**.
    
3.  In the **Label** field, enter a name or description for this field.
    
4.  If you use custom code, enter a unique ID for this custom field.
    
    NetSuite enables you to enter custom JavaScript files to perform functions specific to your business. If you don't enter an ID now, NetSuite automatically assigns one. You can't edit the ID after it's been created.
    
5.  Select the owner of this field. Only the owner can edit this record.
    
6.  Enter a description for your custom field.
    
    This description appears next to the field on time tracking pages.
    
7.  Select the type of custom field you want to add.
    
8.  If you entered a custom list and you want to attach it to your custom field, select the appropriate list in the **List/Record** field.
    
9.  The **Store Value** box is checked by default. This means that information entered in this custom field is stored in your NetSuite account.
    
    Clear this box to indicate that the information stored in this custom field is for display only. The information is not stored in your account.
    
10.  On the **Validation & Defaulting** subtab, check the **Mandatory** box to make this a required field on the transactions you select.
     
11.  Enter a **Default Value** for this field.
     
12.  If you selected **List/Record** in the type field and you want to assign a default value, assign the appropriate selection in the **Default Selection** field.
     
13.  Check **Default Checked** if you want this box to default to a checked state on the transactions pages you select.
     
14.  On the **Sourcing & Filtering** subtab, if you have entered an item custom field and want to attach it to your transaction custom field, select it in the **Source** field.
     
15.  Click **Save**.
     

You new custom field automatically appears in the top portion of weekly timesheets.

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Giving an Employee Access to Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html)
-   [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html)
-   [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html)
-   [Deleting or Editing Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4502096285.html)
-   [Weekly Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html)
-   [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html)
-   [Using the Timer to Track Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905386.html)
-   [Calculating Total Time Worked](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905783.html)
-   [Entering Time for a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906077.html)
-   [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html)
-   [Custom Workflow-based Approvals for Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554190531.html)
-   [Updating Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156408321759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
