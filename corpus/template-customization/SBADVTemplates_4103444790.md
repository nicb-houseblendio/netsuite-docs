---
id: "SBADVTemplates_4103444790"
type: "SBADVTemplates"
title: "Standard Expense Report PDF/HTML Template"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Expense Report PDF/HTML Template"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_4103444790.html"
anchors: ["SBADVTemplates_2342661475", "SBADVTemplates_3484481521", "SBADVTemplates_949488763", "SBADVTemplates_2738172096", "SBADVTemplates_1025989715", "SBADVTemplates_741020264", "SBADVTemplates_3756193226"]
sha256: "26b43a96d7b36244ff03f86a8de1f1215df2d479219c7945515cfca393f8a1ff"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Expense Report PDF/HTML Template template are listed below.

## Record - record {#SBADVTemplates_2342661475}

The following fields are available for the Record record.

| Name | Type | ID |
| --- | --- | --- |
| Account | select | account |
| Account for Corporate Card Expenses | select | acctcorpcardexp |
| Accounting Approval | checkbox | accountingapproval |
| Advance to Apply | currency | advance |
| Advance to Apply | currency | advance2 |
| Advance to Apply Account | select | advanceaccount |
| Class | select | class |
| Complete | checkbox | complete |
| Corporate Card | currency | corporatecard |
| Corporate Card By Default | checkbox | corpcardbydefault |
| Custom Form | select | customform |
| Date | date | trandate |
| Date Due | date | duedate |
| Department | select | department |
| Employee | select | entity |
| Exclude from GL Audit Numbering | checkbox | excludefromglnumbering |
| Exp. Rept. # | text | tranid |
| Expenses Total | currency | total |
| ExternalId | text | externalid |
| From | date | fromdate |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Internal ID | text | id |
| Location | select | location |
| Nexus | select | nexus |
| Non-reimbursable Expenses (Tax Excl.) | currency | nonreimbursable |
| Posting Period | select | postingperiod |
| Purpose | text | memo |
| Reimbursable Expenses | currency | reimbursable |
| Stored tax reference for update | text | taxreferencetobeupdated |
| Subsidiary | select | subsidiary |
| Supervisor Approval | checkbox | supervisorapproval |
| Tax Details Override | checkbox | taxdetailsoverride |
| Tax Reg. Number | select | subsidiarytaxregnum |
| Tax Registration Override | checkbox | taxregoverride |
| Tax Strategy Used | text | taxstrategyused |
| Tax Total | currency | taxtotal |
| Taxes Dirty | checkbox | taxesdirty |
| To | date | todate |
| Total Reimbursable Amount | currency | amount |
| Transaction Number | text | transactionnumber |
| Use Multicurrency | checkbox | usemulticurrency |

### Sublists {#SBADVTemplates_3484481521}

The following sublists are available for the Record record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **accountingbookdetail** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Base Currency | select | currency |
    | Exchange Rate | currency2 | exchangerate |
    | Secondary Book | select | accountingbook |
    
-   The **calls** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Date | date | startdate |
    | Organizer | select | assigned |
    | Phone Number | phone | phone |
    | Subject | text | title |
    
-   The **events** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | All Day | checkbox | alldayevent |
    | Date | date | startdate |
    | End Time | timeofday | endtime |
    | Location | text | location |
    | Start Time | timeofday | starttime |
    | Title | text | title |
    
-   The **expense** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Expense Item | integer | expenseitem |
    | Expense-Based Rules | integer | numrules |
    | Gross Amount | currency | grossamt |
    | Tax Amount | currency | taxamount |
    | Tax Details Reference | text | taxdetailsreference |
    
-   The **mediaitem** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Attach File | select | mediaitem |
    | File Type | text | filetype |
    | Folder | text | folder |
    | Last Modified | datetime | lastmodifieddate |
    | Size (kB) | float | filesize |
    
-   The **tasks** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Due Date | date | duedate |
    | Priority | select | priority |
    | Start Date | date | startdate |
    | Title | text | title |
    
-   The **taxdetails** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Details | textarea | calcdetail |
    | Gross Amount | currency | grossamount |
    | Line Number | posinteger | linenumber |
    | Line type | text | linetype |
    | Name | text | linename |
    | Net Amount | currency | netamount |
    | Tax Amount | currency | taxamount |
    | Tax Basis | currency | taxbasis |
    | Tax Code | select | taxcode |
    | Tax Details Reference | text | taxdetailsreference |
    | Tax Rate | percent | taxrate |
    | Tax Type | select | taxtype |
    
