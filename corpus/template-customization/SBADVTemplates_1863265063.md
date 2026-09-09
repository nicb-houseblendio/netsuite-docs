---
id: "SBADVTemplates_1863265063"
type: "SBADVTemplates"
title: "Standard Statement PDF/HTML Template"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Statement PDF/HTML Template"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_1863265063.html"
anchors: ["SBADVTemplates_3231750985", "SBADVTemplates_4100594221", "SBADVTemplates_3484769939", "SBADVTemplates_1419474764", "SBADVTemplates_630376133", "SBADVTemplates_2119239586", "SBADVTemplates_977526064", "SBADVTemplates_4176685101", "SBADVTemplates_2088997257"]
sha256: "18dc7759a941936aa90f861ef7dc4a9246b8be3b131c13b0586d676035739d0c"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Statement PDF/HTML Template template are listed below.

## Record - record {#SBADVTemplates_3231750985}

The following fields are available for the Record record.

| Name | Type | ID |
| --- | --- | --- |
| 1-30 Days | number | aging2 |
| 31-60 Days | number | aging3 |
| 61-90 Days | number | aging4 |
| Account Number | text | accountnumber |
| Amount Due | number | agingbal |
| Amount Due | number | amountdue |
| Billing Address | text | billaddress |
| Credit Limit | number | creditlimit |
| Currency | text | currency |
| Currency Symbol | text | currencysymbol |
| Current | number | aging1 |
| Over 90 Days | number | aging5 |
| Project | text | project |
| Sales Rep | text | salesrep |
| Subsidiary | text | subsidiary |
| Terms | text | terms |
| Transaction Date | date | trandate |

### Sublists {#SBADVTemplates_4100594221}

The following sublists are available for the Record record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **lines** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Balance | text | balance |
    | Charge | text | charge |
    | Date | text | datecol |
    | Description | text | description |
    | Due Date | text | duedate |
    | End Date | text | enddate |
    | GL # | text | glnumber |
    | GL Audit Numbering Sequence | text | glsequence |
    | Memo | text | memo |
    | Open Amount | text | amountremaining |
    | PO/Check # | text | otherrefnum |
    | Payment | text | payment |
    | Payment Method | text | paymentmethod |
    | Start Date | text | startdate |
    | Subcustomer/Job | text | subname |
    | Terms | text | terms |
    

## Customer - customer {#SBADVTemplates_3484769939}

The following fields are available for the Customer record.

| Name | Type | ID |
| --- | --- | --- |
| Account | text | accountnumber |
| Address | address | defaultaddress |
| Alcohol Recipient Type | select | alcoholrecipienttype |
| Alt. Email | email | altemail |
| Alt. Phone | phone | altphone |
| Assigned Web Site | select | assignedwebsite |
| Auto | checkbox | autoname |
| Billing Rate Card | select | billingratecard |
| Billing Schedule | select | billingschedule |
| Billing Transaction Form | select | billingtransactionform |
| Billing Transaction Type | select | billingtransactiontype |
| Budget Approved | checkbox | isbudgetapproved |
| Buying Reason | select | buyingreason |
| Buying Time Frame | select | buyingtimeframe |
| Campaign Category | select | campaigncategory |
| Campaign Event | select | campaignevent |
| Category | select | category |
| Choose Team | select | salesgroup |
| Comments | textarea | comments |
| Company Name | text | companyname |
| Confirm Password | password | password2 |
| Country | select | shipping\_country |
| Credit Limit | poscurrency | creditlimit |
| Currency Precision | text | currencyprecision |
| Custom Form | select | customform |
| Customer ID | text | entityid |
| Date Created | datetime | datecreated |
| Default Order Priority | float | defaultorderpriority |
| Default Receivables Account | select | receivablesaccount |
| Default Tax Reg. | select | defaulttaxreg |
| Deferred Revenue Account for Revenue Reclassification | select | draccount |
| Email | email | email |
| Email | checkbox | emailtransactions |
| Email Preference | select | emailpreference |
| End Date | date | enddate |
| Estimated Budget | currency | estimatedbudget |
| ExternalId | text | externalid |
| Fax | phone | fax |
| Fax | checkbox | faxtransactions |
| For new access provisioning consider sending a New Access Notification Email with a password setup URL instead of manually assigning a user password. | help | newaccesshelp |
| Foreign Currency Adjustment Revenue Account | select | fxaccount |
| Furigana | text | phoneticname |
| Give Access | checkbox | giveaccess |
| Global Subscription Status | select | globalsubscriptionstatus |
| Hold | select | creditholdoverride |
| Home Phone | phone | homephone |
| Image | select | image |
| Inactive | checkbox | isinactive |
| Individual | radio | isperson |
| Internal ID | text | id |
| Job Title | text | title |
| Language | select | language |
| Last Modified Date | datetime | lastmodifieddate |
| Lead Source | select | leadsource |
| Manually assign or change password | checkbox | fillpassword |
| Mobile Phone | phone | mobilephone |
| Monthly Closing Date | select | monthlyclosing |
| Mr./Ms... | text | salutation |
| Name | text | firstname |
| Negative Number Format | select | negativenumberformat |
| Number Format | select | numberformat |
| Opening Balance | currency | openingbalance |
| Opening Balance Account | select | openingbalanceaccount |
| Opening Balance Date | date | openingbalancedate |
| Parent Company | select | parent |
| Partner | select | partner |
| Password | password | password |
| Phone | phone | phone |
| Pref. CC Processor | select | prefccprocessor |
| Price Level | select | pricelevel |
| Primary Subsidiary | select | subsidiary |
| Print | checkbox | printtransactions |
| Print on Check As | text | printoncheckas |
| Reminder Days | posinteger | reminderdays |
| Represents Subsidiary | select | representingsubsidiary |
| Role | select | accessrole |
| Sales Readiness | select | salesreadiness |
| Sales Rep | integer | salesrep |
| Send New Access Notification Email | checkbox | sendemail |
| Send Transactions Via | label | sendtransactionsvia |
| Ship Complete | checkbox | shipcomplete |
| Shipping Carrier | select | shippingcarrier |
| Shipping Method | select | shippingitem |
| Source Web Site | select | sourcewebsite |
| Start Date | date | startdate |
| Status | select | entitystatus |
| Terms | select | terms |
| Territory | select | territory |
| Type | label | isindividual |
| Unsubscribe from Campaigns | select | unsubscribe |
| Update Transactions | checkbox | syncpartnerteams |
| Web Address | url | url |

