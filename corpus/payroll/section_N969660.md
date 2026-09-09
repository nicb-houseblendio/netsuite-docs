---
id: "section_N969660"
type: "section"
title: "Getting Started with Payroll Solutions"
branch: "payroll"
category: "employee-management"
breadcrumb: "Employee Management > Payroll > Payroll Solutions > Paycheck Journal Feature > Getting Started with Payroll Solutions"
parent: "chapter_N969418"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N969660.html"
anchors: ["bridgehead_N969723", "bridgehead_N969771", "bridgehead_N969857"]
sha256: "67ce1015c42e8aaa18afdce8e228305941bfc57cd4bf540f858b0d9a74fc32ef"
---

You need to understand the following before you begin work on a payroll integration or payroll SuiteApp using the Paycheck Journal feature:

-   [Enabling the Paycheck Journal Feature](#bridgehead_N969723)
    
-   [Paycheck Journal Transaction](#bridgehead_N969771)
    
-   [Payroll Items and the Paycheck Journal Feature](#bridgehead_N969857)
    

## Enabling the Paycheck Journal Feature {#bridgehead_N969723}

Use the following procedure to enable the Paycheck Journal feature.

#### To enable the Paycheck Journal feature:

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Employees** subtab.
    
3.  In the Payroll section, check the **Paycheck Journal** box.
    
    The Paycheck Journal feature requires the Accounting feature, which is located on the **Accounting** subtab in the Basic Features section.
    
4.  Click **Save**.
    

With this feature enabled, the paycheck journal transaction and payroll item records are available to users with appropriate permissions.

## Paycheck Journal Transaction {#bridgehead_N969771}

The paycheck journal transaction works like the paycheck transaction in the Payroll feature, but it doesn't issue a check. Instead, it creates a journal entry to record the accounting impact. This transaction serves as a payroll interface for SOAP web services integrations with external payroll systems and for payroll SuiteApps built with SuiteScript.

The paycheck journal transaction is available at _Transactions > Employees > Paycheck Journal_. Users must have the Paycheck Journal permission, which is a Transactions type permission.

The following screenshot shows the fields supported by the paycheck journal transaction.

Note:

NetSuite customers are not expected to use this form without a partner payroll solution. Partner solutions are expected to include custom forms and custom fields that vary from this example.

![Screenshot of the paycheck journal page. Callouts one and two are on the page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/EmployeeManagement/Payroll/PaycheckJournalPageWithCallouts.png)

| 1 | Body fields |
| --- | --- |
| 2 | Sublist fields |

Paycheck journal body fields store basic values used by the transaction. Note the following:

-   Subsidiary is available only in NetSuite OneWorld.
    
-   Department, Class, and Location are available only in accounts that use these classifications.
    
-   Currency is available only in accounts with the Multiple Currencies feature enabled.
    
-   Exchange Rate is not currently in use. Its value, which is set to 1 when a currency is selected, should not be changed.
    
-   Partners can create custom transaction body fields that display on paycheck journal forms and are accessible to SOAP web services and SuiteScript.
    

Paycheck journal sublist fields store details about different types of payroll items that can be included in the transaction. Partners can create custom transaction line fields.

## Payroll Items and the Paycheck Journal Feature {#bridgehead_N969857}

Similar to transactions related to the Payroll feature, paycheck journal transactions use the payroll item record type to store line item values. The following table outlines some differences in how the two features handle payroll items.

| Payroll Feature | Paycheck Journal Feature |
| --- | --- |
| 
-   NetSuite provides predefined payroll items for deduction, earning, and employer contribution types.
-   You can create additional payroll items of these types.

 | 

-   No predefined payroll items.
-   You must create all deduction, earning, and employer contribution type payroll items.

 |
| 

-   NetSuite completely manages tax line items for payroll transactions.
-   You cannot create payroll items for taxes.

 | 

-   Payroll-related taxes must be implemented through payroll items that you create.
-   You can create two different types of payroll items for taxes: employee paid taxes and company (employer) paid taxes.

 |

Payroll items must be created before any paycheck journal transactions can be entered. The following item types are supported: Deduction, Earning:Addition, Earning:Commission, Earning:Expense, Earning:Salary, Earning:Sick, Earning:Vacation, Earning:Wage, Employer:Contribution, Employer:Expense, and Tax.

The Payroll Item page is available at _Lists > Accounting > Items_. Users must have the Payroll Items permission, which is a Lists type permission. The following screenshot shows the fields supported by the payroll item record.

![Screenshot of the payroll item page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/EmployeeManagement/Payroll/PaycheckJournalItem.png)

Note the following:

-   Subsidiary is available only in NetSuite OneWorld.
    
-   Item Type: Tax is available only for non-U.S. subsidiaries.
    
-   The Employee Paid box is available only when Item Type is set to Tax. When the Employee Paid box is clear, item type is Company Tax. When the Employee Paid box is checked, item type is Employee Tax.
    
-   Account fields vary according to item type, as shown in the following table:
    

| Item Type | Account Fields for Payroll Items |
| --- | --- |
| Deduction | Liability Account, Vendor (Agency) |
| Earning | Expense Account |
| Employer Contribution | Liability Account, Expense Account, Vendor (Agency) |
| Company Tax | Liability Account, Expense Account, Vendor (Agency) |
| Employee Tax | Liability Account, Vendor (Agency) |

### Related Topics

-   [SOAP Web Services and Paycheck Journal Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N972028.html)
-   [SuiteScript and the Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N972189.html)
-   [Custom Payroll Forms and Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N972394.html)
-   [Paycheck Journal Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N969418.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
