---
id: "SBADVTemplates_85934086"
type: "SBADVTemplates"
title: "Standard Invoice PDF/HTML Template (SuiteTax)"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Invoice PDF/HTML Template (SuiteTax)"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_85934086.html"
anchors: ["SBADVTemplates_2492310683", "SBADVTemplates_2986095579", "SBADVTemplates_3147450998", "SBADVTemplates_2434210591", "SBADVTemplates_2407494055", "SBADVTemplates_695834175", "SBADVTemplates_3384547492"]
sha256: "27f3f37dd4d56b12669eb838774bb5e7650f6999a1d3a0c59c49f54f0f91e3da"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Invoice PDF/HTML Template (SuiteTax) template are listed below.

## Record - record {#SBADVTemplates_2492310683}

The following fields are available for the Record record.

| Name | Type | ID |
| --- | --- | --- |
| Account | select | account |
| Acct. No. | text | accountnumber |
| Add Charges | select | whichchargestoadd |
| Amount | currency | expcostdiscamount |
| Amount | currency | itemcostdiscamount |
| Amount | currency | timediscamount |
| As of Date | date | asofdate |
| Balance | currency | balance |
| Base Currency | checkbox | isbasecurrency |
| Bill To | address | billaddress |
| Bill To Select | select | billaddresslist |
| Billing Address | address | billingaddress\_text |
| Billing Address City | text | billcity |
| Billing Address Country | text | billcountry |
| Billing Address Line 1 | text | billaddr1 |
| Billing Address Line 2 | text | billaddr2 |
| Billing Address Line 3 | text | billaddr3 |
| Billing Address State | text | billstate |
| Billing Address Zip Code | text | billzip |
| Billing Addressee | text | billaddressee |
| Billing Attention | text | billattention |
| Billing Phone | text | billphone |
| Can have stackable promotions | checkbox | canhavestackable |
| Class | select | class |
| Coupon Code | select | couponcode |
| Currency | select | currency |
| Currency | text | currencyname |
| Currency Symbol | text | currencysymbol |
| Custom Form | select | customform |
| Customer | select | entity |
| Customer Message | textarea | message |
| Customer Tax Reg. Number | select | entitytaxregnum |
| Date | date | trandate |
| Department | select | department |
| Disc. Amt. | currency | discountamount |
| Disc. Date | date | discountdate |
| Discount Item | select | discountitem |
| Discount Item | currency | discounttotal |
| Discount/Markup | select | expcostdiscount |
| Discount/Markup | select | itemcostdiscount |
| Discount/Markup | select | timediscount |
| Due Date | date | duedate |
| End Date | date | enddate |
| Est. Extended Cost | currency | totalcostestimate |
| Est. Gross Profit | currency | estgrossprofit |
| Est. Gross Profit Percent | percent | estgrossprofitpercent |
| Exchange Rate | currency2 | exchangerate |
| Exclude Commissions | checkbox | excludecommission |
| Exclude from GL Audit Numbering | checkbox | excludefromglnumbering |
| ExternalId | text | externalid |
| FOB | text | fob |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Gift Certificate | currency | giftcertapplied |
| Internal ID | text | id |
| Invoice # | text | tranid |
| Job | select | job |
| Lead Source | select | leadsource |
| Location | select | location |
| Memo | text | memo |
| Nexus | select | nexus |
| Nexus Override | checkbox | taxregoverride |
| Opportunity | select | opportunity |
| PO # | text | otherrefnum |
| Partner | select | partner |
| Payment Custom Data | longtext | paymentcustomdata |
| Posting Period | select | postingperiod |
| Print | checkbox | expcostdiscprint |
| Print | checkbox | itemcostdiscprint |
| Print | checkbox | timediscprint |
| Project | text | project |
| Promo Code | text | muccpromocodeinstance |
| Promo Code | text | promocodepluginimpl |
| Promotion | select | promocode |
| Rate | rate | discountrate |
| Rate | rate | expcostdiscrate |
| Rate | rate | itemcostdiscrate |
| Rate | rate | timediscrate |
| Sales Effective Date | date | saleseffectivedate |
| Sales Rep | select | salesrep |
| Select Message | select | messagesel |
| Ship Date | date | shipdate |
| Ship To | address | shipaddress |
| Ship To Select | select | shipaddresslist |
| Ship Via | select | shipmethod |
| Shipping Address | address | shippingaddress\_text |
| Shipping Address City | text | shipcity |
| Shipping Address Country | text | shipcountry |
| Shipping Address Line 1 | text | shipaddr1 |
| Shipping Address Line 2 | text | shipaddr2 |
| Shipping Address Line 3 | text | shipaddr3 |
| Shipping Address State | text | shipstate |
| Shipping Address Zip Code | text | shipzip |
| Shipping Addressee | text | shipaddressee |
| Shipping Attention | text | shipattention |
| Shipping Cost | currency | shippingcost |
| Shipping Cost Overridden | text | shippingcostoverridden |
| Shipping Phone | text | shipphone |
| Shipping Tax Amount | currency | shippingtaxamount |
| Shipping address is residential | text | billisresidential |
| Shipping address is residential | text | shipisresidential |
| Start Date | date | startdate |
| Stored tax reference for update | text | taxreferencetobeupdated |
| Submission Id | text | bulksubmissionid |
| Subsidiary | select | subsidiary |
| Subsidiary Tax Reg. Number | select | subsidiarytaxregnum |
| Subtotal | currency | subtotal |
| Tax | currency | taxtotal |
| Tax Details Override | checkbox | taxdetailsoverride |
| Tax Strategy Used | text | taxstrategyused |
| Taxes Dirty | checkbox | taxesdirty |
| Terms | select | terms |
| To Be E-mailed | checkbox | tobeemailed |
| To Be Faxed | checkbox | tobefaxed |
| To Be Printed | checkbox | tobeprinted |
| Total | currency | total |
| Total After Taxes | currency | totalaftertaxes |
| Tracking # | text | linkedtrackingnumbers |
| Transaction Number | text | transactionnumber |
| Unbilled Orders | currency | unbilledorders |