### Sublists {#SBADVTemplates_1419474764}

The following sublists are available for the Customer record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **addressbook** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Address | address | addressbookaddress\_text |
    | Default Billing | checkbox | defaultbilling |
    | Default Shipping | checkbox | defaultshipping |
    | Label | text | label |
    | Residential Address | checkbox | isresidential |
    
-   The **calls** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Date | date | startdate |
    | Organizer | select | assigned |
    | Phone Number | phone | phone |
    | Subject | text | title |
    
-   The **contact** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Contact | text | entityid |
    | Email | email | email |
    | Job Title | text | title |
    | Main Phone | phone | phone |
    | Role | select | contactrole |
    | Subsidiary | select | subsidiary |
    
-   The **creditcards** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Card State | select | cardstate |
    | Cardholder Name | text | ccname |
    | Credit Card Number | ccnumber | ccnumber |
    | Credit Card Type | select | paymentmethod |
    | Customer Code | text | customercode |
    | Default Credit Card | checkbox | ccdefault |
    | Expiration Date | mmyydate | ccexpiredate |
    | Memo | text | ccmemo |
    | State From | datetime | statefrom |
    
-   The **currency** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Currency | select | currency |
    | Format Sample | text | formatsample |
    | Override Currency Format | checkbox | overridecurrencyformat |
    | Symbol | text | displaysymbol |
    | Symbol Placement | select | symbolplacement |
    
-   The **download** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Attach File | select | file |
    | Expiration Date | date | expiration |
    | License Code | textarea | licensecode |
    | Remaining Downloads | integer | remainingdownloads |
    
-   The **events** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | All Day | checkbox | alldayevent |
    | Date | date | startdate |
    | End Time | timeofday | endtime |
    | Location | text | location |
    | Start Time | timeofday | starttime |
    | Title | text | title |
    
-   The **grouppricing** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Price Level | select | level |
    | Pricing Group | select | group |
    
-   The **itempricing** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Currency | select | currency |
    | Item | select | item |
    | Price Level | select | level |
    | Unit Price | currency2 | price |
    
-   The **mediaitem** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Attach File | select | mediaitem |
    | File Type | text | filetype |
    | Folder | text | folder |
    | Last Modified | datetime | lastmodifieddate |
    | Size (kB) | float | filesize |
    
-   The **opportunities** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Budget Approved | checkbox | isbudgetapproved |
    | Buying Reason | select | buyingreason |
    | Buying Time Frame | select | buyingtimeframe |
    | Details | textarea | memo |
    | Estimated Budget | currency | estimatedbudget |
    | Expected Close | date | expectedclosedate |
    | Projected Total | currency | projectedtotal |
    | Sales Readiness | select | salesreadiness |
    | Status | select | entitystatus |
    | Title | text | title |
    
-   The **partners** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Contribution % | percent | contribution |
    | Partner | select | partner |
    | Partner Role | select | partnerrole |
    | Primary | checkbox | isprimary |
    
-   The **salesteam** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Contribution % | percent | contribution |
    | Employee | select | employee |
    | Primary | checkbox | isprimary |
    | Sales Role | select | salesrole |
    
-   The **submachine** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Balance | currency | balance |
    | Currency | text | balancecurrency |
    | Currency | text | depositbalancecurrency |
    | Currency | text | unbilledcurrency |
    | Deposit Balance | currency | depositbalance |
    | Entity | text | entity |
    | Inactive | text | issubinactive |
    | Primary | text | isprimesub |
    | Subsidiary | select | subsidiary |
    | Unbilled Orders | currency | unbilledorders |
    
-   The **subscriptionmsgmach** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Author | text | author\_name |
    | Date | datetime | sentDate |
    | Memo | text | memo |
    | Message Type | text | type |
    | Recipient | text | recipient\_name |
    | Recipient Email | text | email |
    | Sender | text | sender\_name |
    
-   The **subscriptions** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Subscribed | checkbox | subscribed |
    | Subscription | select | subscription |
    | Subscription | text | subscription\_display |
    
-   The **tasks** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Due Date | date | duedate |
    | Priority | select | priority |
    | Start Date | date | startdate |
    | Title | text | title |
    
-   The **taxregistration** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Address | select | address |
    | Country | select | nexuscountry |
    | Nexus | select | nexus |
    | State | select | nexusstate |
    | Tax Reg. Number | text | taxregistrationnumber |
    
-   The **usernotes** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Date | date | notedate |
    | Direction | select | direction |
    | Memo | textarea | note |
    | Time | timeofday | time |
    | Title | text | title |
    | Type | select | notetype |
    

## Company Information - companyinformation {#SBADVTemplates_630376133}

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

## Subsidiary - subsidiary {#SBADVTemplates_2119239586}

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

### Sublists {#SBADVTemplates_977526064}

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
    

## User - user {#SBADVTemplates_4176685101}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_2088997257}

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