-   The **usernotes** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Date | date | notedate |
    | Direction | select | direction |
    | Memo | textarea | note |
    | Time | timeofday | time |
    | Title | text | title |
    | Type | select | notetype |
    

## Company Information - companyinformation {#SBADVTemplates_949488763}

The following fields are available for the Company Information record.

| Name | Type | ID |
| --- | --- | --- |
| Account ID | text | companyid |
| Account ID | text | prevparent |
| Address | text | addresstext |
| Address | text | mainaddress\_text |
| Allowed IP Addresses | text | ipaddressrules |
| Always Display Subsidiary Name | checkbox | showsubsidiaryname |
| Company Logo (Forms) | text | formlogo |
| Company Logo (Pages) | text | pagelogo |
| Company Name | text | companyname |
| Country | text | country |
| County/State/Province | text | dropdownstate |
| County/State/Province | text | state |
| Currency | text | basecurrency |
| Customer Center Login | text | customersurl |
| Display Logo Internally | checkbox | displaylogointernally |
| Document Number Prefix | text | tranprefix |
| Edition | text | edition |
| Elimination | checkbox | iselimination |
| Email Address | text | adminemail |
| External Forms | text | formsurl |
| ExternalId | text | externalid |
| Fax | text | fax |
| First Fiscal Month | text | fiscalmonth |
| Fiscal Calendar | text | fiscalcalendar |
| Intercompany Account | text | intercoaccount |
| Internal ID | text | id |
| Legal Name | text | legalname |
| Name | text | name |
| NetSuite UI | text | appurl |
| Rest (RESTlets) | text | restleturl |
| Return Address | text | returnaddress\_text |
| Return Email Address | text | email |
| Shipping Address | text | shippingaddress\_text |
| Subsidiary is Inactive | checkbox | isinactive |
| Subsubsidiary of | text | parent |
| SuiteAnalytics Connect (ODBC) | text | odbcurl |
| SuiteTalk (web services) | text | suitetalkurl |
| Tax Fiscal Calendar | text | taxfiscalcalendar |
| Time Zone | text | timezone |
| Web Site | text | url |

## Subsidiary - subsidiary {#SBADVTemplates_2738172096}

The following fields are available for the Subsidiary record.

