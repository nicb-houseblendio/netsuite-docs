---
id: "SBADVTemplates_1124176509"
type: "SBADVTemplates"
title: "Standard Packing Slip PDF/HTML Template"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced Templates Reference > Standard Packing Slip PDF/HTML Template"
parent: "SBADVTemplates"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SBADVTemplates_1124176509.html"
anchors: ["SBADVTemplates_3204976676", "SBADVTemplates_606484987", "SBADVTemplates_3668865389", "SBADVTemplates_4292863533", "SBADVTemplates_1379557337", "SBADVTemplates_4229531217", "SBADVTemplates_3647475985", "SBADVTemplates_2849686417", "SBADVTemplates_1488288430"]
sha256: "ec7ad5cf74b1b0a763d01f81982787e643cf3f1d331f4a1062fb9e4166155f9c"
---

Note:

The list in this reference topic isn't exhaustive. The fields and sublists available in advanced PDF/HTML templates depend on the features you enable in your account and any custom fields you create. Therefore, the list may include fields that aren't available in your account, and at the same time it may not include all fields that you can access.

You can view the fields and sublists available for a specific template in the Field selector in the advanced templates editor. For more information, see [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html).

The fields and sublists available in the Standard Packing Slip PDF/HTML Template template are listed below.

## Record - record {#SBADVTemplates_3204976676}

The following fields are available for the Record record.

| Name | Type | ID |
| --- | --- | --- |
| Address | address | shipaddress |
| Address 1 | text | shipaddr1 |
| Address 2 | text | shipaddr2 |
| Address 3 | text | shipaddr3 |
| Addressee | text | shipcompany |
| Attention | text | shipattention |
| Base Currency | checkbox | isbasecurrency |
| City | text | shipcity |
| Country | text | shipcountry |
| Custom Form | select | customform |
| Customer:Job | select | entity |
| Date | date | trandate |
| Exclude from GL Audit Numbering | checkbox | excludefromglnumbering |
| ExternalId | text | externalid |
| Fulfillment of | select | createdfrom |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Internal ID | text | id |
| Memo | text | memo |
| Phone | phone | shipphone |
| Posting Period | select | postingperiod |
| Ref No. | text | tranid |
| Residential Address | checkbox | shipisresidential |
| Select Address | select | shipaddresslist |
| Ship Via | select | shipmethod |
| Shipping Address | address | shippingaddress\_text |
| Shipping Cost | currency | shippingcost |
| State/Province | text | shipstate |
| Transaction Number | text | transactionnumber |
| Zip | text | shipzip |

### Sublists {#SBADVTemplates_606484987}

The following sublists are available for the Record record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **item** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Back Ordered | float | quantityremainingdisplay |
    | Class | text | class |
    | Department | text | department |
    | Description | text | description |
    | Description | text | itemdescription |
    | Drop Ship PO | text | createpo |
    | Exclude Item from Rate Request | checkbox | excludefromraterequest |
    | Fulfill | checkbox | itemreceive |
    | Item | text | itemkey |
    | Item | text | itemname |
    | Item | text | sitemname |
    | Job | text | jobname |
    | Location | text | location |
    | On Hand | float | onhand |
    | Options | namevaluelist | options |
    | Quantity Remaining | float | quantityremaining |
    | Shipped | posfloat | quantity |
    | Units | text | unitsdisplay |
    
-   The **package** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Package Contents Description | textarea | packagedescr |
    | Package Tracking Number | text | packagetrackingnumber |
    | Weight | posfloat | packageweight |
    

## Sales Order - salesorder {#SBADVTemplates_3668865389}

The following fields are available for the Sales Order record.

