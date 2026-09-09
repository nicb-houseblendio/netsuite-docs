---
id: "SBADVTemplates_3377692491"
type: "SBADVTemplates"
title: "Standard Check PDF/HTML Template"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Check PDF/HTML Template"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_3377692491.html"
anchors: ["SBADVTemplates_4194814291", "SBADVTemplates_2211315234", "SBADVTemplates_137307251", "SBADVTemplates_2999470055"]
sha256: "85a39cb473551bc45c2f8ddecf4a4b6483ba895b42e3a4540dbaf18ad6813fc7"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Check PDF/HTML Template template are listed below.

## Check - check {#SBADVTemplates_4194814291}

The following fields are available for the Check record.

| Name | Type | ID |
| --- | --- | --- |
| Account | text | account |
| Address | text | address |
| Amount | number | total |
| Amount | number | usertotal |
| Available Balance | number | availablebalance |
| Balance | number | balance |
| Base Currency | checkbox | isbasecurrency |
| Check # | text | tranid |
| Check Number | text | checknumber |
| Class | text | class |
| Currency | text | currency |
| Currency | text | currencyname |
| Currency Symbol | text | currencysymbol |
| Custom Form | text | customform |
| Date | date | trandate |
| Department | text | department |
| Exchange Rate | number | exchangerate |
| Exclude from GL Audit Numbering | checkbox | excludefromglnumbering |
| ExternalId | text | externalid |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Internal ID | text | id |
| Landed Cost per Line | checkbox | landedcostperline |
| Location | text | location |
| Memo | text | memo |
| Payee | text | entity |
| Posting Period | text | postingperiod |
| Subsidiary | text | subsidiary |
| To Be Printed | checkbox | tobeprinted |
| Total | text | totalwords |
| Total | text | usertotalwords |
| Total | text | wordhundreds |
| Total | text | wordhundredthousands |
| Total | text | wordones |
| Total | text | wordtens |
| Total | text | wordtenthousands |
| Total | text | wordthousands |
| Transaction Number | text | transactionnumber |

## Company Information - companyinformation {#SBADVTemplates_2211315234}

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

## User - user {#SBADVTemplates_137307251}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_2999470055}

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
