---
id: "section_N295396"
type: "section"
title: "Standard Roles Permissions Table"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > Standard Roles Permissions Table"
parent: "chapter_N284861"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html"
anchors: ["subsect_0415060145", "subsect_0415060302", "subsect_0425060406", "subsect_0425060641", "subsect_0425061124", "subsect_0425061156", "subsect_0425061225", "subsect_0425061252", "subsect_0425061326", "subsect_0425061352", "subsect_0425061438", "subsect_0425061504", "subsect_0425061528", "subsect_0425061553", "subsect_0425061617", "subsect_78193907376", "subsect_0425061645", "subsect_0425061707", "subsect_0425061940", "subsect_0425062018", "subsect_0425062044", "subsect_0425062104", "subsect_0425062129", "subsect_0425062152", "subsect_0425062219", "subsect_0425062243", "subsect_0425062306", "subsect_0425062331", "subsect_0425062353", "subsect_0425062416", "subsect_0425062438", "subsect_0425062508", "subsect_0425062536", "subsect_0425062632", "subsect_0425062709", "subsect_0425062734", "subsect_0425062759", "subsect_0425062826", "subsect_0425062854", "subsect_0425062918", "subsect_0708012605", "subsect_0302012022", "subsect_0709095451", "subsect_0731010940", "subsect_0709101525", "subsect_0425063323", "subsect_0425062942", "subsect_0425063008", "subsect_0425063031", "subsect_0425063056", "subsect_0425063121", "subsect_0425063146", "subsect_0425063211", "subsect_0425063246"]
sha256: "7b6afb4950035225181a565232d9b45b5360d832ba9e15234815fc2dbb2a7d90"
---

The following table lists the permissions and permission levels for each standard role.

It's best to start with a copy of the standard roles built into NetSuite before you customize them. Giving users only the access they need helps avoid showing restricted pages, records, and data. You can then add or remove permissions from the roles as needed. See [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html) for an updated list of permissions and their corresponding usage.

The standard roles available in your account may differ, depending on the modules you've purchased, and the features you've enabled. You can see the roles available in your account at _Setup > Users/Roles > Manage Roles_, and you can review a role's details by clicking its link on the Manage Roles page.

You can't modify standard roles. You should create a custom version of any standard role before assigning it, so you can change it later if needed, even after it has been assigned.

The Administrator role has **all** permissions available in your NetSuite account at **all** levels. To see the full list of permissions assigned to the Administrator role, go to _Setup > Users/Roles > Manage Roles_, click **Administrator** and see the list of permissions on the Permissions subtab. For more information about the Administrator role, see [NetSuite Account Administration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4570420905.html).

The Data Warehouse Integrator role allows Connect users to have access to all NetSuite data through the NetSuite2.com data source, except for sensitive data. For more information, see [Role and Permission Considerations for NetSuite2.com](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162885566786.html).

Important:

If you have the Advanced Employee Permissions feature enabled, see [Advanced Employee Permissions and Standard NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1495116029.html) for a list of the employee permissions that are assigned to standard NetSuite roles when this feature is enabled.

There are three main groups of standard roles in NetSuite: executive, managerial, and operational.

-   Executive roles include top-level and senior roles that let them see everything happening in their areas.
    
-   Managerial roles, in general, have fewer permissions than executive and operational roles, but they include the key permissions needed to manage their areas.
    
-   Operational roles let users support their customers or colleagues.
    