| Name | Type | ID |
| --- | --- | --- |
| AVS Street Match | select | ccavsstreetmatch |
| AVS Zip Match | select | ccavszipmatch |
| Acct. No. | text | accountnumber |
| Allow Cross-Subsidiary Fulfillment | checkbox | iscrosssubtransaction |
| Auth. Code | text | authcode |
| Authorization ID | text | paypalauthid |
| Base Currency | checkbox | isbasecurrency |
| Bill To | address | billaddress |
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
| Can Stack Promotions | checkbox | canhavestackable |
| Card Data Provided | checkbox | carddataprovided |
| Card Street | text | ccstreet |
| Card Zip Code | text | cczipcode |
| Cards on File | select | creditcard |
| Class | select | class |
| Credit Card # | ccnumber | ccnumber |
| Credit Card Approved | checkbox | ccapproved |
| Currency | select | currency |
| Currency | text | currencyname |
| Currency Symbol | text | currencysymbol |
| Custom Form | select | customform |
| Customer | select | entity |
| Customer Code | text | customercode |
| Customer Message | textarea | message |
| Default | text | isdefaultshippingrequest |
| Default | float | overrideshippingcost |
| Department | select | department |
| Detail | text | cchold |
| Detail | textarea | ccholdetails |
| End Date | date | enddate |
| Exchange Rate | currency2 | exchangerate |
| Exclude Commissions | checkbox | excludecommission |
| Expires (MM/YYYY) | ccexpdate | ccexpiredate |
| ExternalId | text | externalid |
| FOB | text | fob |
| Generate TranId on Save | checkbox | generatetranidonsave |
| Get Authorization | checkbox | getauth |
| IAVS Match | select | cciavsmatch |
| Ignore AVS | checkbox | ignoreavs |
| Ignore CSC | checkbox | ignorecsc |
| Intercompany Status | select | intercostatus |
| Internal ID | text | id |
| Job | select | job |
| Lead Source | select | leadsource |
| Location | select | location |
| Memo | text | memo |
| Name on Card | text | ccname |
| Nexus | select | nexus |
| Opportunity | select | opportunity |
| Order # | text | tranid |
| Order Date | date | trandate |
| Order Status | text | orderstatus |
| Override Hold | checkbox | overridehold |
| Override Hold | checkbox | overrideholdchecked |
| P/N Ref. | text | pnrefnum |
| PO # | text | otherrefnum |
| Paired Intercompany Transaction | select | intercotransaction |
| Partner | select | partner |
| PayPal Order ID | text | paypalorderid |
| Payment Amount | currency | paymentsessionamount |
| Payment Custom Data | longtext | paymentcustomdata |
| Payment Method | select | paymentmethod |
| Payment Operation | select | paymentoperation |
| Payment Processing Profile | select | creditcardprocessor |
| Process PayPal Payment | checkbox | paypalprocess |
| Project | text | project |
| Purchase Card BIN | checkbox | ccispurchasecardbin |
| Reason | select | paymenteventholdreason |
| Recurring Payment | checkbox | isrecurringpayment |
| Redirect From URL | url | returnurl |
| Redirect to URL | url | redirecturl |
| Sales Effective Date | date | saleseffectivedate |
| Sales Rep | select | salesrep |
| Select Message | select | messagesel |
| Send Line-Level Data | checkbox | ccprocessaspurchasecard |
| Ship Complete | checkbox | shipcomplete |
| Ship Date | date | shipdate |
| Ship To | address | shipaddress |
| Ship To Select | select | shipaddresslist |
| Ship Via | select | shipmethod |
| Shipment # | text | shipid |
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
| Status | select | paymenteventresult |
| Stored tax reference for update | text | taxreferencetobeupdated |
| Subsidiary | select | subsidiary |
| Tax | currency | taxtotal |
| Tax Details Override | checkbox | taxdetailsoverride |
| Tax Reg. Number | select | entitytaxregnum |
| Tax Reg. Number | select | subsidiarytaxregnum |
| Tax Registration Override | checkbox | taxregoverride |
| Tax Strategy Used | text | taxstrategyused |
| Taxes Dirty | checkbox | taxesdirty |
| Terms | select | terms |
| To Be Emailed | checkbox | tobeemailed |
| To Be Faxed | checkbox | tobefaxed |
| To Be Printed | checkbox | tobeprinted |
| Tracking # | text | linkedtrackingnumbers |
| Transaction Number | text | transactionnumber |

### Sublists {#SBADVTemplates_4292863533}

The following sublists are available for the Sales Order record.

To add a sublist to your template, use the record and the sublist, for example, customer.addressbook. For information about adding sublists to a template, see [Sublists and Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163732171457.html#subsect_163890430757).

-   The **accountingbookdetail** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Base Currency | select | currency |
    | Exchange Rate | currency2 | exchangerate |
    | Secondary Book | select | accountingbook |
    
-   The **item** sublist has the following fields:
    
    | Name | Type | ID |
    | --- | --- | --- |
    | Charge Type | text | chargetype |
    | Commit | text | commitinventory |
    | Description | textarea | description |
    | Direct Revenue Posting | text | directrevenueposting |
    | Item | select | item |
    | Item Type | text | itemtype |
    | Item subtype | text | itemsubtype |
    | Line Number | integer | linenumber |
    | Matrix Type | text | matrixtype |
    | Minimum Quantity | float | minqty |
    | Options | namevaluelist | options |
    | Print Items | text | printitems |
    | Project Charge Rule | text | chargerule |
    | Rate | rate | rate |
    | Shipped | float | quantity |
    | Tax Details Reference | text | taxdetailsreference |
    | Units | select | units |
    
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
    

## Company Information - companyinformation {#SBADVTemplates_1379557337}

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

## Subsidiary - subsidiary {#SBADVTemplates_4229531217}

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

### Sublists {#SBADVTemplates_3647475985}

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
    

## User - user {#SBADVTemplates_2849686417}

The following fields are available for the User record.

| Name | Type | ID |
| --- | --- | --- |
| Alt. Email | text | altemail |
| Email | text | email |
| First Name | text | firstname |
| Last Name | text | lastname |
| Middle Name | text | middlename |
| Phone | text | phone |

## Preference - preferences {#SBADVTemplates_1488288430}

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
