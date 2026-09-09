---
id: "SBADVTemplates_284379731"
type: "SBADVTemplates"
title: "Standard Period End Journal PDF/HTML Template"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Period End Journal PDF/HTML Template"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_284379731.html"
anchors: ["SBADVTemplates_3347057084", "SBADVTemplates_2977511867", "SBADVTemplates_1408989517", "SBADVTemplates_983448744", "SBADVTemplates_4282019708", "SBADVTemplates_478049357", "SBADVTemplates_2618472364"]
sha256: "073e53bd2dd50d78d1b31b86167dbdc0dd3b97eef95cd77683db1123a75d69e8"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Period End Journal PDF/HTML Template template are listed below.

## Record - record {#SBADVTemplates_3347057084}

The following fields are available for the Record record.

| Name | Type | ID |
| --- | --- | --- |
| Accounting Book | select | accountingbook |
| Class | select | class |
| Credit | currency | credittotal |
| Currency | select | currency |
| Custom Form | select | customform |
| Date | date | trandate |
| Debit | currency | debittotal |
| Department | select | department |
| Entry No. | text | tranid |
| Exclude from GL Audit Numbering | checkbox | excludefromglnumbering |
| ExternalId | text | externalid |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Internal ID | text | id |
| Location | select | location |
| Main Account | select | mainaccount |
| Memo | text | memo |
| Posting Period | select | postingperiod |
| Source Subsidiary | select | sourcesubsidiary |
| Subsidiary | select | subsidiary |
| Transaction Number | text | transactionnumber |

### Sublists {#SBADVTemplates_2977511867}

The following sublists are available for the Record record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

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
    
-   The **line** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Account | select | account |
    | Credit | currency | credit |
    | Debit | currency | debit |
    | Memo | text | memo |
    
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
    
-   The **usernotes** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Date | date | notedate |
    | Direction | select | direction |
    | Memo | textarea | note |
    | Time | timeofday | time |
    | Title | text | title |
    | Type | select | notetype |
    

## Company Information - companyinformation {#SBADVTemplates_1408989517}

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

## Subsidiary - subsidiary {#SBADVTemplates_983448744}

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

### Sublists {#SBADVTemplates_4282019708}

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
    

## User - user {#SBADVTemplates_478049357}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_2618472364}

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
