---
id: "section_N259878"
type: "section"
title: "Setting Up Transactions for NetSuite CRM+"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Setting Up Transactions for NetSuite CRM+"
parent: "chapter_N239909"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259878.html"
anchors: ["procedure_N259897", "bridgehead_N259942", "bridgehead_N260092", "bridgehead_N260104", "bridgehead_N260276", "bridgehead_N261188"]
sha256: "4bbe25cd83a77420bc17c7a1de0f90e78b9a30574cf501e0c7c62c3746a94743"
---

Important:

The information in this section pertains only to users of the NetSuite CRM+ product. Users of other NetSuite products can refer to [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html).

In NetSuite CRM+, users with the Administrator role can use the Set Up Transactions page to set preferences for processing their transactions.

#### To set up transactions: {#procedure_N259897}

1.  Go to Setup > Company > Set Up Transactions.
    
2.  On the Set Up Transactions page, select the preferences you want to set up.
    
    See the sections below for descriptions of these preferences.
    
    (Preferences that appear vary depending on the features you have enabled.)
    
3.  Click **Save**.
    

See the following for descriptions of each subtab on the Set Up Transactions page.

-   [General Subtab](#bridgehead_N259942)
    
-   [Reporting Subtab](#bridgehead_N260092)
    
-   [Ordering/Shipping Subtab](#bridgehead_N260104)
    
-   [Time & Expenses Subtab](#bridgehead_N260276)
    
-   [Tax Subtab](#bridgehead_N261188)
    

## General Subtab {#bridgehead_N259942}

-   **Consolidate Projects on Sales Transactions** - Check this box to consolidate projects on customer invoices. You can create invoices for one customer including multiple projects.
    
    You cannot issue invoices to a specific project. Instead,you issue the invoices to the customer.
    
-   **Maximum # of Quantity-based Price Levels** - Enter a limit for the most price levels allowed to be assigned to an item when using Quantity Pricing.
    
-   **Allow Discounts per Price Level on Quantity Pricing Schedules** - Check this box to enter different quantity discounts for each price level on quantity pricing schedules.
    
-   **Default Estimate Expiration (in days)** - Enter the default number of days before quotes expire.
    
-   **Duplicate Number Warnings** - Choose to have everyone with access to your account receive duplicate number warnings when transactions are submitted with the same numbers. This setting overrides the individual preference set at _Home > Set Preferences_.
    
    If you clear this box, individuals can receive duplicate number warnings by setting the preference at _Home > Set Preferences_.
    
-   **Make Departments Mandatory** - Check this box to make the Department field required on records and transactions.
    
-   **Make Classes Mandatory** - Check this box to make the Class field required on records and transactions.
    
-   **Make Locations Mandatory** - Check this box to make the Location field required on records and transactions.
    
-   **Allow Per-Line Departments** - Check this box to associate a department with individual line items on a transaction. When this box is checked, you can choose a different department for each line item on transactions.
    
    Clear this box to select a department in the header of a transaction. When this box is cleared, the department chosen in the header applies to all line items on the transaction.
    
-   **Allow Per-Line Classes** - Check this box to associate a class with individual line items on a transaction. When this box is checked, you can choose a different class for each line item on transactions.
    
    Clear this box to select a class in the header of a transaction. When this box is cleared, the class chosen in the header applies to all line items on the transaction.
    
-   **Allow Per-Line Locations** - Check this box to associate a location with individual line items on a transaction. When this box is checked, you can choose a different location for each line item on transactions.
    
    Clear this box to select a location in the header of a transaction. When this box is cleared, the location chosen in the header applies to all line items on the transaction.
    

## Reporting Subtab {#bridgehead_N260092}

Check the Include Shipping Costs in Sales and Forecast Reports to have shipping and handling costs includes in order totals for sales and forecasting reports.

## Ordering/Shipping Subtab {#bridgehead_N260104}

-   **Default Shipping Method**: Select the shipping method you want to appear automatically on bills and invoices.
    
    You can choose other shipping methods when you enter transactions.
    
    To add choices to this list, go to Lists > New Shipping Items.
    
-   **Default Sales Order Status**: Choose your default status for sales orders:
    
    -   Choose **Pending Approval** if your company uses the approval process for sales orders.
        
    -   Choose **Pending Fulfillment** if your company does not use the approval process for sales orders.
        
        You can change the sales order status when you enter a transaction.
        
-   **Require Re-approval on Edit of Sales Order**: Choose to require re-approval when someone edits a sales order that was previously approved.
    
    Partially fulfilled sales orders are not affected by this preference. After a sales order is partially fulfilled, the status cannot be changed back to pending approval.
    
-   **Send E-mail Confirmation when Sales Order Cancelled**: Check this box if you want an email messsage sent to the customer when a sales order is canceled.
    
-   **Default Return Auth. Status**: Select **Pending Approval** if your company uses the approval process for return authorizations.
    
    Select **Pending Fulfillment** if your company does not use the approval process for return authorizations.
    
    You can change the return authorization status when you enter a transaction.
    
-   **Charge for Shipping**: Check this box to charge shipping by weight, by percent of total order, or by a flat rate.
    
    After you check this box, go to Lists > Shipping Items > New to create shipping items.
    
    After you create shipping items, you can select them on product invoices. Your customers can also select shipping items when making a purchase from your Web store.
    
-   **Charge Handling Separate from Shipping**: Check this box to charge a separate handling charge in addition to shipping charges.
    
-   **Default Item Weight in Lbs.**: Enter a default shipping weight for items without a weight set on their item records.
    
    Note:
    
    If you don't enter a weight here, NetSuite uses 1 pound as the default weight. Item weight is used to determine shipping costs if you charge shipping per item or use UPS real-time rates.
    

## Time & Expenses Subtab {#bridgehead_N260276}

-   **Override Rates on Time Records**: Check this box if you want the option to lock the billable rate you enter on time records. You would do this so the billable rate isn't affected by any rate changes that may happen before this customer is invoiced.
    
    If you check this box, you can use different price levels by going to Setup > Enable Features > Customers/Sales, and checking the Use Multiple Prices box.
    
    Clear this box if you have the rate field in time tracking and you do not want employees to see the service item rates. Then, the rate is kept in the system, but will no longer show in time tracking.
    
-   **Combine Detail Items on Expense Report Transactions**: This preference affects detail items on expense reports.
    
    Check this box if you want to combine line items from the same category on a single expense report submitted by an employee.
    
    For example, if an employee enters a single expense report that contains two entries for entertainment costs, the total shows as one line item for entertainment costs on the invoice.
    
    Clear this box to detail each expense report line item individually.
    
    This preference does not combine expense categories from multiple expense reports submitted by the same employee.
    
-   **Require Approvals on Time Records**: Check this box to require supervisors to approve their employees' time transactions.
    
    If you don't check this box, time transactions can be billed to customers or included in the payroll run without the approval of a supervisor.
    
-   **Automatically Notify Supervisor**: Check this box to send supervisors email messages when they need to approve expense reports and purchase requests.
    
    If you check this box, you must also check either Use Expense Reports, Enable Purchase Requests or both at Setup > Enable Features.
    

## Tax Subtab {#bridgehead_N261188}

-   **Tax Code Lists Include**: Choose what you want to appear in the Tax field on sales transactions:
    
    -   **Tax Groups Only**
        
    -   **Tax Groups and Tax Items**
        
    -   **Tax Items Only**
        
    
    You can create Tax Groups at Lists > Accounting > Tax Groups > New. You can create tax items at Lists > Accounting > Tax Items > New.
    
    The Tax Code Lists Include preference does not apply to journals.
    

### Related Topics

-   [NetSuite Company Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N239909.html)
-   [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html)
-   [Set Company Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N242860.html)
-   [Change Record and Transaction Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252023.html)
-   [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html)
-   [Setting Up States, Provinces, and Counties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253697.html)
-   [Supported Countries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253846.html)
-   [Setting Printing and Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N253916.html)
-   [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html)
-   [Setting Up Duplicate Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html)
-   [NetSuite Account Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1487792254.html)
-   [Antivirus Scanning on File Cabinet Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4822646785.html)
-   [Activating System Alert Reminders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258424.html)
-   [Searching Bulk Processing Jobs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495464846.html)
-   [Administrative Notification Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258657.html)
-   [Managing Plug-ins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4659859610.html)
-   [NetSuite Service Tiers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1539959231.html)
-   [SuiteCloud Plus Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N259503.html)
-   [The Setup Page for NetSuite CRM+ Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261260.html)
-   [Using Telephony Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N511129.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