### Sublists {#SBADVTemplates_2986095579}

The following sublists are available for the Record record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **accountingbookdetail** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Base Currency | select | currency |
    | Exchange Rate | currency2 | exchangerate |
    | Secondary Book | select | accountingbook |
    
-   The **expcost** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Apply | checkbox | apply |
    | Bill Amount | currency | amount |
    | Category | text | categorydisp |
    | Class | select | class |
    | Date | date | billeddate |
    | Department | select | department |
    | Employee | text | employeedisp |
    | Gross Amount | currency | grossamt |
    | Location | select | location |
    | Memo | text | memo |
    | Original Amount | currency | originalamount |
    | Tax Amount | currency | taxamount |
    | Tax Details Reference | text | taxdetailsreference |
    
-   The **item** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Amount | currency | amount |
    | Charge | text | charge |
    | Charge Type | text | chargetype |
    | Charges | multiselect | charges |
    | Description | textarea | description |
    | Direct Revenue Posting | text | directrevenueposting |
    | Gross Amt | currency | grossamt |
    | Item | select | item |
    | Item Type | text | itemtype |
    | Item subtype | text | itemsubtype |
    | License Code | textarea | licensecode |
    | Line Number | integer | linenumber |
    | Matrix Type | text | matrixtype |
    | Minimum Quantity | float | minqty |
    | Options | namevaluelist | options |
    | Print Items | text | printitems |
    | Quantity | float | quantity |
    | Rate | rate | rate |
    | Tax Amount | currency | taxamount |
    | Tax Details Reference | text | taxdetailsreference |
    | Tax Rate | percent | taxrate |
    | Units | select | units |
    
-   The **itemcost** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Apply | checkbox | apply |
    | Class | select | class |
    | Date | date | billeddate |
    | Department | select | department |
    | Description | text | memo |
    | Gross Amount | currency | grossamt |
    | Item | text | itemdisp |
    | Location | select | location |
    | Options | namevaluelist | options |
    | Qty | text | itemcostcount |
    | Rate | currency2 | cost |
    | Tax Amount | currency | taxamount |
    | Tax Details Reference | text | taxdetailsreference |
    | Total | currency | amount |
    | Units | text | unitdisp |
    
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
    
-   The **time** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Amount | currency | amount |
    | Apply | checkbox | apply |
    | Class | select | class |
    | Date | date | billeddate |
    | Department | select | department |
    | Description | text | memo |
    | Employee | text | employeedisp |
    | Gross Amount | currency | grossamt |
    | Hours | text | quantity |
    | Item | text | itemdisp |
    | Location | select | location |
    | Rate | currency2 | rate |
    | Tax Amount | currency | taxamount |
    | Tax Details Reference | text | taxdetailsreference |
    | Units | text | unitdisp |
    

## Company Information - companyinformation {#SBADVTemplates_3147450998}

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

## Subsidiary - subsidiary {#SBADVTemplates_2434210591}

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

### Sublists {#SBADVTemplates_2407494055}

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
    

## User - user {#SBADVTemplates_695834175}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_3384547492}

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