| Executive | Managerial | Operational |
| --- | --- | --- |
| [CEO](#subsect_0425061252) | [Engineering Manager](#subsect_0425061707) | [A/P Clerk](#subsect_0415060145) |
| [CEO (Hands Off)](#subsect_0425061326) | [Intranet Manager](#subsect_0425062018) | [A/R Clerk](#subsect_0415060302) |
| [CFO](#subsect_0425061352) | [Marketing Manager](#subsect_0425062152) | [Accountant](#subsect_0425060406) |
| [Chief People Officer (CPO)](#subsect_0425061438) | [Payroll Manager](#subsect_0425062243) | [Accountant (Reviewer)](#subsect_0425060641) |
| [Sales Vice President](#subsect_0425062918) | [PM Manager](#subsect_0425062331) | [Bookkeeper](#subsect_0425061156) |
|  | [Product Manager](#subsect_0425062353) | [Buyer](#subsect_0425061225) |
|  | [QA Manager](#subsect_0425062438) | [Consultant](#subsect_0425061504) |
|  | [Resource Manager](#subsect_0425062508) | [Customer Center](#subsect_0425061528) |
|  | [Revenue Manager](#subsect_0425062734) | [Developer](#subsect_0425061553) |
|  | [Sales Manager](#subsect_0425062826) | [Employee Center](#subsect_0425061617) |
|  | [Store Manager](#subsect_0425062942) | [Engineer](#subsect_0425061645) |
|  | [Support Manager](#subsect_0425063031) | [Human Resources Generalist](#subsect_0425061940) |
|  | [Warehouse Manager](#subsect_0425063246) | [Issue Administrator](#subsect_0425062044) |
|  |  | [Marketing Administrator](#subsect_0425062104) |
|  |  | [Marketing Assistant](#subsect_0425062129) |
|  |  | [Partner Center](#subsect_0425062219) |
|  |  | [Payroll Setup](#subsect_0425062306) |
|  |  | [QA Engineer](#subsect_0425062416) |
|  |  | [Retail Clerk](#subsect_0425062536) |
|  |  | [Retail Clerk (Web Services Only)](#subsect_0425062632) |
|  |  | [Revenue Accountant](#subsect_0425062709) |
|  |  | [Sales Administrator](#subsect_0425062759) |
|  |  | [Sales Person](#subsect_0425062854) |
|  |  | [Support Administrator](#subsect_0425063008) |
|  |  | [Support Person](#subsect_0425063056) |
|  |  | [System Administrator](#subsect_0425063121) |
|  |  | [Specialized User: CRM](#subsect_0708012605) |
|  |  | [Specialized User: Manufacturing Operator](#subsect_0302012022) |
|  |  | [Specialized User: Project Manager](#subsect_0709095451) |
|  |  | [Specialized User: Site Operator](#subsect_0731010940) |
|  |  | [Specialized User: View and Approve](#subsect_0709101525) |
|  |  | [Specialized User: WMS](#subsect_0425063323) |
|  |  | [Tax Engine](#subsect_0425063146) |
|  |  | [Vendor Center](#subsect_0425063211) |

## A/P Clerk {#subsect_0415060145}

| A/P Clerk |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Accounts Payable

Accounts Payable Graphing

Amortization Schedules

Bill Of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Custom Recognition Event Type

Deferred Expense Reports

Employee Public

Employee Record

Entity-Subsidiary relationship

Expense Amortization Plan

Expense Amortization Rule

Financial History

Inventory

Non Posting Registers

Notes Tab

Pricing Records

Purchase Order Reports

SaaS Metric

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

System Journal

Tax Records

Tax Reports



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Accounting Lists

Accounts Payable Register

Bill Purchase Orders

Bill of Materials

Bills

Classes

Credit Returns

Departments

Email Template

Enter Vendor Credits

Item Receipt

Items

Locations

Memorized Transactions

Other Lists



 | 

Pay Bills

Pay Sales Tax

Purchase Order

Receive Order

Requisition

Statistical Account Registers

SuiteAnalytics Workbook

Tax Details Tab

Tax Liability Payment

Time-Off

Track Messages

Units

Vendor Prepayment

Vendor Prepayment Application

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors



 | 

Address List in Search

Analytical Impact

Automated Clearing House

Calendar

Contacts

Deleted Records

Documents and Files

Events

Find Transaction

General Token

Inbound Shipment

Log in using Access Tokens

Mobile Device Access

Notifications

Ownership Transfer

Payment Card

Payment Card Token

Payment Instruments

Perform Search

Phone Calls

Posting Period on Transactions

Price Books

Price Plans

Product Analytics Records

Report Customization

Report Scheduling

REST Web Services

Scanned Vendor Bills

SOAP Web Services

Subscription Plan

Tasks

Template Categories

Usage

Vendor Automated Clearing House

Vendor Bill Approval

Vendor Payment Approval

Vendor Prepayment Approval

Vendor Payment Instruments



 |

## A/R Clerk {#subsect_0415060302}

| A/R Clerk |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Receivable

Accounts Receivable Graphing

Bill Of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Custom Recognition Event Type

Employee Public

Employee Record

Entity-Subsidiary relationship

Fair Value Dimension

Fair Value Formula

Fair Value Price

Financial History

Generate Price Lists

Generate Statements

Installment Payment Links

Inventory

Item Revenue Category

Lead Snapshot/Reminders

Notes Tab

Pricing Records

Project Profitability

Project Revenue Rules

Project Templates

Recognition Treatment

Recognition Treatment Rule

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Element

Revenue Management VSOE

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Rule

Revenue Recognition Schedules

SaaS Metric

System Journal

Tax Records

Tax Reports

Time Tracking

Transaction Detail

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Export Lists

Kudos

Recognize Gift Certificate Income

Resource

Tableau® Workbook Export



 | 

Accounting Lists

Accounts Receivable Register

Bill of Materials

Cash Sale

Charge

Charge Rule

Classes

Competitors

Customer Deposit

Customer Payment

Customer Payment Authorization

Customers

Departments

Deposit Application

Email Template

Fulfill Orders

Gift Certificate

Invoice

Invoice Sales Orders

Item Fulfillment

Items

Locations

Memorized Transactions

Other Lists

Override Payment Hold

Print Shipment Documents

Projects

Sales Order

Shipping Partner Package

Shipping Partner Shipment

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook

Tax Details Tab

Time-Off

Track Messages

Transfer Order

Unbilled Receivable Registers

Units



 | 

Address List in Search

Analytical Impact

Automated Clearing House

Calendar

Charge - Run Rules

Contacts

Deleted Records

Documents and Files

Events

Find Transaction

General Token

Invoice Approval

Log in using Access Tokens

Mobile Device Access

Notifications

Payment Card

Payment Card Token

Payment Instruments

Perform Search

Phone Calls

Posting Period on Transactions

Price Books

Price Plans

Product Analytics Records

Project Tasks

Report Customization

Report Scheduling

REST Web Services

SOAP Web Services

Subscription Plan

Tasks

Template Categories

Track Time

Usage



 |

## Accountant {#subsect_0425060406}

| Accountant |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Account Detail

Accounts Payable

Accounts Payable Graphing

Accounts Receivable

Accounts Receivable Graphing

Amortization Reports

Balance Sheet

Bill Of Materials Inquiry

Bulk Processing Submissions

Check Item Availability

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Deferred Expense Reports

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Expenses

Fair Value Dimension

Fair Value Formula

Fair Value Price

Financial Statements

General Ledger

Generate Price Lists

Generate Statements

Income

Income Statement

Inventory

Installment Payment Links

Item Revenue Category

Lead Snapshot/Reminders

Net Worth

Notes Tab

Period End Financial Statements

Pricing Records

Project Budget

Project Profitability

Project Revenue Rules

Project Templates

Purchase Order Reports

Purchases

Recognition Treatment

Recognition Treatment Rule

Revenue Arrangement

Revenue Arrangement Approval

Revenue Element

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Rule

Revenue Recognition Reports

Saas Metric

Sales

Sales By Partner

Sales By Promotion

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Subsidiary Settings Manager

System Journal

Tax

Time Tracking

Transaction Detail

Trial Balance

View Gateway Asynchronous Notifications

View Payment Events

Work Breakdown Structure

Work Calendar



 | 

Balance Transactions by Segments

Balancing Journals

Export Lists

Kudos

Recognize Gift Certificate Income

Resource

Tableau® Workbook Export



 | 

Accounting Lists

Accounting Management

Accounts

Accounts Payable Register

Accounts Receivable Register

Adjust Inventory

Amortization Schedules

Bank Account Registers

Bill of Materials

Bill Purchase Orders

Bills

Build Assemblies

Build Work Orders

Cash Sale

Charge

Charge Rule

Check

Classes

Close Work Orders

Competitors

Create Allocation Schedules

Credit Card Charge

Credit Card Refund

Credit Card Registers

Credit Memo

Credit Returns

CRM Groups

Currency Revaluation

Custom Recognition Event Type

Customer Deposit

Customer Payment

Customer Payment Authorization

Customers

Departments

Deposit

Deposit Application

Distribute Inventory

Email Template

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Equity Registers

Expense Amortization Plan

Expense Amortization Rule



 | 

Fixed Asset Registers

Generate Revenue Commitment

Generate Revenue Commitment Reversals

Gift Certificate

Invoice

Invoice Sales Orders

Issue Components

Items

Locations

Long Term Liability Registers

Make Journal Entry

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Mass Updates

Memorized Transactions

Non Posting Registers

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Other Lists

Other Names

Pay Bills

Pay Sales Tax

Period End Journals

Post Time

Projects

Purchase Order

Reconcile

Reconcile Reporting

Requisition

Revenue Commitment

Revenue Commitment Reversal

Revenue Management VSOE

Revenue Recognition Schedules

Sales Order

Statistical Account Registers

Subscription Change Orders

Subscriptions

SuiteAnalytics Workbook

Tax Details Tab

Tax Liability Payment

Tax Records

Tax Reports

Time-Off

Track Messages

Track Time

Transfer Funds

Transfer Inventory

Unbilled Receivable Registers

Unbuild Assemblies

Units

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

Work Order

Work Order Close

Work Order Completion

Work Order Issue



 | 

Address List in Search

Allocate Orders

Approve Order Reservation

Analytical Impact

Automated Cash Application

Bills

Bill Of Distribution

Blanket Purchase Order

Calendar

Contacts

Count Inventory

Create Inventory Counts

Deleted Records

Distribution Network

Documents and Files

Earliest Availability

Employee Record

Events

Exception Management

Find Transaction

Global Inventory Relationship

Charge - Run Rules

Inventory Cost Template

Invoice Approval

Item Demand Plan

Item Revisions

Item Supply Plan

Log in using Access Tokens

Manufacturing Cost Template

Manufacturing Routing

Material Requirements Planning

Mobile Device Access

Notifications

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Pay Tax Liability

Perform Search

Phone Calls

Planned Standard Cost

Post Vendor Bill Variances

Posting Period on Transactions

Price Books

Price Plans

Product Analytics Records

Project Tasks

Purchase Contract

Reallocate Order Item

Report Customization

Report Scheduling

REST Web Services

Request For Quote

Revalue Inventory Cost

Sales Channel

SOAP Web Services

Standard Cost Version

Subscription Plan

Tasks

Tegata Accounts

Tegata Payable

Tegata Receivables

Template Categories

Transfer Order

Transfer Order Approval

Usage

Vendor Bill Approval

Vendor Payment Approval

Vendor Request For Quote



 |

## Accountant (Reviewer) {#subsect_0425060641}

| Accountant (Reviewer) |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounting Lists

Accounting Management

Accounts

Accounts Payable

Accounts Payable Graphing

Accounts Payable Register

Accounts Receivable

Accounts Receivable Graphing

Accounts Receivable Register

Adjust Inventory

Amortization Reports

Amortization Schedules

Balance Sheet

Balance Transactions by Segments

Balancing Journals

Bank Account Registers

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Build Assemblies

Build Work Orders

Cash Sale

Charge

Charge Rule

Check

Check Item Availability

Classes

Close Work Orders

Commit Orders

Competitors

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Create Allocation Schedules

Credit Card Charge

Credit Card Refund

Credit Card Registers

Credit Memo

Credit Returns

CRM Groups

Currency Revaluation

Custom Recognition Event Type

Customer Deposit

Customer Payment

Customer Payment Authorization

Customers

Deferred Expense Reports

Departments

Deposit

Deposit Application

Distribute Inventory

Employee Public

Employee Reminders

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Entity-Subsidiary relationship

Equity Registers

Expense Amortization Plan

Expense Amortization Rule

Expenses

Fair Value Dimension

Fair Value Formula

Fair Value Price

Financial Statements

Fixed Asset Registers

General Ledger

Generate Price Lists

Generate Statements

Gift Certificate

Income



 | 

Income Statement

Inventory

Invoice

Installment Payment Links

Issue Components

Item Revenue Category

Items

Lead Snapshot/Reminders

Locations

Long Term Liability Registers

Make Journal Entry

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Memorized Transactions

Net Worth

Non Posting Registers

Notes Tab

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Other Lists

Other Names

Pay Sales Tax

Period End Financial Statements

Period End Journals

Price Books

Price Plans

Pricing Records

Project Budget

Project Profitability

Project Revenue Rules

Projects

Purchase Contract

Purchase Order

Purchases

Recognition Treatment

Recognition Treatment Rule

Reconcile Reporting

Request For Quote

Requisition

Revalue Inventory Cost

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Element

Revenue Management VSOE

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Order

Sales Order Reports

Sales Order Transaction Report

Statistical Account Registers

Subscription Plan

Subscription Change Orders

Subscriptions

System Journal

Tax

Tax Details Tab

Tax Liability Payment

Tax Records

Tax Reports

Time Tracking

Track Time

Transaction Detail

Transfer Funds

Transfer Inventory

Transfer Order

Trial Balance

Unbilled Receivable Registers

Unbuild Assemblies

Units

Usage

Vendor Request For Quote

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

View Gateway Asynchronous Notifications

View Payment Events

View Breakdown Structure

Work Calendar

Work Order

Work Order Close

Work Order Completion

Work Order Issue



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Bills

Email Template

Mass Updates

Override Payment Hold

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Allocate Orders

Analytical Impact

Approve Order Reservation

Bill Of Distribution

Blanket Purchase Order

Calendar

Charge - Run Rules

Contacts

Count Inventory

Create Inventory Counts

Deleted Records

Distribution Network

Documents and Files

Employee Record

Events

Find Transaction

Global Inventory Relationship

Inventory Cost Template

Item Demand Plan

Item Revisions

Item Supply Plan

Log in using Access Tokens

Manufacturing Cost Template

Manufacturing Routing

Material Requirements Planning

Mobile Device Access

Notifications

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Perform Search

Phone Calls

Planned Standard Cost

Posting Period on Transactions

Product Analytics Records

Project Tasks

Reallocate Order Item

Report Customization

Report Scheduling

REST Web Services

Sales Channel

SOAP Web Services

Standard Cost Version

Subsidiary - Tax Engine selection

Tasks

Tegata Accounts

Tegata Payable

Tegata Receivables

Template Categories

Vendor Bill Approval

Vendor Payment Approval



 |

## Advanced Partner Center {#subsect_0425061124}

| Advanced Partner Center |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Bill Of Materials Inquiry

Bill of Materials

Credit Memo

Customer Refund

Customer Payment

Email Template

Financial History

Installment Payment Links

Invoice

Items

Knowledge Base

Lead Snapshot/Reminders

Marketing Campaigns

Non Posting Registers

Partner Commission Reports

Project Templates

Return Authorization

Sales

Sales By Partner

Sales Force Automation

Sales Order Reports

Sales Order Transaction Report

Subscriptions

Subscription Plan

Subsidiaries

Support

Support Case Snapshot/Reminders

Tax Details Tab

Tax Records

Units

Work Calendar



 | 

Export Lists

Kudos

Notes Tab

Promotion

Tableau® Workbook Export



 | 

Campaign History

Cases

CRM Groups

Cases

Estimate

Gift Certificate

Opportunity

Sales Order

SuiteAnalytics Workbook

Track Messages



 | 

Calendar

Contacts

Custom Record Entries

Customers

Events

Find Transaction

Log in using Access Tokens

Mobile Device Access

Notifications

Partners

Perform Search

Price Books

Price Plans

Phone Calls

Project Tasks

Report Customization

Report Scheduling

REST Web Services

SOAP Web Services

Tasks

Template Categories

Usage



 |

## Bookkeeper {#subsect_0425061156}

| Bookkeeper |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounting Management

Accounts

Accounts Payable

Accounts Payable Register

Accounts Receivable

Accounts Receivable Register

Bank Account Registers

Bill Of Materials Inquiry

Bulk Processing Submissions

Check Item Availability

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Credit Card Registers

Deferred Expense Reports

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Equity Registers

Fixed Asset Registers

Generate Price Lists

Generate Statements

Installment Payment Links

Inventory

Lead Snapshot/Reminders

Long Term Liability Registers

Non Posting Registers

Notes Tab

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Pricing Records

Project Profitability

Project Templates

Purchase Order Reports

Revalue Inventory Cost

SaaS Metric

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Statistical Account Registers

System Journal

Tax

Tax Records

Tax Reports

Time Tracking

Transaction Detail

Unbilled Receivable Registers

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Export Lists

Kudos

Recognize Gift Certificate Income

Resource

Tableau® Workbook Export



 | 

Accounting Lists

Address List in Search

Adjust Inventory

Bill Purchase Orders

Bill of Materials

Bills

Cash Sale

Charge

Charge Rule

Check

Classes

Competitors

Credit Card Charge

Credit Card Refund

Credit Memo

Credit Returns

CRM Groups

Currency Revaluation

Customer Deposit

Customer Payment

Customer Payment Authorization

Customers

Departments

Deposit

Deposit Application

Email Template

Employees

Enter Opening Balances

Enter Vendor Credits

Gift Certificate

Invoice

Invoice Sales Orders

Item Revisions

Items

Locations

Make Journal Entry

Memorized Transactions

Other Lists

Other Names

Pay Bills

Pay Sales Tax

Projects

Purchase Order

Reconcile

Reconcile Reporting

Requisition

Sales Order

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook

Tax Details Tab

Tax Liability Payment

Time-Off

Track Messages

Transfer Funds

Transfer Order

Units

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors



 | 

Allocate Orders

Analytical Impact

Approve Order Reservation

Automated Cash Application

Bill Of Distribution

Calendar

Charge - Run Rules

Contacts

Count Inventory

Create Inventory Counts

Deleted Records

Distribution Network

Documents and Files

Earliest Availability

Employee Record

Events

Find Transaction

Global Inventory Relationship

Inventory Cost Template

Invoice Approval

Item Demand Plan

Item Supply Plan

Log in using Access Tokens

Manufacturing Cost Template

Manufacturing Routing

Material Requirements Planning

Mobile Device Access

Notifications

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Perform Search

Phone Calls

Planned Standard Cost

Price Books

Price Plans

Product Analytics Records

Post Vendor Bill Variances

Posting Period on Transactions

Project Tasks

Reallocate Order Item

Report Customization

Report Scheduling

REST Web Services

Sales Channel

SOAP Web Services

Standard Cost Version

Subscription Plan

Tasks

Tegata Accounts

Tegata Payable

Tegata Receivables

Template Categories

Track Time

Usage

Vendor Bill Approval

Vendor Payment Approval



 |

## Buyer {#subsect_0425061225}

| Buyer |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Accounts Payable

Accounts Payable Graphing

Amortization Schedules

Bill Of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Custom Recognition Event Type

Employee Public

Employee Record

Entity-Subsidiary relationship

Expense Amortization Plan

Expense Amortization Rule

Financial History

Inventory

Non Posting Registers

Notes Tab

Pricing Records

Purchase Order Reports

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Accounting Lists

Accounts Payable Register

Bill Purchase Orders

Bill of Materials

Bills

Classes

Departments

Email Template

Item Receipt

Items

Locations

Memorized Transactions

Other Lists

Receive Order

Requisition

Statistical Account Registers

SuiteAnalytics Workbook

Time-Off

Track Messages

Units

Vendor Returns

Vendors



 | 

Address List in Search

Blanket Purchase Order

Blanket Purchase Order Approval

Calendar

Contacts

Deleted Records

Documents and Files

Employee Record

Events

Find Transaction

Inbound Shipment

Log in using Access Tokens

Mobile Device Access

Notifications

Ownership Transfer

Perform Search

Phone Calls

Product Analytics Records

Purchase Contract

Purchase Contract Approval

Purchase Order

Report Customization

Report Scheduling

Request For Quote

Requisition Approval

REST Web Services

SOAP Web Services

Tasks

Template Categories

Vendor Return Auth. Approval

Vendor Return Authorization



 |

## CEO {#subsect_0425061252}

| CEO |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Payable

Accounts Payable Graphing

Accounts Receivable

Accounts Receivable Graphing

Amortization Reports

Amortization Schedules

Balance Sheet

Bill Of Materials Inquiry

Bulk Processing Submissions

Check Item Availability

Commission Reports

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Create Allocation Schedules

Custom Recognition Event Type

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Expense Amortization Plan

Expense Amortization Rule

Expenses

Fair Value Dimension

Fair Value Formula

Fair Value Price

Financial History

Financial Statements

General Ledger

Generate Price Lists

Generate Statements

Imported Employee Expenses

Income

Income Statement

Individual Paycheck

Installment Payment Links

Inventory

Item Revenue Category

Lead Snapshot/Reminders

Net Worth

Notes Tab

Partner Authorized Commission Reports

Partner Commission Reports

Pricing Records

Project Budget

Project Profitability

Project Revenue Rules

Project Templates

Purchase Order Reports

Purchases

Quota Reports

Recognition Treatment

Recognition Treatment Rule

Resource Allocations

Return Authorization Reports

Revalue Inventory Cost

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Element

Revenue Management VSOE

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

System Journal

Tax

Tax Details Tab

Tax Records

Tax Reports

Time Tracking

Trial Balance

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Web Store Report

Work Breakdown Structure

Work Calendar



 | 

Export Lists

Kudos

Recognize Gift Certificate Income

Tableau® Workbook Export



 | 

Email Template

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

Mass Updates

PDF Messages

PDF Template

Reconcile

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Accounting Lists

Accounting Management

Accounts

Accounts Payable Register

Accounts Receivable Register

Address List in Search

Adjust Inventory

ADP Import Data

Allocate Orders

Analytical Impact

Approve Order Reservation

Audit Trail

Automated Cash Application

Automated Clearing House

Bank Account Registers

Bill Of Distribution

Bill Purchase Orders

Bill of Materials

Bills

Blanket Purchase Order

Blanket Purchase Order Approval

Build Work Orders

Calculate Time

Calendar

Cash Sale

Cash Sale Refund

Check

Classes

Close Work Orders

Competitors

Contacts

Count Inventory

Create Inventory Counts

Credit Card Charge

Credit Card Refund

Credit Card Registers

Credit Memo

Credit Returns

CRM Groups

Currency Revaluation

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Customers

Deleted Records

Departments

Deposit

Deposit Application

Distribution Network

Documents and Files

Earliest Availability



 | 

Edit Forecast

Employee Commission Transaction

Employee Commission Transaction Approval

Employee Record

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Enter Year-To-Date Payroll Adjustments

Equity Registers

Events

Expense Report

Finance Charge

Find Transaction

Fixed Asset Registers

Fulfill Orders

General Token

Gift Certificate

Global Inventory Relationship

Import Online Banking File

Inbound Shipment

Internal Publisher

Inventory Cost Template

Invoice

Invoice Approval

Invoice Sales Orders

Issue Components

Item Fulfillment

Item Receipt

Item Revisions

Item/Category Layouts

Items

Locations

Log in using Access Tokens

Long Term Liability Registers

Mail Merge

Make Journal Entry

Manufacturing Cost Template

Manufacturing Routing

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Matching Rules for Online Banking

Memorized Transactions

Mobile Device Access

Non Posting Registers

Notifications

Opportunity

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Other Lists

Other Names

Outlook Integration 2.0

Ownership Transfer



 | 

Pay Bills

Pay Sales Tax

Payment Card

Payment Card Token

Payment Instruments

Payroll Liability Payments

Perform Search

Phone Calls

Planned Standard Cost

Post Vendor Bill Variances

Posting Period on Transactions

Presentation Categories

Price Books

Price Plans

Print Shipment Documents

Process GST Refund

Product Analytics Records

Project Tasks

Projects

Publish Forms

Purchase Contract

Purchase Contract Approval

Purchase Order

Quote

Reallocate Order Item

Receive Order

Receive Returns

Reconcile Reporting

Refund Returns

Report Customization

Report Scheduling

Request For Quote

Requisition

Requisition Approval

Resource

Resource Allocation Approval

REST Web Services

Return Auth. Approval

Return Authorization

Sales Channel

Sales Order

Sales Order Approval

Scanned Vendor Bills

Set Up Budgets

Shipping Partner Package

Shipping Partner Shipment

SOAP Web Services

Standard Cost Version

Statement Charge

Statistical Account Registers

Store Account Registers

Store Categories

Store Content Categories

Store Content Items

Store Tabs

Subscription Change Orders

Subscription Plan

Subscriptions

Tasks

Tegata Accounts

Tegata Payable

Tegata Receivables

Template Categories

Timer

Track Time

Transfer Funds

Transfer Order

Transfer Order Approval

Unbilled Receivable Registers

Units

Usage

Vendor Bill Approval

Vendor Payment Approval

Vendor Request For Quote

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

Work Order

Work Order Close

Work Order Completion

Work Order Issue



 |

## CEO (Hands Off) {#subsect_0425061326}

| CEO (Hands Off) |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounting Lists

Accounting Management

Accounts

Accounts Payable

Accounts Payable Graphing

Accounts Payable Register

Accounts Receivable

Accounts Receivable Graphing

Accounts Receivable Register

Adjust Inventory

ADP Import Data

Amortization Reports

Audit Trail

Balance Sheet

Bank Account Registers

Bill of Materials

Bill Of Materials Inquiry

Bill Purchase Orders

Build Work Orders

Calculate Time

Cash Sale

Cash Sale Refund

Check

Classes

Close Work Orders

Commission Reports

Competitors

Contact-Subsidiary relationship

Credit Card Charge

Credit Card Refund

Credit Card Registers



 | 

Bulk Processing Submissions

Credit Memo

Credit Returns

Currency Revaluation

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Customers

Departments

Deposit

Deposit Application

Edit Forecast

Employee Commission Transaction Approval

Employee Public

Employee Reminders

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Enter Year-To-Date Payroll Adjustments

Entity-Subsidiary relationship

Equity Registers

Expense Report

Expenses

Finance Charge

Financial History

Financial Statements

Fixed Asset Registers

Fulfill Orders

General Ledger

Generate Price Lists

Generate Statements

Gift Certificate

Imported Employee Expenses

Import Online Banking File

Income

Income Statement

Individual Paycheck

Installment Payment Links



 | 

Inventory

Invoice

Invoice Sales Orders

Issue Components

Item Fulfillment

Item Receipt

Items

Lead Snapshot/Reminders

Locations

Long Term Liability Registers

Make Journal Entry

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Memorized Transactions

Net Worth

Non Posting Registers

Notes Tab

Opportunity

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Other Lists

Other Names

Partner Authorized Commission Reports

Partner Commission Reports

Pay Bills

Pay Sales Tax

Payroll Liability Payments

Posting Period on Transactions

Price Books

Price Plans

Pricing Records

Print Shipment Documents

Print Shipping Documents

Process GST Refund

Projects

Project Profitability

Purchase Contract

Purchase Order

Purchase Order Reports

Purchases

Quota Reports

Quote



 | 

Receive Order

Receive Returns

Reconcile Reporting

Refund Returns

Request For Quote

Requisition

Resource Allocations

Return Auth. Approval

Return Authorization

Return Authorization Reports

Revenue Recognition Reports

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order

Sales Order Approval

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Set Up Budgets

Shipping Partner Package

Shipping Partner Shipment

Statement Charge

Statistical Account Registers

Subscription Plan

Subscriptions

Subscription Change Orders

System Journal

Tax

Tax Details Tab

Tax Records

Tax Reports

Tegata Accounts

Tegata Payable

Tegata Receivables

Time Tracking

Timer

Track Time

Transfer Funds

Transfer Order

Trial Balance

Unbilled Receivable Registers

Units

Usage

Vendor Request For Quote

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Web Store Report

Work Calendar

Work Order

Work Order Close

Work Order Completion

Work Order Issue



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

Bills

Email Template

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

PDF Messages

PDF Template

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Analytical Impact

Automated Clearing House

Blanket Purchase Order

Calendar

Contacts

Deleted Records

Documents and Files

Employee Commission Transaction

Employee Record

Events

Find Transaction

General Token

Inbound Shipment

Log in using Access Tokens

Mobile Device Access

Notifications

Outlook Integration 2.0

Ownership Transfer

Payment Card

Payment Card Token

Payment Instruments

Perform Search

Phone Calls

Product Analytics Records

Project Tasks

Report Customization

Report Scheduling

Resource

Resource Allocation Approval

REST Web Services

SOAP Web Services

Tasks

Template Categories

Transfer Order Approval

Vendor Bill Approval

Vendor Payment Approval



 |

## CFO {#subsect_0425061352}

| CFO |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Account Detail

Accounts Payable

Accounts Payable Graphing

Accounts Receivable

Accounts Receivable Graphing

Amortization Reports

Balance Overview

Balance Sheet

Bill Of Materials Inquiry

Budget

Build Assemblies

Bulk Processing Submissions

Check Item Availability

Commission Reports

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Cross Charge Journal

Custom Record Types

Deferred Expense Reports

Employee Commission Schedules/Plans

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Expenses

Fair Value Dimension

Fair Value Formula

Fair Value Price

Financial Statements

General Ledger

Generate Price Lists

Generate Statements

Imported Employee Expenses

Income

Income Statement

Individual Paycheck

Installment Payment Links

Inventory

Item Fulfillment

Item Receipt

Item Revenue Category

Lead Snapshot/Reminders

Net Worth

Partner Authorized Commission Reports

Partner Commission Reports

Period End Financial Statements

Print Shipment Documents

Pricing Records

Project Profitability

Project Revenue Rules

Project Templates

Purchase Order Reports

Purchases

Quota Reports

Recognition Treatment

Recognition Treatment Rule

Resource Allocations

Return Authorization Reports

Revenue Arrangement

Revenue Arrangement Approval

Revenue Element

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Saas Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Shipping Partner Package

Shipping Partner Shipment

System Journal

Tax

Tax Records

Time Tracking

Unbuild Assemblies

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Balance Transactions by Segments

Export Lists

Kudos

Tableau® Workbook Export

Vendor Request For Quote



 | 

Netting Settlement Approval

Override Payment Hold

Subsidiary Settings Manager

SuiteAnalytics Workbook

Tax Details Tab

Tax Reports

Time-Off



 | 

Accounting Book

Accounting Lists

Accounting Management

Accounts

Accounts Payable Register

Accounts Receivable Register

Address List in Search

Adjust Inventory

Allocate Orders

Amortization Schedules

Analytical Impact

Approve Order Reservation

Audit Trail

Automated Cash Application

Balance Location Costing Group Accounts

Balancing Journals

Bank Account Registers

Bill Of Distribution

Bill of Materials

Bill Purchase Orders

Bills

Blanket Purchase Order

Blanket Purchase Order Approval

Build Work Orders

Calculate Time

Calendar

Cash Sale

Cash Sale Refund

Charge

Charge Rule

Charge - Run Rules

Check

Class Mapping

Classes

Close Work Orders

Competitors

Contacts

Copy Budgets

Count Inventory

Create Allocation Schedules

Create Inventory Counts

Credit Card Charge

Credit Card Refund

Credit Card Registers

Credit Memo

Credit Returns

CRM Groups

Currency Revaluation

Custom Recognition Event Type

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Customers

Deleted Records

Department Mapping

Departments

Deposit

Deposit Application

Distribution Network

Documents and Files

Earliest Availability

Email Template

Employee Commission Transaction

Employee Commission Transaction Approval

Employee Record

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Enter Year-To-Date Payroll Adjustments

Entity Account Mapping

Equity Registers



 | 

Events

Exception Management

Expense Amortization Plan

Expense Amortization Rule

Expense Report

Fax Messages

Fax Template

Finance Charge

Financial History

Find Transaction

Fixed Asset Registers

Foreign Currency Variance Mapping

Fulfill Orders

Generate Revenue Commitment

Generate Revenue Commitment Reversals

Gift Certificate

Global Account Mapping

Global Inventory Relationship

Import Online Banking File

Inbound Shipment

Intercompany Adjustments

Inventory Cost Template

Invoice

Invoice Approval

Invoice Sales Orders

Issue Components

Item Account Mapping

Item Revisions

Items

Journal Approval

Letter Messages

Letter Template

Location Costing Group

Location Mapping

Locations

Log in using Access Tokens

Long Term Liability Registers

Mail Merge

Make Journal Entry

Manage Cross Charge Automation

Manufacturing Cost Template

Manufacturing Routing

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Mass Updates

Matching Rules for Online Banking

Memorized Transactions

Mobile Device Access

Netting Settlement

Non Posting Registers

Notes Tab

Notifications

Opportunity

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Other Asset Registers

Other Current Asset Registers

Other Current Liability Registers

Other Lists

Other Names

Outlook Integration 2.0

Override Estimated Cost on Transactions

Ownership Transfer

Partner Commission Transaction

Partner Commission Transaction Approval

Pay Bills

Pay Sales Tax

Pay Tax Liability

Payroll Liability Payments

PDF Messages

PDF Template



 | 

Perform Search

Period End Journals

Phone Calls

Planned Standard Cost

Post Time

Post Vendor Bill Variances

Posting Period on Transactions

Price Books

Price Plans

Process GST Refund

Product Analytics Records

Projects

Project Budget

Project Intercompany Cross Charge Request

Project Tasks

Publish Search

Purchase Contract

Purchase Contract Approval

Purchase Order

Quote

Reallocate Order Item

Receive Order

Receive Returns

Reconcile

Reconcile Reporting

Refund Returns

Report Customization

Report Scheduling

Request For Quote

Requisition

Requisition Approval

Resource

Resource Allocation Approval

REST Web Services

Return Auth. Approval

Return Authorization

Revalue Inventory Cost

Revenue Commitment

Revenue Commitment Reversal

Revenue Management VSOE

Revenue Recognition Schedules

Sales Channel

Sales Order

Sales Order Approval

Scanned Vendor Bills

Set Up Budgets

SOAP Web Services

Standard Cost Version

Statement Charge

Statistical Account Registers

Subscription Change Orders

Subscription Plan

Subscriptions

Subsidiary - Tax Engine selection

Tasks

Tax Liability Payment

Tegata Accounts

Tegata Payable

Tegata Receivables

Template Categories

Timer

Track Messages

Track Time

Transaction Detail

Transfer Funds

Trial Balance

Unbilled Receivable Registers

Units

Usage

Vendor Bill Approval

Vendor Payment Approval

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

Work Breakdown Structure

Work Order

Work Order Close

Work Order Completion

Work Order Issue



 |

## Chief People Officer (CPO) {#subsect_0425061438}

| Chief People Officer (CPO) |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Commission Reports

Employee Commission Transaction

Employee Commission Transaction Approval

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Expense Categories

Find Transaction

Imported Employee Expenses

Individual Paycheck

Payroll Check Register

Payroll Hours & Earnings

Payroll Items

Payroll Summary & Detail Reports

Personal Banking Information

Purchase Order Reports

Tax Details Tab

Tax Reports

Workforce Analytics



 | 

Export Lists

Resource

Tableau® Workbook Export

Vendors



 | 

Email Template

Form W-2 - Wage and Tax Statement

Kudos

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Advanced Government Issued IDs

Amend W-4

Basic Government Issued IDs

Calendar

Chief People Officer (CPO)

Departments

Documents and Files

Edit Profile

Employee Effective Dating

Employee Change Reason

Employee Change Requests

Employee Change Request Types

Employee Effective Dating

Employee Record

Employee Social Security Numbers

Employees

Events

Expense Report

Generic Resources

Government Issued ID Types

Job Management

Job Requisitions

Locations

Manage Users

News Item

Notes Tab

Notifications

Onboarding Administration

Onboarding Plan

Onboarding Task

Organization Value

Other Lists

Perform Search

Phone Calls

Positions

Product Analytics Records

Report Customization

Report Scheduling

Talent Administration

Tasks

Template Categories

Termination Reasons

Time-Off Administration

Track Time

View Login Audit Trail

Work Calendar

Workplaces



 |

## Consultant {#subsect_0425061504}

| Consultant |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Accounts Receivable Un-Billed

Bulk Processing Submissions

Classes

Customers

Departments

Entity-Subsidiary relationship

Imported Employee Expenses

Locations

Non Posting Registers

Price Books

Price Plans

Project Profitability

Projects

Statistical Account Registers

Subscriptions

Subscription Change Orders

Time Tracking



 | 

Kudos

Project Tasks



 | 

Calendar

Cases

Documents and Files

Find Transaction

Perform Search

Purchase Order

Requisition

SuiteAnalytics Workbook



 | 

Address List in Search

Events

Expense Report

Notification

Phone Calls

Product Analytics Records

Report Scheduling

Resource Allocations

Tasks

Track Time



 |

## Customer Center {#subsect_0425061528}

| Customer Center |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Accounts Receivable Register

Cash Sale

Cardholder Authentications

Charge

Charge Rule

Credit Memo

Customer Deposit

Customer Payment Authorization

Estimate

Fulfill Orders

Installment Payment Links

Invoice

Issues

Items

Non Posting Registers

Perform Search

Price Plans

Return Authorization Reports

Sales Order Transaction Report

Subscription Change Orders

Subscriptions

Track Messages



 | 

Deposit Application

Export Lists

Generate Statements

Item Fulfillment

Print Shipment Documents

Return Authorization

Shipping Partner Package

Shipping Partner Shipment

Tableau&reg; Workbook Export



 | 

Automated Clearing House

Cases

Cardholder Authentication

Contacts

Customer Payment

Customer Profile

Gift Certificate

General Token

Payment Card

Payment Card Token

Sales Order



 | 

Charge - Run Rules

Deleted Records

Find Transaction

Perform Search

Log in using Access Tokens

Notifications

Payment Instruments

REST Web Services

SOAP Web Services



 |

## Developer {#subsect_0425061553}

| Developer |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| \- | \- | 
SuiteAnalytics Workbook



 | 

Address List in Search

Advanced PDF/HTML Templates

Allow JS / HTML Uploads

Bulk Manage Roles

Create HTML Formulas in Search

CRM Lists

Custom Address Form

Custom Body Fields

Custom Center Categories

Custom Center Links

Custom Center Tabs

Custom Centers

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Item Fields

Custom Item Number Fields

Custom Lists

Custom PDF Layouts

Custom Record Entries

Custom Record Types

Custom Segments

Custom Sublist

Custom Sublists

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Custom Transaction Types

Documents and Files

Email Template

Enable Features

Import CSV File

KPI Scorecards

Log in using Access Tokens

Log in using OAuth 2.0 Access Tokens

Manage Custom Permissions

Manage Translation

Marketing Template

Other Custom Fields

PDF Template

Perform Search

Product Analytics Records

Publish Dashboards

Publish Search

REST Web Services

Set Up CSV Preferences

Set Up Web Site

SOAP Web Services

SuiteApp Deployment

SuiteApp Marketplace

SuiteScript

SuiteScript Scheduling

User Access Tokens

Vicarious emails

Website (External) publisher

Workflow



 |

## Employee Center {#subsect_0425061617}

| Employee Center |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Amend W-4 (Payroll)

Bills

Bonus (SuitePeople HR)

Commission Reports (Incentive Compensation)

Employee Compensation (SuitePeople HR)

Employee Confidential (SuitePeople HR)

Employee Public (SuitePeople HR)

Employee Reminders

Employee Self (SuitePeople HR)

Employee Social Security Numbers

Expense Report Policies

Financial History

Imported Employee Expenses

Individual Paycheck (Payroll)

News Items

Non Posting Registers

Personal Banking Information

Project Profitability (Project Management)

Resource Allocations

Sales Order Transaction Report

Time Tracking

Vendor Prepayment (Procurement)

Work Calendar



 | 

Export Lists

Kudos (SuitePeople HR)

Resource

Tableau® Workbook Export



 | 

Contacts

Edit Profile

Employee Record

Notes Tab

Onboarding Plan (SuitePeople HR)

Onboarding Task (SuitePeople HR)

Time-Off

SuiteAnalytics Workbook



 | 

Address List in Search

Calendar

Cases

Deleted Records

Documents and Files

Events

Expense Report

Find Transaction

Log in using Access Tokens

Mobile Device Access

Notifications

OAuth 2.0

OpenID Connect (OIDC) Single Sign-on

OpenID Single Sign-on

Perform Search

Phone Calls

Print/Email/Fax

Project Tasks (Project Management)

Purchase Order

Request For Quote (Procurement)

Requisition (Procurement)

Requisition Approval (Procurement)

Resource Allocation Approval

REST Web Services

SAML Single Sign-on

SOAP Web Services

Talent Employee

Talent Employee (Performance Management)

Tasks

Tax Details Tab

Tax Registrations Tab

Tax Reports

Track Messages

Track Time

User Access Tokens

Vendor Bill Approval

Vendor Prepayment Approval (Procurement)

Vendor Request For Quote (Procurement)



 |

Permissions enabled by modules indicated as follows:

-   Payroll = NetSuite SuitePeople US Payroll Cloud Service
    
-   Project Management = NetSuite SuiteProject Management Mid-Market Cloud Service
    
-   SuitePeople HR = NetSuite SuitePeople HR Cloud Service
    
-   Incentive Compensation = NetSuite Incentive Compensation Mid Market Cloud Service
    
-   Procurement = NetSuite Procurement Management Mid-Market Cloud Service
    
-   Performance Management = NetSuite SuitePeople Performance Management Cloud Service
    

## Employee Center with Highest Access Levels Shown {#subsect_78193907376}

| Employee Center |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bills

Bonus (SuitePeople HR)

Commission Reports (Incentive Compensation)

Employee Reminders

Employee Social Security Numbers

Financial History

Imported Employee Expenses

Individual Paycheck (Payroll)

Non Posting Registers

Project Profitability (Project Management)

Resource Allocations

Sales Order Transaction Report

Time Tracking

Vendor Prepayment (Procurement)

Work Calendar



 | 

Export Lists

Kudos (SuitePeople HR)

Resource

Tableau® Workbook Export



 | 

Contacts

Employee Record

Notes Tab

SuiteAnalytics Workbook

Tax Details Tab



 | 

Amend W-4 (Payroll)

Address List in Search

Calendar

Cases

Deleted Records

Documents and Files

Edit Profile

Employee Compensation (SuitePeople HR)

Employee Confidential (SuitePeople HR)

Employee Public (SuitePeople HR)

Employee Self (SuitePeople HR)

Events

Expense Reports

Expense Report Policies

Find Transaction

Log in using Access Tokens

Mobile Device Access

Notifications

OAuth 2.0

Onboarding Plan (SuitePeople HR)

Onboarding Task (SuitePeople HR)

OpenID Connect (OIDC) Single Sign-on

OpenID Single Sign-on

Perform Search

Personal Banking Information

Phone Calls

Print/Email/Fax

Project Tasks (Project Management)

Purchase Orders

Request For Quote (Procurement)

Requisition (Procurement)

Requisition Approval (Procurement)

Resource Allocation Approval

REST Web Services

SAML Single Sign-on

SOAP Web Services

Talent Employee (Performance Management)

Tasks

Tax Registrations Tab

Tax Reports

Track Messages

Track Time

User Access Tokens

Vendor Bill Approval

Vendor Prepayment Approval (Procurement)

Vendor Request For Quote (Procurement)



 |

Permissions enabled by modules indicated as follows:

-   Payroll = NetSuite SuitePeople US Payroll Cloud Service
    
-   Project Management = NetSuite SuiteProject Management Mid-Market Cloud Service
    
-   SuitePeople HR = NetSuite SuitePeople HR Cloud Service
    
-   Incentive Compensation = NetSuite Incentive Compensation Mid Market Cloud Service
    
-   Procurement = NetSuite Procurement Management Mid-Market Cloud Service
    
-   Performance Management = NetSuite SuitePeople Performance Management Cloud Service
    

## Engineer {#subsect_0425061645}

| Engineer |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Contacts

Contact-Subsidiary relationship

Email Template

Employee Public

Employee Record

Entity-Subsidiary relationship

Template Categories

Track Messages



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

Issue Reports

Issues

Mail Merge

Mark Issue As Showstopper

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Admindocs

Calendar

Deleted Records

Documents and Files

Events

Log in using Access Tokens

Mobile Device Access

Notes Tab

Notifications

Perform Search

Product Analytics Records

Report Scheduling

REST Web Services

SOAP Web Services

Tasks



 |

## Engineering Manager {#subsect_0425061707}

| Engineering Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Contacts

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Track Messages



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

Issues

Perform Search

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Admindocs

Calendar

Deleted Records

Documents and Files

Events

Issue Reports

Log in using Access Tokens

Mark Issue As Showstopper

Mobile Device Access

Notes Tab

Notifications

Product Analytics Records

Report Scheduling

REST Web Services

SOAP Web Services

Tasks



 |

## Human Resources Generalist {#subsect_0425061940}

| Human Resources Generalist |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Commission Reports

Employee Commission Transaction

Employee Commission Transaction Approval

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Expense Categories

Find Transaction

Imported Employee Expenses

Individual Paycheck

Payroll Chek Register

Payroll Hours & Earnings

Payroll Items

Payroll Summary & Detail Reports

Purchase Order Reports

Workforce Analytics



 | 

Export Lists

Resource

Tableau® Workbook Export

Vendors



 | 

Email Template

Form W-2 - Wage and Tax Statement

Kudos

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Advanced Government Issued IDs

Amend W-4

Basic Government Issued IDs

Bonus

Bonus Types

Calendar

Departments

Documents and Files

Edit Profile

Employee Effective Dating

Employee Change Reason

Employee Change Request

Employee Change Request type

Employee Record

Employees

Employee Social Security Numbers

Events

Expense Report

Generic Resources

Government Issued ID Types

Job Management

Job Requisitions

Locations

Manage Users

Mass Updates

News Items

Notes Tab

Notifications

Onboarding Administration

Onboarding Plan

Onboarding Task

Organization Value

Other Lists

Perform Search

Personal Banking Information

Phone Calls

Positions

Product Analytics Records

Report Customization

Report Scheduling

Talent Administration

Talent Employee

Tasks

Template Categories

Termination Reasons

Time-Off Administration

Track Time

View Login Audit Trail

Work Calendar

Workplaces



 |

## Intranet Manager {#subsect_0425062018}

| Intranet Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bill Of Materials Inquiry

Bulk Processing Submissions

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Find Transaction

Notes Tab

Pricing Records

Web Site Report

Web Store Report



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Email Template

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Allow JS / HTML Uploads

Bill of Materials

Calendar

Color Themes

Custom Item Fields

Deleted Records

Documents and Files

Events

Internal Publisher

Item/Category Layouts

Items

Log in using Access Tokens

Mobile Device Access

Notifications

Online Customer Form

Perform Search

Phone Calls

Presentation Categories

Publish Employee List

Publish Forms

Publish RSS Feeds

Product Analytics Records

Related Items

Report Scheduling

REST Web Services

Set Up Image Resizing

Set Up Web Site

SOAP Web Services

Store Categories

Store Content Categories

Store Content Items

Store Tabs

Tasks

Template Categories

Units

Website (External) publisher



 |

## Issue Administrator {#subsect_0425062044}

| Issue Administrator |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Employee Public

Employee Record



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Calendar

CRM Groups

Deleted Records

Documents and Files

Events

Import CSV File

Issue Reports

Issue Setup

Issues

Log in using Access Tokens

Mark Issue As Showstopper

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Perform Search

Product Analytics Records

Publish Dasboards

Publish Search

Report Scheduling

REST Web Services

SOAP Web Services

Tasks



 |

## Marketing Administrator {#subsect_0425062104}

| Marketing Administrator |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Cases

Contact-Subsidiary relationship

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Financial History

Find Transaction

Lead Snapshot/Reminders

Marketing Campaign Reports

Price Books

Price Plans

Project Templates

Quota Reports

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Subscription Plan

Web Site Report

Work Calendar



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

Classes

Departments

Email Template

Locations

SuiteAnalytics Workbook

Time-Off

Track Messages

Vendors



 | 

Address List in Search

Backup Your Data

Bulk Manage Roles

Calendar

Campaign History

Color Themes

Companies

Competitors

Contact Roles

Contacts

CRM Groups

CRM Lists

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Item Fields

Custom Lists

Custom PDF Layouts

Custom Record Entries

Custom Record Types

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Customer Profile

Customer Segments Manager

Customer Status

Customers

Delete Event

Deleted Records

Documents and Files



 | 

Duplicate Detection Setup

Duplicate Entity Management

Employee Record

Employees

Events

Fax Messages

Fax Template

Import CSV File

Intelligent Recommendations

Internal Publisher

Item Collection

Knowledge Base

KPI Scoreboards

Letter Messages

Letter Template

Log in using Access Tokens

Mail Merge

Manage Users

Marketing Campaigns

Marketing Template

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Online Custom Record Form

Online Customer Form

Other Names

Partners

PDF Messages



 | 

PDF Template

Perform Search

Phone Calls

Presentation Categories

Product Analytics Records

Project Tasks

Projects

Promotion

Public Template Categories

Publish Dashboards

Publish Knowledge Base

Publish Search

Record Custom Field

Report Customization

Report Scheduling

Resource

REST Web Services

Sales Force Automation Setup

Sales Order Reports

Setup Campaign Email Addresses

Set Up Domains

Setup Campaigns

Shortcuts

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Template Categories

Two-Factor Authentication base

Upsell Assistant

Upsell Setup

Upsell Wizard

Users & Passwords



 |

## Marketing Assistant {#subsect_0425062129}

| Marketing Assistant |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bill Of Materials

Bill of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Public

Employee Record

Entity-Subsidiary relationship

Financial History

Items

Lead Snapshot/Reminders

Marketing Campaign Reports

Price Books

Price Plans

Pricing Records

Project Templates

Quota Reports

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Reports

Subscription Plan

Units

Work Calendar



 | 

Export Lists

Kudos

Knowledge Base

Tableau® Workbook Export



 | 

CRM Lists

Email Template

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

Partners

PDF Messages

PDF Template

Promotion

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Allow JS / HTML Uploads

Calendar

Campaign History

Companies

Competitors

Contacts

CRM Groups

Customers

Deleted Records

Documents and Files

Duplicate Entity Management

Events

Find Transaction

Intelligent Recommendations

Log in using Access Tokens

Marketing Campaigns

Marketing Template

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Perform Search

Phone Calls

Product Analytics Records

Project Tasks

Projects

Publish RSS Feeds

Report Customization

Report Scheduling

Resource

REST Web Services

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Template Categories

Upsell Assistant

Upsell Setup

Upsell Wizard

Website (External) Publisher



 |

## Marketing Manager {#subsect_0425062152}

| Marketing Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Financial History

Items

Lead Snapshot/Reminders

Marketing Campaign Reports

Price Books

Price Plans

Pricing Records

Project Templates

Quota Reports

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Reports

Subscription Plan

Units

Web Site Report

Web Store Report

Work Calendar



 | 

Export Lists

Knowledge Base

Kudos

Tableau® Workbook Export



 | 

CRM Lists

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Event Fields

Custom Fields

Custom Lists

Email Template

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

PDF Messages

PDF Template

Publish Knowledge Base

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Calendar

Campaign History

Companies

Competitors

Contact Roles

Contacts

CRM Groups

Custom Transaction Forms

Customer Segments Manager

Customer Status

Customers

Deleted Records

Documents and Files

Duplicate Entity Management

Events

Find Transaction

Intelligent Recommendations

Internal Publisher

Item Collection

Log in using Access Tokens

Marketing Campaigns

Marketing Template

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Online Customer Form

Outlook Integration 2.0

Partners

Perform Search

Phone Calls

Product Analytics Records

Project Tasks

Projects

Promotion

Public Template Categories

Report Customization

Report Scheduling

REST Web Services

Resource

Sales Territory Rule

Set Up Campaign Email Addresses

Set Up Image Resizing

Setup Campaigns

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Template Categories

Upsell Assistant

Upsell Setup

Upsell Wizard



 |

## Partner Center {#subsect_0425062219}

| Partner Center |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Find Transaction

Notes Tab

Partner Commission Reports

Price Books

Price Plans

Project Templates

Resource Allocations

Sales By Partner

Sales By Promotion



 | 

Export Lists

Tableau® Workbook Export



 | 

Competitors

Customers

Jobs

Projects

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook



 | 

Deleted Records

Log in using Access Tokens

Notifications

Partners

Perform Search

Promotion

Resource Allocation Approval

REST Web Services

SOAP Web Services



 |

## Payroll Manager {#subsect_0425062243}

| Payroll Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Financial History

Find Transaction

Form 940 - Employer's Annual Federal Unemployment Tax Return

Form 941 - Employer's Quarterly Federal Tax Return

Form W4 - Employee's Withholding Allowance Certificate

Make Journal Entry

Manage Payroll

Notes Tab

Payroll Hours & Earnings

Payroll Check Register

Payroll Journal Report

Payroll Liability Report

Payroll Summary & Detail Reports

Project Profitability

Time Tracking



 | 

Export Lists

Kudos

Posting Period on Transactions

Resource

Tableau® Workbook Export



 | 

Email Template

Form W-2 - Wage and Tax Statement

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Calendar

Contacts

Deleted Records

Documents and Files

Employee Record

Employee Social Security Numbers

Employees

Enter Year-To-Date Payroll Adjustments

Events

Individual Paycheck

Log in using Access Tokens

Mobile Device Access

Notifications

Paychecks

Payroll Items

Payroll Liability Payments

Perform Search

Phone Calls

Process Payroll

Product Analytics Records

Report Customization

Report Scheduling

REST Web Services

Run Payroll

Set Up Payroll

SOAP Web Services

Tasks

Template Categories

Track Time

Vendors

Workplaces



 |

## Payroll Setup {#subsect_0425062306}

| Payroll Setup |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Financial History

Find Transaction

Form 940 - Employer's Annual Federal Unemployment Tax Return

Form 941 - Employer's Quarterly Federal Tax Return

Form W4 - Employee's Withholding Allowance Certificate

Make Journal Entry

Manage Payroll

Notes Tab

Payroll Check Register

Payroll Journal Report

Payroll Liability Report

Payroll Summary & Detail Reports

Project Profitability

Time Tracking



 | 

Export Lists

Kudos

Posting Period on Transactions

Resource

Tableau® Workbook Export



 | 

Email Template

Form W-2 - Wage and Tax Statement

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Calendar

Contacts

Deleted Records

Documents and Files

Employee Record

Employee Social Security Numbers

Employees

Enter Year-To-Date Payroll Adjustments

Events

Individual Paycheck

Locations

Log in using Access Tokens

Mobile Device Access

Notifications

Paychecks

Payroll Items

Payroll Liability Payments

Perform Search

Phone Calls

Process Payroll

Product Analytics Records

Report Customization

Report Scheduling

REST Web Services

Run Payroll

Set Up Payroll

SOAP Web Services

Tasks

Template Categories

Track Time

Vendors

Workplaces



 |

## PM Manager {#subsect_0425062331}

| PM Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Find Transaction

Lead Snapshot/Reminders

Partners

Project Templates

Provisioning

Support

Support Case Snapshot/Reminders

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Companies

Contacts

CRM Groups

Email Template

Issue Reports

Issues

Mark Issue As Showstopper

Opportunity

Perform Search

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Cases

Competitors

Customers

Documents and Files

Events

Financial History

Jobs

Knowledge Base

KPI Scoreboards

Mail Merge

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Phone Calls

Product Analytics Records

Project Budget

Project Tasks

Publish Dashboards

Publish Knowledge Base

Report Customization

Report Scheduling

Resource Allocation Approval

Resource Allocations

Subscriptions

Tasks

Template Categories

Work Breakdown Structure



 |

## Product Manager {#subsect_0425062353}

| Product Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bulk Processing Submissions

Charge

Charge Rule

Contact-Subsidiary relationship

Credit Memo

Employee Public

Employee Record

Entity-Subsidiary relationship

Find Transaction

Gift Certificate

Installment Payment Links

Invoice

Lead Snapshot/Reminders

Partners

Price Books

Price Plans

Project Templates

Provisioning

Sales Order

Support

Support Case Snapshot/Reminders

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Companies

Contacts

CRM Groups

Email Template

Issues

Opportunity

Perform Search

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Cases

Competitors

Customers

Deleted Records

Documents and Files

Events

Financial History

Charge - Run Rules

Issue Reports

Knowledge Base

Log in using Access Tokens

Mail Merge

Mark Issue As Showstopper

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Outlook Integration 2.0

Phone Calls

Product Analytics Records

Project Tasks

Projects

Publish Knowledge Base

Report Customization

Report Scheduling

REST Web Services

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Template Categories



 |

## QA Engineer {#subsect_0425062416}

| QA Engineer |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Employee Public

Employee Record



 | Kudos | 

Issue Reports

Issues

Mark Issue As Showstopper

Perform Search

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Documents and Files

Events

Mobile Device Access

Notes Tab

Notifications

Product Analytics Records

System Status

Tasks



 |

## QA Manager {#subsect_0425062438}

| QA Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Cases

Employee Compensation

Employee Confidential

Employee Public

Employee Record



 | Kudos | 

Issues

Perform Search

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Documents and Files

Events

Issue Reports

Issue Setup

KPI Scorecards

Mark Issue As Showstopper

Mobile Device Access

Notes Tab

Notifications

Product Analytics Records

Publish Dashboards

System Status

Tasks



 |

## Resource Manager {#subsect_0425062508}

| Resource Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Audit Trail

Bill of Materials

Calendar

Contact-Subsidiary relationship

Contacts

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom HTML Layouts

Custom Item Fields

Custom Item Number Fields

Custom Lists

Custom PDF Layouts

Custom Record Entries

Custom Record Types

Custom Sublists

Custom Subtabs

Email Template

Employee Public

Employee Reminders

Employees

Entity-Subsidiary relationship

Generic Resources



 | 

Import CSV File

Items

KPI Scorecards

Locations

Mass Updates

Notes Tab

Other Custom Fields

Outlook Integration 2.0

Price Books

Price Plans

Pricing Records

Project Profitability

Project Templates

Report Customization

Report Scheduling

Subscription Plan

Subsidiaries

SuiteScript

SuiteSignOn

Tasks

Template Categories

Time Tracking

Two-Factor Authentication

Two-Factor Authentication base

Usage

Vendors

Work Calendar

Workflow



 | 

Custom Body Fields

Custom Center Categories

Custom Center Links

Custom Centers

Custom Column Fields

Custom Transaction Forms

Kudos

Perform Search

Publish Forms

Publish Search



 | 

Customers

Events

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Deleted Records

Documents and Files

Employee Record

Mobile Device Access

Notifications

Product Analytics Records

Project Tasks

Projects

Resource Allocation Approval

Resource Allocations

Review Custom GL Plug-in Executions

Subscriptions

Subscription Change Orders

Vicarious emails



 |

## Retail Clerk {#subsect_0425062536}

Note that this role cannot be customized. See [Retail Clerk Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291985.html).

| Retail Clerk (Note that this role cannot be customized. See [Retail Clerk Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291985.html).) |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Calendar

Contact-Subsidiary relationship

Edit Profile

Employee Public

Employee Record

Employee Reminders

Entity-Subsidiary relationship

Events

Fulfill Orders

Installment Payment Links

Item Fulfillment

Items

Locations

Personal Banking Information

Pricing Records

Print Shipment Documents

Project Profitability

Purchase Order

Requistion

Sales Order Fulfillment Reports

Shipping Partner Package

Shipping Partner Shipment

Tasks

Time Tracking

Track Messages

Track Time

Transaction Detail

View Gateway Asynchronous Notifications

View Payment Events



 | 

Kudos

Phone Calls



 | 

Contacts

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Cases

Charge

Charge Rule

Charge - Run Rules

Credit Memo

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Customers

Deposit Application

Documents and Files

Find Transaction

Gift Certificate

Invoice

Invoice Approval

Invoice Sales Orders

Mobile Device Access

Notes Tab

Notifications

Perform Search

Product Analytics Records

Sales Order

Transfer Order

Transfer Order Approval



 |

## Retail Clerk (Web Services Only) {#subsect_0425062632}

Note that this role cannot be customized. See [Retail Clerk Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291985.html)

| Retail Clerk (Web Services Only) (Note that this role cannot be customized. See [Retail Clerk Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N291985.html).) |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bill Of Materials Inquiry

Bulk Processing Submissions

Currency

Employee Public

Employees

Installment Payment Links

Locations

Pricing Records

View Gateway Asynchronous Notifications

View Payment Events



 | 

Kudos



 | 

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Bill of Materials

Charge

Charge Rule

Charge - Run Rules

Credit Memo

Custom Record Entries

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Customers

Deleted Records

Deposit Application

Documents and Files

Employee Record

Find Transaction

Gift Certificate

Invoice

Invoice Approval

Items

Log in using Access Tokens

Mobile Device Access

Notifications

Product Analytics Records

REST Web Services

Sales Order

SOAP Web Services

Set Up SOAP Web Services

Track Time

Transfer Order

Transfer Order Approval

View Unencrypted Credit Cards

View Unencrypted General Tokens

View Unencrypted Payment Card Tokens

View SOAP Web Services Logs



 |

## Revenue Accountant {#subsect_0425062709}

| Revenue Accountant |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Account Detail

Balance Sheet

Bill Of Materials

Billing Schedules

Bulk Processing Submissions

Create Allocation Schedules

Currency

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Employee Public

Employee Reminders

Employees

Entity-Subsidiary relationship

Financial Statements

Fulfill Orders

General Ledger

Income

Income Statement

Installment Payment Links

Item Fulfillment

Item Revisions

Items

Pricing Records

Projects

Project Profitability

Purchase Order

Reconcile Reporting

Sales Order Fulfillment Reports

Sales Order Reports

Tax Details Tab

Time Tracking

Trial Balance

Units



 | 

Kudos

Resource



 | 

Accounts

Accounts Receivable

Cash Sale

Cash Sale Refund

Credit Memo

Customers

Email Template

Fair Value Dimension

Fair Value Formula

Fair Value Price

Gift Certificate

Invoice

Invoice Sales Orders

ltem Revenue Category

Non Posting Registers

Recognition Treatment

Recognition Treatment Rule

Return Authorization

Revenue Recognition Field Mapping

Sales Order

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Amortization Reports

Amortization Schedules

Calendar

Custom Recognition Event Type

Deferred Expense Reports

Documents and Files

Employee Record

Events

Expense Amortization Plan

Expense Amortization Rule

Find Transaction

Generate Revenue Commitment

Generate Revenue Commitment Reversals

Make Journal Entry

Mass Updates

Notes Tab

Notifications

Perform Search

Phone Calls

Product Analytics Records

Project Revenue Rules

Project Tasks

Report Customization

Report Scheduling

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Element



 | 

Revenue Management VSOE

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

Tasks

Template Categories



 |

## Revenue Manager {#subsect_0425062734}

| Revenue Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Account Detail

Balance Sheet

Bulk Processing Submissions

Create Allocation Schedules

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Refund

Employee Public

Employee Reminders

Employees

Entity-Subsidiary relationship

Financial Statements

Fulfill Orders

General Ledger

Income

Income Statement

Installment Payment Links

Item Fulfillment

Pricing Records

Project Profitability

Projects

Purchase Order

Reconcile Reporting

Sales Order Fulfillment Reports

Sales Order Reports

Time Tracking

Trial Balance

Units



 | 

Kudos

Resource



 | 

Accounts

Accounts Receivable

Bill Of Materials

Billing Schedules

Cash Sale

Cash Sale Refund

Credit Memo

Currency

Customers

Email Template

Gift Certificate

Invoice

Invoice Sales Orders

Item Revisions

Items

Non Posting Registers

Return Authorization

Sales Order

SuiteAnalytics Workbook

Time-Off



 | 

Accounting Lists

Accounting Management

Accounting Preferences

Address List in Search

Amortization Reports

Amortization Schedules

Calendar

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Item Fields

Custom Lists

Custom PDF Layouts

Custom Recognition Event Type

Custom Record Types

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Deferred Expense Reports

Documents and Files

Employee Record



 | 

Enable Features

Events

Expense Amortization Plan

Expense Amortization Rule

Fair Value Dimension

Fair Value Formula

Fair Value Price

Find Transaction

Generate Revenue Commitment

Generate Revenue Commitment Reversals

Item Revenue Category

Make Journal Entry

Mass Updates

Notes Tab

Notifications

Other Lists

Perform Search

Phone Calls

Product Analytics Records

Project Revenue Rules

Project Tasks

Recognition Treatment

Recognition Treatment Rule

Report Customization

Report Scheduling

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Element

Revenue Management VSOE

Revenue Recognition Field Mapping

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

Tasks

Template Categories



 |

## Sales Administrator {#subsect_0425062759}

| Sales Administrator |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Receivable

Accounts Receivable Register

Bill Of Materials Inquiry

Bill of Materials

Commission Reports

Contact-Subsidiary relationship

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Financial History

Items

Lead Snapshot/Reminders

Marketing Campaign Reports

Non Posting Registers

Pricing Records

Project Templates

Quota Reports

Resource Allocations

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Shipping Items

Shipping Partner Registration

Statistical Account Registers

Subscription Plan

Unbilled Receivable Registers

Units

Usage

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Cash Sale

CRM Lists

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Event Fields

Custom Fields

Custom Lists

Custom Subtabs

Custom Transaction Fields

Mass Updates

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Analytical Impact

Bulk Manage Roles

Calendar

Commission Feature Setup

Companies

Competitors

Contact Roles

Contacts

CRM Groups

Custom Entry Forms

Custom Transaction Forms

Customer Segments Manager

Customer Status

Customers

Deleted Records

Documents and Files

Duplicate Detection Setup

Duplicate Entity Management

Edit Forecast

Edit Manager Forecast

Email Template

Employee Commission Schedules/Plans

Employee Commission Transaction

Employee Record

Employees

Establish Quotas

Events

Fax Messages

Fax Template



 | 

Find Transaction

Gift Certificate

Intelligent Recommendations

Internal Publisher

Item Collection

KPI Scorecards

Lead Conversion

Lead Conversion Mapping

Letter Messages

Letter Template

Log in using Access Tokens

Mail Merge

Manage Users

Marketing Template

Mobile Device Access

Notes Tab

Notifications

Online Customer Form

Opportunity

Outlook Integration 2.0

Override Estimated Cost on Transactions

Partner Authorized Commission Reports

Partner Commission Reports

Partner Commission Schedules/Plans

Partner Commission Transaction

Partner Contribution

PDF Messages

PDF Template

Perform Search

Phone Calls

Price Books

Price Plans

Product Analytics Records

Project Tasks

Projects

Promotion

Publish Dashboards

Publish Search

Quote

Report Customization

Report Scheduling

Resource Allocation Approval

REST Web Services

Sales Campaigns

Sales Force Automation Setup

Sales Order

Sales Order Approval

Sales Territory

Sales Territory Rule

Set Up Domains

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Team Selling Contribution

Telephony Integration

Template Categories

Track Messages

Two-Factor Authentication base

Upsell Assistant

Upsell Setup

Upsell Wizard



 |

## Sales Manager {#subsect_0425062826}

| Sales Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Receivable

Accounts Receivable Register

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Cases

Check Item Availability

Commission Reports

Commit Orders

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Item Revisions

Items

Lead Snapshot/Reminders

Marketing Campaigns

Marketing Campaign Reports

Non Posting Registers

Pricing Records

Project Templates

Quota Reports

Resource Allocations

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Statistical Account Registers

Subscription Plan

Unbilled Receivable Registers

Units

Usage

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Web Store Report

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Campaign History

Cash Sale

CRM Lists

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Fields

Custom Lists

Custom Subtabs

Custom Transaction Fields

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

Mass Updates

Override Payment Hold

PDF Messages

PDF Template

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Allocate Orders

Analytical Impact

Approve Order Reservation

Bill Of Distribution

Calendar

Commission Feature Setup

Companies

Competitors

Contact Roles

Contacts

CRM Groups

Custom Entry Forms

Custom Transaction Forms

Customer Segments Manager

Customer Status

Customers

Deleted Records

Distribution Network

Documents and Files

Earliest Availability

Edit Forecast

Edit Manager Forecast

Email Template

Employee Commission Schedules/Plans

Employee Commission Transaction

Establish Quotas



 | 

Events

Find Transaction

Gift Certificate

Global Inventory Relationship

Internal Publisher

Intelligent Recommendations

Item Collection

Lead Conversion

Lead Conversion Mapping

Log in using Access Tokens

Marketing Template

Mobile Device Access

Notes Tab

Notifications

Online Customer Form

Opportunity

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Outlook Integration 2.0

Override Estimated Cost on Transactions

Partner Commission Schedules/Plans

Partner Commission Transaction

Partner Contribution

Perform Search

Phone Calls

Price Books

Price Plans

Product Analytics Records

Projects

Project Tasks

Promotion

Quote

Reallocate Order Item

Report Customization

Report Scheduling

Resource Allocation Approval

REST Web Services

Sales Campaigns

Sales Channel

Sales Order

Sales Order Approval

Sales Territory

Sales Territory Rule

Set Up Image Resizing

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Team Selling Contribution

Template Categories

Track Messages

Upsell Assistant

Upsell Setup

Upsell Wizard



 |

## Sales Person {#subsect_0425062854}

| Sales Person |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Cases

Commission Reports

Contact-Subsidiary relationship

CRM Lists

Duplicate Entity Management

Employee Commission Transaction

Employee Public

Employee Record

Entity-Subsidiary relationship

Items

Lead Snapshot/Reminders

Marketing Campaigns

Marketing Campaign Reports

Non Posting Registers

Pricing Records

Project Templates

Quota Reports

Resource Allocations

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Subscription Plan

Units

Usage

View Gateway Asynchronous Notifications

View Payment Events

Work Calendar



 | 

Export Lists

Kudos

Notes Tab

Resource

Tableau® Workbook Export



 | 

Campaign History

Cash Sale

Edit Forecast

Fax Messages

Fax Template

Gift Certificate

Letter Messages

Letter Template

Mail Merge

Mass Updates

Opportunity

PDF Messages

PDF Template

Sales Order

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Calendar

Competitors

Contacts

CRM Groups

Customers

Deleted Records

Documents and Files

Email Template

Events

Find Transaction

Lead Conversion

Lead Conversion Mapping

Log in using Access Tokens

Marketing Template

Mobile Device Access

Notifications

Outlook Integration 2.0

Perform Search

Phone Calls

Price Books

Price Plans

Product Analytics Records

Projects

Project Tasks

Quote

Report Customization

Report Scheduling

Resource Allocation Approval

REST Web Services

Sales Campaigns

SOAP Web Services

Subscriptions

Subscription Change Orders

Tasks

Template Categories

Track Messages

Upsell Assistant



 |

## Sales Vice President {#subsect_0425062918}

| Sales Vice President |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Receivable

Accounts Receivable Register

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Cases

Check Item Availability

Commission Reports

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Employee Public

Employee Record

Entity-Subsidiary relationship

Item Revisions

Items

Lead Snapshot/Reminders

Marketing Campaigns

Non Posting Registers

Price Books

Price Plans

Pricing Records

Quota Reports

SaaS Metric

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Statistical Account Registers

Subscription Change Orders

Subscriptions

Subscription Plan

Usage

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Web Store Report



 | 

Export Lists

Kudos

Tableau® Workbook Export



 | 

Campaign History

Cash Sale

Fax Messages

Fax Template

Letter Messages

Letter Template

Mail Merge

Mass Updates

Override Payment Hold

PDF Messages

PDF Template

SuiteAnalytics Workbook

Time-Off



 | 

Address List in Search

Allocate Orders

Analytical Impact

Approve Order Reservation

Bill Of Distribution

Calendar

Companies

Competitors

Contact Roles

Contacts

CRM Groups

Customers

Distribution Network

Documents and Files

Earliest Availability

Edit Forecast

Edit Manager Forecast

Email Template

Establish Quotas

Events

Find Transaction

Gift Certificate

Global Inventory Relationship

Manufacturing Cost Template

Manufacturing Routing

Mobile Device Access

Notes Tab

Notifications

Opportunity

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Perform Search

Phone Calls

Product Analytics Records

Quote

Reallocate Order Item

Report Customization

Report Scheduling

Sales Campaigns

Sales Channel

Sales Order

Sales Order Approval

Subsidiary - Tax Engine selection

Tasks

Template Categories

Track Messages



 |

## Specialized User: CRM {#subsect_0708012605}

| Specialized User: CRM |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Accounts Receivable

Accounts Receivable Register

Adjust Inventory

Bulk Processing Submissions

Companies

Contact Roles

Credit Returns

Custom Center Categories

Custom Center Link

Custom Center Links

Custom Center Tabs

Custom Centers

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom HTML Layouts

Custom Item Fields

Custom Item Number Fields

Custom Lists

Custom PDF Layouts

Custom Record Types

Custom Segments

Custom Sublist

Custom Sublists

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Custom Transaction Types

Customer Deposit

Customer Payment

Customer Segments Manager

Customer Status

Customize Field Level Help

Delete Event

Delete Records

Email Template

Employee Reminders

Entity-Subsidiary relationship

Fax Messages

Fax Template

Fulfill Orders

Generate Price Lists

Generate Statements

Installment Payment Links

Inventory

Item Fulfillment

Items

KPI Scorecards

Lead Snapshot/Reminders

Letter Messages

Letter Template

Locations

Marketing Campaign Reports

Other Custom Fields

Pricing Records

Purchase Order

Quantity pricing Schedules

Quota Reports

Refund Returns

Return Authorization Reports

Sales

Sales By Partner

Sales By Promotion

Sales Force Automation

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Schedule Mass Updates

Statement Charge

Support

Support Case Snapshot/Reminders

Unbilled Receivable Registers

Update Prices

Vendors

View Payment Events

Work Calendar



 | 

Cash Sale

Cash Sale Refund

Customer Refund

Export Lists

Other Lists

Upsell Setup

Work Order



 | 

Campaign History

Commit Orders

Invoice

Override Payment Hold

PDF Messages

PDF Template

SuiteAnalytics Workbook



 | 

Address List in Search

Calendar

Case Alerts

Cases

Competitors

Contacts

Credit Memo

CRM Groups

CRM Lists

Customers

Documents and Files

Edit Forecast

Edit Manager Forecast

Establish Quotas

Estimate

Events

Find Transaction

Gift Certificate

Import CSV File

Internal Publisher

Invoice Approval

Lead Conversion

Lead Conversion Mapping

Mail Merge

Marketing Campaigns

Marketing Template

Mass Updates

Mobile Device Access

Notes Tab

Online Case Form

Online Custom Record Form

Online Customer Form

Opportunity

Partners

Perform Search

Phone Calls

Promotion

Publish Dashboards

Report Customization

Report Scheduling

Return Auth. Approval

Return Authorization

Sales Campaigns

Sales Force Automation Setup

Sales Order

Sales Order Approval

Sales Territory

Sales Territory Rule

SAML Single Sign-on

Set Up Image Resizing

Support Case Issue

Support Case Origin

Support Case Priority

Support Case Status

Support Case Territory

Support Case Territory Rule

Support Case Type

Support Setup

Tasks

Track Messages

Upsell Assistant

Upsell Wizard



 |

## Specialized User: Manufacturing Operator {#subsect_0302012022}

| Specialized User: Manufacturing Operator |
| --- |
| **View** | **Edit** | **Full** |
| --- | --- | --- |
| 
Bill Of Materials

Bill Of Materials Inquiry

Bins

CRM Groups

Custom Entity Fields

Employee Record

Entity-Subsidiary Relationship

Inventory Status

Item Process Family

Item Process Group

Locations

Manage Accounting Periods

Manufacturing Routing

Notes Tab

Perform Search

Subsidiaries

SuiteScript

Tasks

Units



 | 

Documents and Files

Items

Work Order



 | 

Build Assemblies

Build Work Orders

Custom Item Fields

Custom Item Number Fields

Custom Lists

Custom Record Entries

Custom Record Types

Custom Sublists

Custom Transaction Fields

Custom Transaction Forms

Find Transaction

SAML Single Sign-On

SuiteScript Scheduling

Work Order Completion

Work Order Issue



 |

## Specialized User: Project Manager {#subsect_0709095451}

| Specialized User: Project Manager |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Account Detail

Accounts

Accounts Payable

Accounts Payable Graphing

Accounts Receivable

Accounts Receivable Graphing

Accounts Receivable Register

Accounts Receivable Un-Billed

Bill Purchase Orders

Bills

Bulk Processing Submissions

Calculate Time

Classes

Contact Roles

Contact-Subsidiary relationship

Currency

Custom Record Entries

Custom Record Types

Customer Payment

Customer Profile

Customers

Departments

Employee Reminders

Enter Vendor Credits

Entity-Subsidiary relationship

Expense Categories

Expenses

Imported Employee Expenses

Installment Payment Links

Inventory

Invoice

Items

Locations

Make Journal Entry

Non Posting Registers

Opportunity

Pay Bills

PDF Messages

Project Profitability

Purchase Order Reports

Purchases

Resource Allocation Reports

Revenue Arrangement

Revenue Element

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

Sales

Sales Force Automation

Sales Order Reports

Sales Order Transaction Report

Subsidiaries

Time Tracking

Timer

Unbilled Receivable Registers



 | 

Contacts

Credit Memo

Estimate

Export Lists

Notes Tab



 | 

Accounting Lists

Billing Schedules

Employee Record

Employees

Financial History

Find Transaction

Fulfill Orders

Item Fulfillment

Other Lists

Project Revenue Rules

Purchase Orders

Receive Order

Report Customization

Sales Order

SuiteAnalytics Workbook

Time-Off

Track Messages

Vendors

Work Calendar



 | 

Address List in Search

Bulk Manage Roles

Bulk Time Entry Modification

Calendar

Charge

Charge - Run Rules

Charge Rule

Copy Project Tasks

Create Jobs from Sales Transactions

Custom Segments

Documents and Files

Events

Expense Report

Expense Report Policies

Generic Resources

Import CSV File

Jobs

Mobile Device Access

Perform Search

Phone Calls

Project / Project Template Conversion

Project Budget

Project Profitability Setup

Project Tasks

Project Templates

Publish Dashboards

Report Scheduling

Resource

Resource Allocation Approval

Resource Allocations

Resource Groups

Sales Order Approval

SuiteScript Scheduling

Tasks

Track Time

Vendor Bill Approval

Work Breakdown Structure



 |

## Specialized User: Site Operator {#subsect_0731010940}

| Specialized User: Site Operator |
| --- |
| **View** | **Create** | **Edit** | **Full** |
| --- | --- | --- | --- |
| 
Accounts Payable

Accounts Payable Graphing

Accounts Payable Register

Accounts Receivable

Accounts Receivable Graphing

Accounts Receivable Register

Accounts Receivable Un-Billed

Adjust Inventory

Adjust Inventory Worksheet

Balance Sheet

Bill of Materials

Bill of Materials Inquiry

Bill Purchase Orders

Bills

Bin Putaway Worksheet

Bin Transfer

Bins

Blanket Purchase Order

Blanket Purchase Order Approval

Budget

Bulk Processing Submissions

Calendar

Campaign History

Cash Flow Statement

Cash Sale

Cash Sale Refund

Check

Check Item Availability

Classes

Component Where Used

Contacts

Copy Budgets

Cost of Goods Sold Registers

Credit Card Charge

Credit Card Refund

Credit Memo

Credit Returns

CRM Groups

Custom Record Entries

Customer Deposit

Customer Payment

Customer Refund

Customers

Departments

Deposit

Deposit Application

Distribute Inventory

Duplicate Entry Management

Employee Reminders

Enter Vendor Credits

Estimate

Events

Expense Categories

Expense Registers

Fulfill Orders

Gift Certificate

Income

Income Statement



 | 

Installment Payment Links

Inventory

Inventory Status

Inventory Status Change

Invoice

Invoice Approval

Issue Reports

Issues

Item Fulfillment

Item Receipt

Item Revisions

Items

Jobs

Knowledge Base

Kudos

Lead Conversion

Make Journal Entry

Media Folders

Non Posting Registers

Notes Tab

Opportunity

Order Management Dashboard

Organizational Value

Other Names

Perform Search

Promotion

Publish Search

Purchase Order

Purchase Order Reports

Purchases

Receive Order

Receive Returns

Record Custom Field

Report Customization

Requisition

Requisition Approval

Return Auth. Approval

Return Authorization

Sales

Sales Order

Sales Order Approval

Schedule Mass Updates

Sent Email

Set Up Budgets

Shipping Items

Statistical Account Registers

SuiteScript

Support

Support Case Snapshot/Reminders

Tax Reports

Termination Reasons

Time Tracking

Time-Off Administration

Track Messages

Track Time

Unbuild Assemblies

Undelivered Emails

Units

Vendor Prepayment

Vendor Prepayment Application

Vendor Return Auth. Approval

Vendor Return Authorization

Vendor Returns

Vendors

Work Order



 | 

Bills

Export Lists

Persist Search

Phone Calls

Tasks



 | 

Cases

Count Inventory

Create Inventory Counts

Documents and Files

Enter Vendor Credits

Item Receipt

Item Fulfillment

Perform Search

Purchase Order

Scanned Vendor Bills

Shortcuts

SuiteAnalytics Workbook

Tax Details Tab

Time-Off

Transfer Inventory

Transfer Order

Transfer Order Approval

Vendors

Vendor Return Authorization



 | 

Address List in Search

Control SuiteScript and Workflow Triggers in Web Services Request

Control SuiteScript and Workflow Triggers per CSV Import

Custom Centers

Duplicate Case Management

Find Transaction

Import CSV File

Mobile Device Access

Publish Dashboards

Report Scheduling

SAML Single Sign-on

SuiteScript Scheduling



 |

## Specialized User: View and Approve {#subsect_0709101525}

| Specialized User: View and Approve |
| --- |
| **View** | Edit | Full |
| --- | --- | --- |
| 
Access Payment Audit Log

Access to transaction numbering audit log

Account Detail

Accounting Lists

Accounts

Accounts Payable

Accounts Payable Graphing

Accounts Receivable

Accounts Receivable Graphing

Accounts Receivable Un-Billed

Address List in Search

Adjust Inventory

Adjust Inventory Worksheet

Advanced PDF/HTML Templates

Allocation Schedules

Amortization Reports

Amortization Schedules

Audit Trail

Automated Cash Application

Balance Sheet

Balancing Journals

Bill Inbound Shipment

Bill Of Distribution

Bill of Materials

Bill Of Materials Inquiry

Bill Purchase Orders

Billing Schedules

Bills

Bin Putaway Worksheet

Bin Transfer

Bins

Blanket Purchase Order

Budget

Build Assemblies

Build Work Orders

Calculate Time

Calendar

Campaign History

Case Alerts

Cases

Cash Flow Statement

Cash Sale

Cash Sale Refund

Charge

Charge - Run Rules

Charge Rule

Check

Check Item Availability

Classes

Color Themes

Commission Reports

Commit Orders

Companies

Competitors

Component Where Used

Contact Roles

Contacts

Cost of Goods Sold Registers

Costed Bill Of Materials Inquiry

Count Inventory

Create Allocation Schedules

Create Inventory Counts

Credit Card Charge

Credit Card Refund

Credit Memo

Credit Returns

CRM Groups

CRM Lists

Cross Charge Request

Currency

Currency Adjustment Journal

Currency Revaluation

Custom Address Form

Custom Body Fields

Custom Center Categories

Custom Center Link

Custom Center Links

Custom Center Tabs

Custom Centers

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom HTML Layouts

Custom Item Fields

Custom Item Number Fields

Custom Lists

Custom PDF Layouts

Custom Record Entries

Custom Record Types



 | 

Custom Segments

Custom Sublist

Custom Sublists

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Custom Transaction Types

Customer Deposit

Customer Payment

Customer Payment Authorization

Customer Profile

Customer Refund

Customer Segments Manager

Customer Status

Customers

Customize Field Level Help

Deferred Expense Reports

Deleted Records

Departments

Deposit

Deposit Application

Distribute Inventory

Distribution Network

Documents and Files

Earliest Availability

Edit Forecast

Edit Manager Forecast

Edit Profile

Employee Commission Transaction

Employee Reminders

Employees

Enter Completions

Enter Opening Balances

Enter Vendor Credits

Enter Year-To-Date Payroll Adjustments

Entity-Subsidiary relationship

Equity Registers

Establish Quotas

Estimate

Events

Expense Categories

Expense Report

Expenses

Fair Value Dimension

Fair Value Formula

Fair Value Price

Fax Messages

Fax Template

Finance Charge

Financial History

Financial Statements

Find Transaction

Fulfill Orders

Fulfillment Request

General Ledger

General Token

Generate Price Lists

Generate Statements

Gift Certificate

Global Inventory Relationship

Granting access to Reports

Inbound Shipment

Income

Income Statement

Individual Paycheck

Installment Payment Links

Integration

Intelligent Recommendations

Intercompany Adjustments

Inventory

Inventory Status

Inventory Status Change

Invoice

Invoice Sales Orders

Issue Components

Issue Reports

Issues

Item Collection

Item Demand Plan

Item Fulfillment

Item Process Family

Item Process Group

Item Receipt

Item Revenue Category

Item Revisions

Item Supply Plan

Item Templates

Item/Category Layouts

Items

Jobs

Knowledge Base

KPI Scorecards



 | 

Kudos

Labor Costing

Lead Conversion

Lead Snapshot/Reminders

Letter Messages

Letter Template

Locations

Make Journal Entry

Manufacturing Cost Template

Manufacturing Routing

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Marketing Campaign Reports

Marketing Campaigns

Marketing Template

Matching Rules for Online Banking

Material Requirements Planning

Media Folders

Memorized Transactions

Net Worth

Netting Settlement

News Items

Notes Tab

Online Case Form

Online Custom Record Form

Online Customer Form

Opportunity

Order Management Dashboard

Order Reservation

Organizational Value

Other Custom Fields

Other Names

Override Estimated Cost on Transactions

Override Payment Hold

Ownership Transfer

Partner Authorized Commission Reports

Partner Commission Reports

Partner Commission Transaction

Partners

Pay Bills

Pay Sales Tax

Pay Tax Liability

Paycheck Journal

Payment Instruments

Payment Methods

Payroll Liability Payments

PDF Messages

PDF Template

Perform Search

Period End Financial Statements

Period End Journals

Persist Search

Phone Calls

Pick Strategy

Pick Task

Planned Revenue

Planned Standard Cost

Positions

Post Time

Post Vendor Bill Variances

Posting Period on Transactions

Presentation Categories

Pricing Records

Print Shipment Documents

Process GST Refund

Process Payroll

Project Budget

Project Profitability

Project Revenue Rules

Project Tasks

Project Templates

Promotion

Public Template Categories

Publish Forms

Publish RSS Feeds

Publish Search

Purchase Contract

Purchase Order

Purchase Order Reports

Purchases

Quantity pricing Schedules

Quota Reports

Receive Order

Receive Returns

Recognition Treatment

Reconcile Reporting

Record Custom Field

Refund Returns

Related Items

Report Customization

Report Scheduling

Request For Quote

Requisition



 | 

Resource

Resource Allocation Approval

Resource Allocation Reports

Resource Allocations

Resource Groups

Return Authorization

Return Authorization Reports

Revenue Arrangement

Revenue Arrangement Approval

Revenue Commitment

Revenue Commitment Reversal

Revenue Contracts

Revenue Element

Revenue Management VSOE

Revenue Recognition Plan

Revenue Recognition Reports

Revenue Recognition Rule

Revenue Recognition Schedules

Sales

Sales By Partner

Sales By Promotion

Sales Campaigns

Sales Force Automation

Sales Order

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Sales Roles

Scanned Vendor Bills

Schedule Mass Updates

Sent Email

Shipping Items

Shortcuts

Standard Cost Version

Statement Charge

Statistical Account Registers

Store Categories

Store Content Categories

Store Content Items

Store Pickup Fulfillment

Store Tabs

Subscription Change Orders

Subscription Plan

Subscriptions

Subsidiaries

SuiteAnalytics Workbook

Supply Chain Snapshot List

Support

Support Case Snapshot/Reminders

Tasks

Tax

Tax Details Tab

Tax Records

Tax Reports

Tax Schedules

Tegata Payable

Tegata Receivable

Template Categories

Time Codes

Time Tracking

Time-Off Administration

Timer

Track Messages

Track Time

Transaction Detail

Transaction Receive Inbound Shipment

Transfer Funds

Transfer Inventory

Transfer Order

Trial Balance

Unbuild Assemblies

Units

Vendor Prepayment

Vendor Prepayment Application

Vendor Request For Quote

Vendor Return Authorization

Vendor Returns

Vendors

View Gateway Asynchronous Notifications

Wave

Web Site Report

Web Store Report

Work Breakdown Structure

Work Calendar

Work Order

Work Order Close

Work Order Completion

Work Order Issue

Workflow



 | 

Time-Off



 | 

Blanket Purchase Order Approval

Employee Commission Transaction Approval

Invoice Approval

Journal Approval

Mobile Device Access

Partner Commission Transaction Approval

Purchase Contract Approval

Requisition Approval

Return Auth. Approval

Sales Order Approval

SAML Single Sign-on

Transfer Order Approval

Vendor Bill Approval

Vendor Payment Approval

Vendor Return Auth. Approval



 |

## Specialized User: WMS {#subsect_0425063323}

| Specialized User: WMS |
| --- |
| **View** | **Create** | Edit | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bulk Processing Submissions

Cash Sale

Currency

Departments

Entity-Subsidiary relationship

Expense Report

Fiscal Calendars

Installment Payment Links

Inventory

Invoice

Manage Accounting Periods

Notes Tab

Pay Sales Tax

Pricing Records

Sales Order Fulfillment Reports

Sales Order Transaction Report

Set Up Company

Subsidiaries

Tax Schedules



 | 

Export Lists



 | 

SuiteAnalytics Workbook

Time-Off



 | 

Accounting Lists

Accounting Preferences

Accounts

Address List in Search

Adjust Inventory

Allow JS / HTML Uploads

Audit Trail

Bin Transfer

Bins

Build Assemblies

Build Work Orders

Bulk Manage Roles

Classes

Companies

Contacts

Count Inventory

Create HTML Formulas in Search

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Lists

Custom Record Entries

Custom Record Types

Custom Transaction Fields

Custom Transaction Forms

Customer Profile

Customers

Distribute Inventory

Documents and Files

Employee Record

Employees

Find Transaction

Fulfill Orders

Generate Statements

Gift Certificate

Import CSV File

Inbound Shipment

Inventory Status

Inventory Status Change

Item Fulfillment

Item Process Family

Item Process Group

Item Receipt

Item/Category Layouts

Items

Locations

Perform Search

Pick Strategy

Pick Task

Publish Dashboards

Publish Forms

Publish Search

Purchase Order

Receive Order

Receive Returns

Record Custom Field

Report Customization

Return Authorization

Sales Force Automation Setup

Sales Order

SAML Single Sign-on

Schedule Mass Updates

Shipping Items

Shipping Partner Package

SuiteScript

SuiteScript Scheduling

Tasks

Track Time

Transfer Inventory

Transfer Order

Transfer Order Approval

Units

Vendor Return Authorization

Vendor Returns

Vendors

Vicarious emails

Wave

Work Order

Zone



 |

## Store Manager {#subsect_0425062942}

| Store Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Accounts Receivable

Bill Of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Inventory

Lead Snapshot/Reminders

Non Posting Registers

Price Books

Price Plans

Pricing Records

Project Templates

Purchase Order Reports

Resource Allocations

Sales

Sales By Partner

Sales By Promotion

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Subscription Plan

Usage

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Web Store Report

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Companies

Competitors

Custom Item Fields

Custom Lists

Customers

Email Template

Notes Tab

Override Payment Hold

Projects

Shipping Items

Shipping Partner Registration

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook

Time-Off

Track Messages

Vendors



 | 

Address List in Search

Allow JS / HTML Uploads

Bill of Materials

Calendar

Cash Sale

Cash Sale Refund

Color Themes

Commerce Categories

Contacts

CRM Groups

CRM Lists

Customer Segments Manager

Deleted Records

Documents and Files

Duplicate Entity Management

Events

Find Transaction

Gift Certificate

Intelligent Recommendations

Internal Publisher

Item Collection

Item Demand Plan

Item Supply Plan

Item/Category Layouts

Items

Log in using Access Tokens

Material Requirements Planning

Mobile Device Access

Notifications

Online Customer Form

Perform Search

Phone Calls

Presentation Categories

Product Analytics Records



 | 

Project Tasks

Publish Forms

Publish RSS Feeds

Purchase Order

Related Items

Report Customization

Report Scheduling

Requisition

Resource Allocation Approval

REST Web Services

Sales Order

Sales Order Approval

Set Up Domains

Set Up Image Resizing

Set Up Web Site

Site Search

SOAP Web Services

Store Content Items

Store Tabs

System Email Template

Tasks

Template Categories

Transfer Order

Transfer Order Approval

Uncategorized Presentation Items

Units

Upsell Assistant

Upsell Setup

Upsell Wizard

Website (External) publisher

Web Site Management



 |

## Support Administrator {#subsect_0425063008}

| Support Administrator |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bill Of Materials Inquiry

Bulk Processing Submissions

Contact-Subsidiary relationship

Employee Public

Employee Reminders

Entity-Subsidiary relationship

Financial History

Lead Snapshot/Reminders

Memorized Transactions

Price Books

Price Plans

Pricing Records

Project Templates

Promotion

Quota Reports

Resource Allocations

Return Authorization Reports

Sales Force Automation

Subscription Plan

Usage

Vendors

View Gateway Asynchronous Notifications

View Payment Events

Web Site Report

Work Calendar



 | 

Export Lists

Kudos

Receive Returns

Refund Returns

Return Auth. Approval

Return Authorization

Tableau® Workbook Export



 | 

Bill of Materials

Classes

Color Themes

Departments

Email Template

Items

Locations

Marketing Template

SuiteAnalytics Workbook

Time-Off

Track Messages

Units



 | 

Address List in Search

Admindocs

Audit Trail

Backup Your Data

Bulk Manage Roles

Calculate Time

Calendar

Case Alerts

Cases

Companies

Competitors

Contact Roles

Contacts

Create Public Search

CRM Groups

CRM Lists

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Item Fields

Custom Lists

Custom PDF Layouts

Custom Record Entries

Custom Record Types

Custom Subtabs

Custom Transaction Fields

Custom Transaction Forms

Customer Profile

Customers



 | 

Delete Event

Deleted Records

Documents and Files

Duplicate Entity Management

Employee Record

Employees

Escalation Assignment

Escalation Assignment Rule

Events

Fax Messages

Fax Template

Find Transaction

Import CSV File

Internal Publisher

Knowledge Base

KPI Scoreboards

Letter Messages

Letter Template

Log in using Access Tokens

Mail Merge

Manage Users

Mass Updates

Mobile Device Access

Notes Tab

Notifications

Online Case Form

Other Names

Partners

PDF Messages

PDF Template

Perform Search

Phone Calls

Product Analytics Records

Projects

Project Profitability

Project Tasks

Publish Dashboards

Publish Knowledge Base



 | 

Publish Search

Record Custom Field

Report Customization

Report Scheduling

Resource

Resource Allocation Approval

REST Web Services

Shortcuts

SOAP Web Services

Subscriptions

Subscription Change Orders

Support

Support Case Issue

Support Case Origin

Support Case Priority

Support Case Snapshot/Reminders

Support Case Status

Support Case Territory

Support Case Territory Rule

Support Case Type

Support Setup

System Email Template

Tasks

Telephony Integration

Template Categories

Time Tracking

Timer

Track Time

Two-Factor Authentication base

Users & Passwords



 |

## Support Manager {#subsect_0425063031}

| Support Manager |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Contact-Subsidiary relationship

CRM Lists

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Items

Lead Snapshot/Reminders

Price Books

Price Plans

Pricing Record

Project Templates

Resource Allocations

Sales

Sales By Partner

Sales By Promotion

Sales Order Reports

Subscription Plan

Support

Support Case Snapshot/Reminders

Units

Usage

Work Calendar



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Competitors

Customers

Email Template

Fax Messages

Fax Template

Issues

Letter Messages

Letter Template

Mail Merge

Mass Updates

PDF Messages

PDF Template

Projects

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Case Alerts

Cases

Companies

Contact Roles

Contacts

CRM Groups

Deleted Records

Documents and Files

Duplicate Entity Management

Escalation Assignment

Escalation Assignment Rule

Events

Find Transaction

Internal Publisher

Knowledge Base

Log in using Access Tokens

Mobile Device Access

Notes Tab

Notifications



 | 

Online Case Form

Perform Search

Phone Calls

Product Analytics Records

Project Tasks

Publish Knowledge Base

Report Customization

Report Scheduling

Resource Allocation Approval

REST Web Services

SOAP Web Services

Support Case Issue

Support Case Origin

Support Case Priority

Support Case Status

Support Case Territory

Support Case Territory Rule

Support Case Type

Support Setup

System Email Template

Tasks

Template Categories

Track Time



 |

## Support Person {#subsect_0425063056}

| Support Person |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Contact-Subsidiary relationship

CRM Lists

Duplicate Entity Management

Employee Public

Employee Record

Entity-Subsidiary relationship

Items

Lead Snapshot/Reminders

Price Books

Price Plans

Pricing Records

Project Templates

Publish Knowledge Base

Publish RSS Feeds

Resource Allocations

Subscription Plan

Support

Support Case Snapshot/Reminders

Units

Usage

Website (External) publisher

Work Calendar



 | 

Export Lists

Knowledge Base

Kudos

Notes Tab

Resource

Tableau® Workbook Export



 | 

Companies

Competitors

Customers

Email Template

Fax Messages

Fax Template

Issues

Letter Messages

Letter Template

Mail Merge

Mass Updates

PDF Messages

PDF Template

Projects

Subscriptions

Subscription Change Orders

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Calendar

Cases

Contacts

Deleted Records

Documents and Files

Events

Find Transaction

Log in using Access Tokens

Mobile Device Access

Notifications

Perform Search

Phone Calls

Product Analytics Records

Project Tasks

Report Customization

Report Scheduling

Resource Allocation Approval

REST Web Services

SOAP Web Services

Tasks

Template Categories

Track Time



 |

## System Administrator {#subsect_0425063121}

| System Administrator |
| --- |
| **View** | Create | **Edit** | Full |
| --- | --- | --- | --- |
| 
Bulk Processing Submissions

Employee Public

Employee Reminders

Find Transaction

Notes Tab

SaaS Metric

Sent Email

System Status

Undelivered Emails



 | 

Kudos



 | 

Email Template

Override Payment Hold

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Admindocs

Analytical Impact

Auto-Generated Numbers

Billing Information

Bulk Manage Roles

Classes

Credit Card Processing

Custom Body Fields

Custom Column Fields

Custom Entity Fields

Custom Entry Forms

Custom Event Fields

Custom Fields

Custom Item Fields

Custom Lists

Custom PDF Layouts

Custom Record Types

Custom Sublist

Custom Subtabs

Custom Transaction Fields



 | 

Custom Transaction Forms

Customer Segments Manager

Deleted Records

Departments

Duplicate Detection Setup

Employee Record

Employee Social Security Numbers

Employees

Enable Features

Events

Financial Institution Records

Internal Publisher

Item Collection

KPI Scorecards

Locations

Log in using Access Tokens

Manage Custom Permissions

Manage Custom Restrictions

Manage Users

Notifications

Price Books

Price Plans

Product Analytics Records

Publish Dashboards

Publish Search

REST Web Services

Set Up Company

SOAP Web Services

Subscription Change Orders

Subscription Plan

Subscriptions

Tasks

Template Categories

Two-Factor Authentication base

Usage

Web Services



 |

## Tax Engine {#subsect_0425063146}

| Tax Engine |
| --- |
| **View** | **Create** | **Edit** | Full |
| --- | --- | --- | --- |
| 
Accounts

Auto-Generated Numbers

Bills

Bulk Processing Submissions

Cash Sale

Cash Sale Refund

Companies

Credit Card Charge

Credit Card Refund

Credit Memo

Credit Returns

Currency

Customer Deposit

Customer Payment

Customer Refund

Customers

Deposit

Deposit Application

Enter Vendor Credits

Entity-Subsidiary relationship

Expense Categories

Expense Report

Finance Charge

Find Transaction

Gift Certificate

Installment Payment Links

Imported Employee Expenses

Invoice

Item Fulfillment

Item Receipt

Items

Make Journal Entry

Opportunity

Other Names

Perform Search

Posting Period on Transactions

Pricing Records

Projects

Promotion

Purchase Order

Quote

Return Authorization

Sales Order

Set Up Company

Shipping Items

Subsidiaries

Subsidiary Tax Registrations Tab

Tax Details Tab

Vendor Return Authorization

Vendors



 | \- | \- | 

Address List in Search

Product Analytics Records

Tax Records



 |

## Vendor Center {#subsect_0425063211}

| Vendor Center |
| --- |
| **View** | **Create** | Edit | Full |
| --- | --- | --- | --- |
| 
Accounts Payable Register

Find Transaction

Non Posting Registers

Notes Tab

Purchase Order

Requisition

Sales Order Transaction Report



 | \- | \- | 

Deleted Records

Log in using Access Tokens

Notifications

REST Web Services

SOAP Web Services

Track Time

Vendor Request For Quote



 |

## Warehouse Manager {#subsect_0425063246}

| Warehouse Manager |
| --- |
| **View** | **Create** | Edit | Full |
| --- | --- | --- | --- |
| 
Access Payment Audit Log

Bill Of Materials Inquiry

Bill of Materials

Bulk Processing Submissions

Check Item Availability

Commit Orders

Component Where Used

Contact-Subsidiary relationship

Costed Bill Of Materials Inquiry

Customers

Employee Compensation

Employee Confidential

Employee Public

Employee Record

Entity-Subsidiary relationship

Gift Certificate

Inventory

Item Revisions

Non Posting Registers

Notes Tab

Purchase Order Reports

Price Books

Pricing Records

Price Plans

Revalue Inventory Cost

Sales Order

Sales Order Fulfillment Reports

Sales Order Reports

Sales Order Transaction Report

Subscription Plan

Units

Vendors

View Gateway Asynchronous Notifications

View Payment Events



 | 

Export Lists

Kudos

Resource

Tableau® Workbook Export



 | 

Bills

Email Template

Items

Shipping Items

Shipping Partner Registration

SuiteAnalytics Workbook

Time-Off

Track Messages



 | 

Address List in Search

Adjust Inventory

Allocate Orders

Approve Order Reservation

Bill Of Distribution

Build Work Orders

Calendar

Close Work Orders

Contacts

Count Inventory

Create Inventory Counts

Deleted Records

Distribution Network

Documents and Files

Enter Completions

Events

Find Transaction

Fulfill Orders

Global Inventory Relationship

Inbound Shipment

Inventory Cost Template

Issue Components

Item Demand Plan

Item Fulfillment

Item Process Family

Item Process Group

Item Receipt

Item Supply Plan

Licence Plate

Log in using Access Tokens

Manufacturing Cost Template

Manufacturing Routing

Mark Work Orders Built

Mark Work Orders Firmed

Mark Work Orders Released

Material Requirements Planning

Mobile Device Access

Notifications

Order Allocation Strategy

Order Management Dashboard

Order Reservation

Ownership Transfer

Perform Search

Phone Calls

Pick Strategy

Pick Task

Planned Standard Cost

Print Shipment Documents

Product Analytics Records

Purchase Order

Reallocate Order Item

Receive Order

Receive Returns

Report Customization

Report Scheduling

Requisition

Requisition Approval

REST Web Services

Sales Channel

Shipping Partner Package

Shipping Partner Shipment

SOAP Web Services

Standard Cost Version

Supply Chain Snapshot List

Tasks

Template Categories

Transfer Order

Transfer Order Approval

Units for Pick Decomposition

Vendor Bill Approval

Wave

Work Order

Work Order Close

Work Order Completion

Work Order Issue

Zone



 |

### Related Topics

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [NetSuite Access Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285060.html)
-   [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html)
-   [Feature Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491844394.html)
-   [NetSuite Roles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285436.html)
-   [NetSuite Users Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N321756.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