| Name | Type | ID |
| --- | --- | --- |
| Account ID | select | prevparent |
| Address | address | mainaddress\_text |
| Allow Customer Override | checkbox | issuecustomernotificationoverride |
| Always Display Subsidiary Name | checkbox | showsubsidiaryname |
| Balance Sheet Closing Account | select | bsclosingacct |
| Balance Sheet Opening Account | select | bsopeningacct |
| CSV column delimiter | select | CSV\_COLUMN\_DELIMITER |
| CSV decimal delimiter | select | CSV\_DECIMAL\_DELIMITER |
| Calendar System | select | CALENDARSYSTEM |
| Check Default Chart Type | select | checklayout |
| Country | select | country |
| Create Balance Sheet Closing and Opening Journals | checkbox | enablebscloseandopen |
| Create Income Summary Journals | checkbox | enableincomesummarystep |
| Create Period End Journals By Segment | checkbox | createpejebysegment |
| Currency | text | currency |
| Customer Center Email Template | select | CUSTCENTEREMAILTEMPLATE |
| Customer Template | select | issuecustomertemplate |
| Date Format | select | DATEFORMAT |
| Default Account for Corporate Card Expenses | select | DEFAULTACCTCORPCARDEXP |
| Default Advance to Apply Account for Expense Reports | select | DEFAULT\_ADVANCE\_ACCT\_FOR\_EXPREPT |
| Default Case Profile | select | defaultcaseprofile |
| Default Check Type | select | CHECKTYPE |
| Default Payable Account for Expense Reports | select | DEFAULTAPACCOUNTFOREXPREPT |
| Document Number Prefix | text | tranprefix |
| Edition | text | edition |
| Elimination | checkbox | iselimination |
| Employee Template | select | issueemployeetemplate |
| Enable Period End Journal Entries | checkbox | enableperiodendjournals |
| ExternalId | text | externalid |
| Fax | text | fax |
| First Day of Week | select | FIRSTDAYOFWEEK |
| Fiscal Calendar | select | fiscalcalendar |
| GL Impact Locking | checkbox | glimpactlocking |
| Income Summary Loss Account | select | islossacct |
| Income Summary Profit Account | select | isprofitacct |
| Intercompany Account | select | intercoaccount |
| Internal ID | text | id |
| Language | select | languagelocale |
| Legal Name | text | legalname |
| Long Date Format | select | LONGDATEFORMAT |
| Name | text | name |
| Negative Number Format | select | NEGATIVE\_NUMBER\_FORMAT |
| Number Format | select | NUMBERFORMAT |
| Partner Center Email Template | select | PARTCENTEREMAILTEMPLATE |
| Phone Number Format | select | PHONEFORMAT |
| Require Memo on Period End Journals | checkbox | requirepejememo |
| Return Address | address | returnaddress\_text |
| Return Email Address | email | email |
| Round Time Entry Duration | select | roundtime |
| Search Sorting | select | SEARCHSORTING |
| Send Customer Notifications When | select | issuecustomernotification |
| Shipping Address | address | shippingaddress\_text |
| Spelling Locale | select | SPELL\_LOCALE |
| State/Province | select | dropdownstate |
| State/Province | text | state |
| Subsidiary Logo (Forms) | select | logo |
| Subsidiary Logo (Pages) | select | pagelogo |
| Subsidiary is Inactive | checkbox | isinactive |
| Subsubsidiary of | select | parent |
| Tax Fiscal Calendar | select | taxfiscalcalendar |
| Time Format | select | TIMEFORMAT |
| Time Zone | select | TIMEZONE |
| Use In-Transit Vendor Payments By Default | checkbox | DEFAULTVENDORPAYMENTTYPE |
| User Access Email Template | select | EMAILACCESSTEMPLATE |
| Vendor Bill - Item Receipt Amount Tolerance | posfloat | receiptamount |
| Vendor Bill - Item Receipt Quantity Difference | posfloat | receiptquantitydiff |
| Vendor Bill - Item Receipt Quantity Tolerance | posfloat | receiptquantity |
| Vendor Bill - Purchase Order Amount Tolerance | posfloat | purchaseorderamount |
| Vendor Bill - Purchase Order Quantity Difference | posfloat | purchaseorderquantitydiff |
| Vendor Bill - Purchase Order Quantity Tolerance | posfloat | purchaseorderquantity |
| Vendor In-Transit Payment Account | select | VENDORITPACCOUNT |
| Web Site | text | url |

### Sublists {#SBADVTemplates_1025989715}

The following sublists are available for the Subsidiary record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **accountingbookdetail** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Base Currency | select | currency |
    | Enable Period End Journal Entries | checkbox | enableperiodendjournals |
    | Secondary Book | select | accountingbook |
    | Status | select | bookstatusname |
    
-   The **classtranslation** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Language | text | language |
    | Name | text | name |
    
-   The **taxregistration** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Country | select | nexuscountry |
    | Effective From | date | effectivefrom |
    | Nexus | select | nexus |
    | Tax Agency | select | taxagency |
    | Tax Engine | select | taxengine |
    | Tax Reg. Number | text | taxregistrationnumber |
    | Valid Until | date | validuntil |
    

## User - user {#SBADVTemplates_741020264}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_3756193226}

The following fields are available for the Preference record.

| Name | Type | ID |
| --- | --- | --- |
| Bar Code | checkbox | print\_barcodes |
| Name for Case | text | naming\_case |
| Name for Customer | text | naming\_customer |
| Name for Lead | text | naming\_lead |
| Print Accounts on Vouchers | checkbox | voucheraccount |
| Print Business Number on Forms | checkbox | printfednum |
| Print Discount and Shipping Lines in Columns | checkbox | inlinediscountshipping |
| Print Remittance Form with {#Invoices#} & Statements | checkbox | remittanceform |
| Print Return Form with Packing Slip | checkbox | returnform |
| Print Separate Voucher for {#Bill#} {#Payments#} | checkbox | paymentvouchers |
| Print Transaction Forms Landscape | checkbox | formlandscape |
| Time Zone | text | timezone |
| Use Multiple Versions and Builds | checkbox | issue\_multiple\_versions |
| Use {#Location#} Address on Forms | checkbox | printlocaddress |
| {#Customers#} Default to Print Transactions | checkbox | customerprinttransactions |
| {#Vendors#} Default to Print Transactions | checkbox | vendorprinttransactions |

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
