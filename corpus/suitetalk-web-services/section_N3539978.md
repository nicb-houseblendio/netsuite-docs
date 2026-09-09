---
id: "section_N3539978"
type: "section"
title: "Error Status Codes"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Error Handling and Error Codes > Error Status Codes"
parent: "chapter_N3536378"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539978.html"
anchors: []
sha256: "697431b7a9526b203f2d159dbb74b67b2ba7065aec384961dfda58dab19ffde9"
---

The following table lists error status code types that can be returned in a message Response. These are values that are used in the code field of the statusDetail type where the type attribute has a value of error.

These codes are listed in the StatusDetailCodeType enumeration, which is defined in the [platform faults XSD](https://webservices.netsuite.com/xsd/platform/v2025_2_0/faults.xsd). You can also view error codes on the [Status Detail Code page of the SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/enum/statusdetailcodetype.html?mode=package).

| Error Code Returned | Long Description or Message |
| --- | --- |
| ABORT\_SEARCH\_EXCEEDED\_MAX\_TIME | This search has timed out. You can choose to schedule it to run in the background and have the results emailed to you when complete. On the saved search form, click the "Email" tab, check "Send According to Schedule", choose an email address on the "Specific Recipients" subtab and a recurrence pattern on the "Schedule" subtab. |
| ABORT\_UPLOAD\_VIRUS\_DETECTED | The file {1} contains a virus {2}. Upload abort. |
| ACCESS\_DENIED | Access to this configuration is denied. Please contact NetSuite to gain access to this configuration. |
| ACCTNG\_PRD\_REQD | Missing next accounting period |
| ACCT\_DISABLED | account disabled |
| ACCT\_DISABLED | This account has been disabled. |
| ACCT\_DISABLED | Please contact <a href=''mailto:{1}''> Accounts Receivable</a> at 650.627.1316 to re-enable this company. |
| ACCT\_DISABLED | Your account has been inactivated by an administrator. |
| ACCT\_MERGE\_DUP | The account merge would result in one or more items using duplicate accounts. |
| ACCT\_NAME\_REQD | Accounts require a name. |
| ACCT\_NEEDS\_CAMPAIGN\_PROVISION | Please contact your account representative to provision campaign emailing for your account. |
| ACCT\_NOT\_CREATED | Account creation was unsuccessful. NetSuite Customer Support has been alerted to this problem. |
| ACCT\_NUM\_REQD | Missing Account Number. Account number is a required field and it cannot be null or empty. |
| ACCT\_NUMS\_REQD\_OR\_DONT\_MATCH | Missing ACCT # or ACCT numbers don't match |
| ACCT\_PERIOD\_SETUP\_REQD | The accounting period range {1} has not been defined. Please visit '<A href='{2}'>_Setup > Accounting > Manage Accounting Periods_</A>' to define this period or set up your year. |
| ACCT\_PRDS\_BEING\_ADDED | Periods are currently being added to this account. Please try again later. |
| ACCT\_REQD | Attempting to adjust provisioning for a customer without an existing account |
| ACCT\_TEMP\_DISABLED | You have entered an invalid password on {1} consecutive attempts. Access to your account has been suspended for {2} minutes. If you have forgotten your password, please contact Customer Support. |
| ACCT\_TEMP\_UNAVAILABLE | Can't update information - this company's database is currently offline for maintenance. Please try again later. |
| ACCT\_TEMP\_UNAVAILABLE | (Temporarily unavailable) |
| ACCT\_TEMP\_UNAVAILABLE | The account you are trying to access is currently unavailable while we undergo our regularly scheduled maintenance. |
| ACCT\_TEMP\_UNAVAILABLE | We are currently performing maintenance on our system. Please try again soon. |
| ACCT\_TEMP\_UNAVAILABLE | The account you are trying to access is currently unavailable while we undergo our regularly scheduled maintenance. |
| ACCT\_TEMP\_UNAVAILABLE | Your account is disabled for {1} more minutes due to {2} consecutive failed login attempts. |
| ACCT\_TEMP\_UNAVAILABLE | Your account is not yet ready for you to log in. Please wait and try again. |
| ACCT\_TEMP\_UNAVAILABLE | Your company database is offline. |
| ACCT\_TEMP\_UNAVAILABLE | Your data is still being loaded. Please try again later. Contact <a href='/app/crm/support/nlcorpsupport.nl?type=bug&spf=31'>Professional Services</a> if you have questions. |
| ACH\_NOT\_AVAILBL | ACH Processing is not available in this environment. |
| ACH\_SETUP\_REQD | Account {1} is not setup for ACH transactions. |
| ACTIVE\_AP\_ACCT\_REQD | This transaction requires an active Accounts Payable account. Please enable an existing Accounts Payable account, create a new Accounts Payable account, or contact your System Administrator. |
| ACTIVE\_ROLE\_REQD | You can only set an active login role as the SOAP web services default role. |
| ACTIVE\_TRANS\_EXIST | There are active direct deposit transactions for this paycheck |
| ADDITIONAL\_AUTHENTICATION\_REQUIRED\_2FA | Additional Authentication required - 2FA. |
| ADDITIONAL\_AUTHENTICATION\_REQUIRED\_SQ | Additional Authentication required - Security Questions. |
| ADDRESS\_LINE\_1\_REQD | Address Line 1 is a required field and it cannot be null or empty. |
| ADMIN\_ACCESS\_REQ | At least one active administrator for each account must have access. |
| ADMIN\_ACCESS\_REQ | At least one active administrator for this account must have access. |
| ADMIN\_ACCESS\_REQD | Only administrators may enter a memorized transaction in a closed period. |
| ADMIN\_ONLY\_ACCESS | {1} only the administrator may access this page. |
| ADMIN\_ONLY\_ACCESS | {1} only the administrator may currently access this page. |
| ADMIN\_USER\_REQD | User is not an Admin of the demo account |
| ADMISSIBILITY\_PACKG\_TYP\_REQD | An Admissibility Package Type is required for this international shipment. |
| ALL\_DATA\_DELETE\_REQD | You must first delete all the data in your account before performing this action. Click <a href='/pages/setup/clearaccount.jsp?import=T'>here</a> to delete your data. |
| ALL\_MTRX\_SUBITMES\_OPTNS\_REQD | The following matrix subitems exist but aren't included in the options you just specified. On the Matrix tab, please make sure the options you select include all existing subitems:<p> {1} |
| ALREADY\_IN\_INVT | The following {1} numbers are already in inventory: {2} |
| ALREADY\_IN\_INVT | The following {1} number is already in inventory: {2} |
| AMORTZN\_INVALID\_DATE\_RANGE | Amortization end date can not be before amortization start date. |
| AMORTZN\_TMPLT\_DATA\_MISSING | One or more line items on this transaction have Variable Amortization Templates, but do not have the required {1} also populated. Please either change the Template for these items or indicate which {1} will be used to schedule the amortization. |
| AMT\_DISALLWD | Description items may not have an amount. |
| AMT\_EXCEEDS\_APPROVAL\_LIMIT | No one in your chain of command has a sufficient spending limit to approve this transaction. |
| ANSWER\_REQD | Please provide an answer. |
| APPROVAL\_PERMS\_REQD | {1} The restrictions on your role do not allow you to approve or reject this record. |
| AREA\_CODE\_REQD | Please include an area code with the phone number. |
| ASSIGNEE\_REQD | {1} must be assigned to {2} |
| AT\_LEAST\_ONE\_FILE\_REQD | Download folder must have at least one file. |
| AT\_LEAST\_ONE\_PACKAGE\_REQD | 1 or more packages are required. |
| AT\_LEAST\_ONE\_RETURN\_FLD\_REQD | You must specify at least one field to be returned. |
| AT\_LEAST\_ONE\_SUB\_REQD | You must choose at least one subsidiary. |
| ATTACH\_SIZE\_EXCEEDED | The data you are uploading exceeds the maximum allowable size of {1}. Please change your selection and try again |
| ATTACH\_SIZE\_EXCEEDED | This message exceeds the limit of 24 MB. Please reduce the size of the message and its attachments and try again.<br/>Note: Files can be larger when attached due to encoding. |
| ATTACHMNT\_CONTAINS\_VIRUS | The attachment with file name {1} contains a virus {2}. It is removed from the message. |
| ATTACHMNT\_CONTAINS\_VIRUS | The attachment file {0} contains virus {1}. Save message abort. |
| AUDIT\_W2\_1099 | Use this report to audit the information that will be used to generate W2s and 1099s. |
| AUTO\_NUM\_UPDATE\_DISALLWD | We currently do not support an automatic numbering update of more than {1} {2} records. Please contact <A href='/app/crm/support/nlcorpsupport.nl?type=support'>NetSuite Customer Support</A> to request a full numbering update of your {2}s.</a> |
| AVS\_ERROR | This order failed the AVS check and will not be saved.<br><br>An AVS mismatch has been detected and the transaction has been rejected. However, a valid authorization has been created against the cardholder's account. If you want to accept this order, click Go Back and check the Ignore AVS checkbox and Save the order. Note that this will result in a second authorization. |
| BALANCE\_EXCEEDS\_CREDIT\_LIMIT | Customer balance exceeds credit limit |
| BANK\_ACCT\_REQD | You must have a bank account to perform this operation. Click <a href='/app/accounting/account/account.nl'>here</a> to add one. |
| BASE\_CRNCY\_REQD | You may not delete you base currency. |
| BILLABLES\_DISALLWD | {1} does not allow billables. |
| BILLING\_ISSUES | Your account has been locked due to billing issues. You must call your NetSuite Sales Representative for further assistance. |
| BILLING\_ISSUES | Your account has not been fully paid for. Please log in to your account and follow the billing process or contact your Account Manager. |
| BILLING\_SCHDUL\_INVALID\_RECURR | Billing schedules may not have a recurrence count greater than 500 |
| BIN\_DSNT\_CONTAIN\_ENOUGH\_ITEM | The following bins do not contain enough of the requested item ({1}): {2} |
| BIN\_DSNT\_CONTAIN\_ENOUGH\_ITEM | The following bin does not contain enough of the requested item ({1}): {2} |
| BIN\_ITEM\_UNAVAILBL | The following bins are not available for the specified item: {1} |
| BIN\_ITEM\_UNAVAILBL | The following bins are not available for the specified item ({1}): {2} |
| BIN\_ITEM\_UNAVAILBL | The following bin in not available for the specified item ({1}): {2} |
| BIN\_ITEM\_UNAVAILBL | The following bin is not available for the specified item: {1} |
| BIN\_SETUP\_REQD | The following bins are not associated with the item '{1}': {2}.<br>You can associate bins with an item on the inventory tab of the item record. |
| BIN\_UNDEFND | The following bins specified for the item {1} are not defined in the transaction location ({2}): {3} |
| BUNDLE\_IS\_DEPRECATED | This bundle is no longer available. It has been deprecated by bundle {1} on account {2}. |
| BUNDLE\_IS\_DEPRECATED | You cannot update this bundle as it has been deprecated and you have not been granted access to the replacement bundle. Please contact the solution provider. |
| CALENDAR\_PREFS\_REQD | Set up {1} Calendar Preferences first. |
| CALENDAR\_PREFS\_REQD | Set up Calendar Preferences first |
| CAMPAGIN\_ALREADY\_EXECUTED | You cannot delete email campaigns that have already been executed |
| CAMPAIGN\_IN\_USE | You cannot delete a campaign event that already has activity. |
| CAMPAIGN\_SET\_UP\_REQD | The following steps need to be performed before a campaign can be created:<p>{1} |
| CANNOT\_RESET\_PASSWORD | Sorry, we are currently unable to reset your password. Please contact support or try again later. |
| CANT\_APPLY\_PMT | The top level entity cannot accept payment because it has a status of {1}. It must have a status of {2} or {3} to accept payment. |
| CANT\_APPLY\_PMT | This entity cannot accept payment because it has a status of {1}. It must have a status of {2} or {3} to accept payment. |
| CANT\_AUTO\_CREATE\_ADJSTMNT | The 'Intercompany Expenses' accounting preference does not currently support the automated creation of adjustments. If you would like to create adjustments automatically, please change that preference to 'Allow and Auto Adjust.' |
| CANT\_CALC\_FEDEX\_RATES | FedEx rates cannot be calculated: |
| CANT\_CANCEL\_APPRVD\_RETRN\_AUTH | You cannot cancel this return authorization because it has already been approved. |
| CANT\_CHANGE\_CONTACT\_RESTRICTN | You cannot change the restriction on this contact. |
| CANT\_CHANGE\_CRMRECORDTYPELINKS | Cannot alter standard CrmRecordTypeLinks |
| CANT\_CHANGE\_EVENT\_PRIMARY\_TYP | You cannot change the primary type for this event |
| CANT\_CHANGE\_IP\_ADDRESS | The domain {1} is currently associated with IP address {2}. You cannot change the IP address of a live domain. |
| CANT\_CHANGE\_LEAD\_SOURCE\_CAT | You cannot change the category for a leadsource that is defined as the default leadsource for another category |
| CANT\_CHANGE\_PSWD | You changed your password less than 24 hours ago. NetSuite only allows one password change per 24-hour period. |
| CANT\_CHANGE\_REV\_REC\_TMPLT | The rev rec template on a billable expense can not be changed or removed after it is saved. |
| CANT\_CHANGE\_REV\_REC\_TMPLT | The rev rec template on billable time and items can not be changed or removed after it is saved. |
| CANT\_CHANGE\_SUB | You cannot change the subsidiary on this record because doing so will change the subsidiary selected on the associated employee record. |
| CANT\_CHANGE\_TASK\_LINK | Cannot alter standard task links |
| CANT\_CHANGE\_UNITS\_TYP | You may not change the units type of an item after it has been set. |
| CANT\_CHANGE\_VSOE\_ALLOCTN | You are attempting to change the VSOE Allocation for a transaction in a closed period. You must either change the posting period for the related transaction or open the period. |
| CANT\_CHG\_POSTED\_BILL\_VRNC | The receipts for this bill can not be changed after the bill variance has been posted. |
| CANT\_CHG\_POSTED\_BILL\_VRNC | One or more lines have had their bill variance posted and can not be changed. |
| CANT\_COMPLETE\_FULFILL | The fulfillment cannot be completed. |
| CANT\_CONNECT\_TO\_STORE | Error - Unable to connect to store {1} |
| CANT\_CONVERT\_CLASS\_DEPT | You cannot convert classes to departments because you already have department data in the system. You must remove all departments first. |
| CANT\_CONVERT\_CLASS\_LOC | You cannot convert classes to locations because you already have location data in the system. You must remove all locations first. |
| CANT\_CONVERT\_INVT\_ITEM | This item is a member of a kit or a non-numbered assembly. You may not convert it to a numbered inventory item. |
| CANT\_CREAT\_SHIP\_LABEL | A shipping label could not be generated because the In Bond Code field is not set. Please enter a value in the In Bond Code field on the Item Fulfillment page. |
| CANT\_CREATE\_FILES | Could not create files for uploading your data |
| CANT\_CREATE\_NON\_UNIQUE\_RCRD | A record with the same unique signatures already exists. You must enter unique signatures for each record you create. |
| CANT\_CREATE\_PO | Purchase Orders cannot be created for assembly items. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because a currency must be defined for the "Ship From" country "{1}" when using the Insured Value option. Go to Lists -> Accounting -> Currencies to create a currency for {1}. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because a currency must be defined for the "Ship To" country "{1}" when using the COD option. Go to Lists -> Accounting -> Currencies to create a currency for {1}. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Addressee field of the "Ship To" address is not set. Please enter a "Ship To" Addressee on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Address 1 field of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" Address 1. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Address 1 field of the "Ship To" address is not set. Please enter a "Ship To" Address 1 on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Attention field of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" Attention. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the City field of the "Ship To" address is not set. Please enter a "Ship To" City on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the City of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" City. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Company or Location Name of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" Company/Location Name. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Country field of the "Ship To" address is not set. Please enter a "Ship To" Country on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Country of the "Ship From" address is not set. Please go to $(regex) to set the "Ship From" Country. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Package Weight was not entered. Please enter a value in the Package Weight field on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Phone Number of the "Ship From" address is not set. Please go to $(regex) to set the "Ship From" Phone Number. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Phone Number of the "Ship To" address is not set. Please enter a "Ship To" Phone Number on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Pickup Type was not set. Please go to _Setup > Set Up Shipping_ to select a shipping Pickup Type. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the shipping method was not set. Please go to Lists > Shipping Items to select a Shipping Label Integration shipping method for this shipping item. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the State field of the "Ship To" address is not set. Please enter a "Ship To" State on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the State of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" State. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Zip Code of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" Zip Code. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because the Zip field of the "Ship To" address is not set. Please enter a "Ship To" Zip code on the Item Fulfillment page. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Account Number is not set. Go to Setup > Set Up Shipping > {2} Registration to enter your {3} Account Number. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration Address Line 1 is not set. Go to Setup > {2} Registration to complete the Address Line 1 field. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration City is not set. Go to Setup > {2} Registration to enter your City. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration Company field is not set. Go to Setup > {2} Registration to enter a name in the Company field. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration Country is not set. Go to Setup > {2} Registration to select your Country. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration Ship to Attention field is not set. Go to Setup > {2} Registration to enter a name in the Ship to Attention field. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration State is not set. Go to Setup > {2} Registration to select or enter your State. |
| CANT\_CREATE\_SHIP\_LABEL | A shipping label could not be generated because your {1} Registration Zip Code is not set. Go to Setup > {2} Registration to enter your Zip Code. |
| CANT\_CREATE\_WORK\_ORD | Work orders can only be created for assembly items. |
| CANT\_DEL\_DEFAULT\_CALENDAR |  |
| CANT\_DEL\_DEFAULT\_SHIP\_METHOD | This Shipping Item cannot be deleted because it is the Default Shipping Method. Please go to _Setup > Accounting > Set Up Shipping_ and choose a new Default Shipping Method before deleting this Shipping Item. |
| CANT\_DEL\_REALIZED\_GAINLOSS | A Realized Gain/Loss Transaction cannot be deleted. |
| CANT\_DEL\_TRANS\_RVRSL | The reversal of the month-end Unrealized Gain/Loss transaction cannot be deleted. |
| CANT\_DELETE\_ACCT | This account cannot be deleted because it has associated transactions. |
| CANT\_DELETE\_ACCT | This account cannot be deleted because it is a special type of account needed by {1} |
| CANT\_DELETE\_ACCT | This account cannot be deleted because it is a special type of account needed by NetSuite |
| CANT\_DELETE\_ACCT | This account cannot be deleted because it is a special type of account needed by the system. |
| CANT\_DELETE\_ACCT | This account cannot be deleted because it is used by one or more transactions or it has child accounts or it is used by one or more items. |
| CANT\_DELETE\_ACCT\_PRD | You may not delete an accounting period with transactions posted to it. You must first edit the transactions, change the posting period and then delete the period. |
| CANT\_DELETE\_ALLOCTN | This allocation detail can not be deleted because it has a journal entry. |
| CANT\_DELETE\_BIN | You may not delete this bin record because it is already in use. You must either remove all references to it in item records and transactions or make it inactive. |
| CANT\_DELETE\_CATEGORY | This category cannot be deleted because it has child items |
| CANT\_DELETE\_CATEGORY | This category cannot be deleted because it has subcategories |
| CANT\_DELETE\_CC\_PROCESSOR | This credit card processor is used in transaction and cannot be deleted. |
| CANT\_DELETE\_CELL | This cell cannot be deleted because it has child items |
| CANT\_DELETE\_CHILD\_RCRD\_FOUND | This {1} record cannot be deleted because it is referenced by other records. |
| CANT\_DELETE\_CHILD\_RCRDS\_EXIST | This record can not be deleted because it has child records. |
| CANT\_DELETE\_CLASS | This class cannot be deleted because it has child items |
| CANT\_DELETE\_COLOR\_THEME | This color theme cannot be deleted because it is being used |
| CANT\_DELETE\_COMMSSN\_SCHDUL | This schedule has already been used to generate commission calculations and can't be deleted. If no authorizations have been made, schedule can be deleted after being removed from all active plans. |
| CANT\_DELETE\_COMPANY | This company cannot be deleted because it has child entities |
| CANT\_DELETE\_COMPANY\_TYP | This company type cannot be deleted because the company has associated transactions. |
| CANT\_DELETE\_CONTACT\_HAS\_CHILD | The contact record cannot be deleted because it has child records. |
| CANT\_DELETE\_CONTACT\_HAS\_CHILD | This contact cannot be deleted because it has child entities |
| CANT\_DELETE\_CSTM\_FIELD | This custom field cannot be deleted because it is referred to by other custom fields |
| CANT\_DELETE\_CSTM\_FORM | This custom form cannot be deleted because it is referred to by other custom forms |
| CANT\_DELETE\_CSTM\_ITEM\_FIELD | This custom item field has dependent matrix items. It can not be deleted. |
| CANT\_DELETE\_CSTM\_LAYOUT | This custom layout cannot be deleted because it is used by custom forms |
| CANT\_DELETE\_CSTM\_LIST | This custom list cannot be deleted because it is referred to by custom fields |
| CANT\_DELETE\_CSTM\_RCRD | This custom record cannot be deleted because it is referred to by custom fields |
| CANT\_DELETE\_CSTM\_RCRD\_ENTRY | This custom record entry cannot be deleted because it is referred to by other records |
| CANT\_DELETE\_CUST | You can't delete this customer because it's set up as default Anonymous Customer |
| CANT\_DELETE\_CUSTOMER | This customer or job cannot be deleted because it has child entities. |
| CANT\_DELETE\_DEFAULT\_FLDR | You cannot delete the default folders. |
| CANT\_DELETE\_DEFAULT\_PRIORITY | You cannot delete the default case priority. Please select a new default first. |
| CANT\_DELETE\_DEFAULT\_SALES\_REP | Default Sales Rep Role cannot be deleted. |
| CANT\_DELETE\_DEFAULT\_STATUS | You cannot delete a default case status. Please select a new default first. |
| CANT\_DELETE\_DEFAULT\_STATUS | You can't delete or inactivate that status because it is a set up as a default status. Please navigate to <a href='/app/setup/sfasetup.nl' target='\_blank'>Sales Preferences</a> and change that status |
| CANT\_DELETE\_DEFAULT\_VALUE | You may not delete or inactivate that value because it is a default. Please select a new default first. |
| CANT\_DELETE\_DEFAULT\_WEBSITE | The default Web site cannot be deleted. |
| CANT\_DELETE\_EMPL | This employee cannot be deleted because it has child entities |
| CANT\_DELETE\_ENTITY | This entity cannot be deleted because it has child items |
| CANT\_DELETE\_FIN\_STATMNT\_LAYOUT | This financial statement layout cannot be deleted because it is referred to by other layouts. |
| CANT\_DELETE\_FLDR | These predefined folders cannot be deleted |
| CANT\_DELETE\_HAS\_CHILD\_ITEM | This {1} cannot be deleted because it has child items |
| CANT\_DELETE\_INFO\_ITEM | This information item cannot be deleted because it has child items |
| CANT\_DELETE\_ITEM | This item cannot be deleted because it has child items |
| CANT\_DELETE\_ITEM\_LAYOUT | This item/category layout cannot be deleted because it is used by store tabs |
| CANT\_DELETE\_ITEM\_TMPLT | This item/category template cannot be deleted because it is referred to by a theme or an item |
| CANT\_DELETE\_JOB\_RESOURCE\_ROLE | Default Job Resource Role cannot be deleted. |
| CANT\_DELETE\_LEGACY\_CATEGORY | Legacy category cannot be removed |
| CANT\_DELETE\_LINE | This line cannot be deleted, because it is referred to by other records. Before removing this line, remove any discount or markup lines applied to it. |
| CANT\_DELETE\_MEDIA\_ITEM | This media item cannot be deleted because it is being referenced by another item. |
| CANT\_DELETE\_MEMRZD\_TRANS | This memorized transaction cannot be deleted because it referenced in transactions |
| CANT\_DELETE\_OR\_CHANGE\_ACCT | Special accounts cannot be deleted and their type cannot be changed |
| CANT\_DELETE\_PLAN\_ASSGNMNT | Trying to delete plan assignment referenced by precalcs. |
| CANT\_DELETE\_PRESNTN\_CAT | This presentation category cannot be deleted because it has subcategories |
| CANT\_DELETE\_RCRD | This {1} record cannot be deleted because it referenced by other records |
| CANT\_DELETE\_RCRD | This record cannot be deleted because it has {1}child records{2} |
| CANT\_DELETE\_RCRD | This record cannot be deleted because it is referenced by other records or it is used by one or more transactions. |
| CANT\_DELETE\_RCRD | This record cannot be deleted, because it is referred to by other records. |
| CANT\_DELETE\_RCRDS | Selected records could not be deleted because one or more of them are of a special type of account needed by {1} |
| CANT\_DELETE\_RCRDS | Selected records could not be deleted because one or more of them are referenced by other records. |
| CANT\_DELETE\_SITE\_TAG | This site tag cannot be deleted because it is being used. |
| CANT\_DELETE\_SITE\_THEME | This site theme cannot be deleted because it is being used |
| CANT\_DELETE\_SOLUTN | This solution cannot be deleted because it has been applied to support cases. |
| CANT\_DELETE\_STATUS\_TYPE | You cannot delete the only status of type {1} |
| CANT\_DELETE\_SUBTAB | This subtab cannot be deleted because it is referred to by custom fields |
| CANT\_DELETE\_SYSTEM\_NOTE | You cannot alter or delete a system logged note. |
| CANT\_DELETE\_TAX\_VENDOR | This is a special tax vendor and cannot be deleted. |
| CANT\_DELETE\_TMPLT\_RCRD | This template record cannot be deleted. |
| CANT\_DELETE\_TRANS | This transaction cannot be deleted because it is a Google Checkout order awaiting updated payment information. |
| CANT\_DELETE\_TRANS | This transaction cannot be deleted because it is a posting Google Checkout order. |
| CANT\_DELETE\_TRANS | This transaction cannot be deleted because it is linked to one or more commission transactions. The commission authorizations due to this transaction need to be removed to be able to delete this transaction. |
| CANT\_DELETE\_TRANS | This transaction cannot be deleted because it is referenced by an intercompany adjustment. The adjustment must be deleted first. |
| CANT\_DELETE\_TRANS | This transaction cannot be deleted because it is referred to by other transactions. It may be a bill or an invoice that has been paid or an expense that has been reimbursed. |
| CANT\_DELETE\_TRAN\_LINE | Failed to delete line {1}. This line is linked to another transaction. |
| CANT\_DELETE\_TRAN\_LINES | Lines with partially recognized rev rec or amortization schedules can not be deleted. |
| CANT\_DELETE\_UPDATE\_ACCT | This account cannot be deleted or changed because it is a special type of account needed by {1} |
| CANT\_DELETE\_URL | This third party conversion tracking URL cannot be deleted because it is reference by other records. |
| CANT\_DELETE\_VENDOR | This {1:Vendor} is related to a {2:Partner} which is eligible for commission and cannot be deleted. |
| CANT\_DELETE\_VENDOR | This vendor cannot be deleted because there are dependent items, such as a pending payment. If you wish to remove the payee, you must first delete all such dependent items. |
| CANT\_DIVIDE\_BY\_ZERO | There is a divide by zero error in this search. It may be an error with a formula you have used. Please retry without the formula(s). If an error still occurs, please file with Customer Support. If it does not, please correct your formula. Typically that consists of taking the denominator and wrapping it in NULLIF(<denominator>,0). |
| CANT\_DOWNLOAD\_EXPIRED\_FILE | This file has expired and can no longer be downloaded |
| CANT\_EDIT\_CHARGED\_ORDER | You cannot charge an order that is already completely charged. |
| CANT\_EDIT\_CUST\_LIST | Can not modify this Custom List because its entries are in use. |
| CANT\_EDIT\_CUST\_PMT | This customer payment cannot be edited while it has an Automated Clearing House transmission in process.</TD></TR><TR><TD class=text> </TD></TR><TR><TD class=text> To view the status of customer payments with ACH transmissions, go to Transactions > View Electronic Funds Transfer Status. |
| CANT\_EDIT\_DPLYMNT\_IN\_PROGRESS | You cannot change or delete a deployment that is in progress or in the queue. |
| CANT\_EDIT\_DPLYMNT\_IN\_PROGRESS | You cannot edit a script deployment when it is being executed. |
| CANT\_EDIT\_FOLDER | Predefined folders cannot be updated. |
| CANT\_EDIT\_OLD\_CASE | This case cannot be edited because it was closed {1} or more days ago. |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard dashboards |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard dashboard role maps |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard dashboard section maps |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard fields |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard forms or layouts |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard portlets |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard report snapshot layouts |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard roles |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard searches |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard sections |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard tabs |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard tasks |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard task categories |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard templates |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot Alter Standard Types |
| CANT\_EDIT\_STANDARD\_OBJ | Cannot alter standard words |
| CANT\_EDIT\_TAGATA | The Receivable Tegata is linked to Invoices and is no longer editable |
| CANT\_EDIT\_TRAN | You cannot edit intercompany adjustments. |
| CANT\_EDIT\_TRAN | You cannot edit the account of a transaction line that is linked to others |
| CANT\_EDIT\_TRAN | You cannot edit this expense report |
| CANT\_EDIT\_TRAN | You cannot edit this transaction because it was automatically created by the Payroll feature |
| CANT\_ESTABLISH\_LINK | Unable to establish link with {1} |
| CANT\_FIND\_BUG | Cannot locate the bug that was just entered (1)! |
| CANT\_FIND\_MAIL\_MERGE\_ID | Mail Merge Id not found |
| CANT\_FIND\_RCRD | Could not find record with {1} = {2} |
| CANT\_FIND\_SAVED\_IMPORT | No saved import with internalId {1} |
| CANT\_FIND\_SOURCE\_AMORTZN\_ACCT | The source account for the amortization schedule could not be determined. |
| CANT\_FIND\_UPS\_REG\_FOR\_LOC | No UPS registration was found for the location selected. Please select a different shipping item, or go to Setup > Set Up Shipping to register a UPS account for this location. |
| CANT\_FULFILL\_ITEM | An item receipt has been posted |
| CANT\_INACTIVATE\_COMMSSN\_PLAN | You cannot inactivate a plan that has commission payments that are pending authorization. Please clear the commission payments at _Transactions > Authorize Commissions_ before inactivating this plan. |
| CANT\_INACTIVE\_DEFAULT\_SYNC\_CAT | You cannot inactivate the default synchronization category. |
| CANT\_INACTIVE\_DEFAULT\_TMPLT | You cannot inactivate this template record because it is set up as a default template |
| CANT\_LOAD\_SAVED\_SEARCH\_PARAM | Error loading saved search params |
| CANT\_LOGIN\_WITH\_OAUTH | A login operation or Request Level Credentials must not be used in conjunction with OAuth authorization{:do not translate 'login' or capitalized words} |
|  | Can not lookup field {1} by {2} |
| CANT\_MAKE\_CONTACT\_PRIVATE | Employee contacts cannot be made private |
| CANT\_MAKE\_CONTACT\_PRIVATE | Individual relationship contacts cannot be made private |
| CANT\_MARK\_SHIPPED | Item {1:item name} cannot be marked shipped because the remaining quantity on the linked purchase order does not match the remaining quantity on the sales order. |
| CANT\_MERGE\_EMPLS | employees can not be merged |
| CANT\_MODIFY\_APPRVD\_TIME | Time records can not be modified after they have been approved. |
| CANT\_MODIFY\_FULFILL\_STATUS | You may not change the fulfillable status of an item which has transactions associated with it. |
| CANT\_MODIFY\_ISSUE\_STATUS | The issue status '{1:issue status name}' cannot be changed from {2:base status} to {3:base status} because it is in use. |
| CANT\_MODIFY\_LOCKED\_FLD | You may not update or delete a locked custom field. |
| CANT\_MODIFY\_PARENT | Payments have been accepted from the top level parent. The top level parent can not be changed. |
| CANT\_MODIFY\_REV\_REC | The value of Rev Rec on Rev Commit may not be modified for this transaction. |
| CANT\_MODIFY\_SUB | You cannot change the subsidiary of this entity because one or more transactions exist for this entity. |
| CANT\_MODIFY\_TAGATA | The Payable Tegata is no longer in Issued state and cannot be modified.' |
| CANT\_MODIFY\_TAGATA | The Receivable Tegata is no longer in Holding state and cannot be modified. |
| CANT\_MODIFY\_TEGATA | The Payable Tegata is linked to bills and cannot be modified.' |
| CANT\_MODIFY\_VOID\_TRANS | The G/L impact of a voided transaction cannot be changed. |
| CANT\_MODIFY\_VOID\_TRANS | You may not change the GL impact on a voided {1: transaction type}. |
| CANT\_MOVE\_REALIZED\_GAINLOSS | You cannot move a Realized Gain/Loss transaction to a date before either the source or the payment transaction. |
| CANT\_PAY\_TAGATA | Endorsed Tegata can only be paid on or after its maturity date. |
| CANT\_PAY\_TAGATA | Payable Tegata can only be paid on or after its maturity date. |
| CANT\_PROCESS\_IMG | Faceless PDF Library unable to process image. Image DPI:{1}. |
| CANT\_RCEIV\_BEFORE\_FULFILL | The item receipt for a transfer order line can not occur before the item fulfillment. |
| CANT\_RCEIV\_ITEM | A mark shipped fulfillment line has been processed against item {1:item name}. This item cannot be received. |
| CANT\_RECEIVE\_TAGATA | Receivable Tegata can only be collected on or after its maturity date. |
| CANT\_REJECT\_ORDER | You cannot reject this order because it has already been approved. |
| CANT\_REMOV\_ALL\_FULFILMNT\_LINKS | You may not modify this sales order in such a way that it removes all links to any fulfillment. The modifications you made would leave the fulfillment <a href="https://docs.oracle.com/app/accounting/transactions/transaction.nl?id={1}">{2}</a> unlinked. |
| CANT\_REMOV\_ITEM\_SUB | You may not remove a subsidiary from an item that is a member of an assembly, group, or kit item if the parent item is available in that subsidiary. |
| CANT\_REMOVE\_ACH\_PAY\_METHOD | ACH payment methods cannot be removed |
| CANT\_REMOVE\_APPROVAL | The accounting approval cannot be removed from this expense report because some of its lines have already been invoiced to the customer. |
| CANT\_REMOVE\_DOMAIN | You are trying to remove a domain that is referenced by {1} CRM template(s). Please first clear the domain from CRM templates before trying to remove it. |
| CANT\_REMOVE\_NEXUS | A nexus cannot be removed from a subsidiary if the nexus is associated with a transaction. |
| CANT\_REMOVE\_SCHDUL | You have attempted to remove an active schedule from a plan. Removing this participant is not permitted after commissions against the plan have been generated. |
| CANT\_REMOVE\_SUB | You cannot remove subsidiary: {1} because this record is used on a transaction for subsidiary: {1}. |
| CANT\_REMOVE\_SUB | You attempted to remove one or more subsidiaries from this item, but the item appears in at least one transaction in those subsidiaries. To remove a subsidiary from the item, make sure the item does not appear in any transactions for that subsidiary. |
| CANT\_RESUBMIT\_FAILED\_DPLYMNT | You cannot submit a deployment for execution whose status is set to Scheduled. |
| CANT\_RETURN\_FLD | Can not return field {1}. Reason: {2} |
| CANT\_RETURN\_USED\_GIFT\_CERT | Used gift certificates can not be returned. |
| CANT\_REV\_REC\_BODY\_AND\_LINE | The Revenue Recognition fields must be specified at EITHER the transaction body or the item line level, and may NOT be specified at both levels. |
| CANT\_REVERSE\_AUTH | Card type doesn't allow reversals. No resolution. Authorization cannot be reversed. |
| CANT\_SCHDUL\_RECUR\_EVENT | Because the number of days in each month differs, recurring monthly events cannot be scheduled after the 28th. |
| CANT\_SEND\_EMAIL | Unable to send notification email |
| CANT\_SEND\_EMAIL | Unable to send notification email to support rep |
| CANT\_SET\_CLOSE\_DATE | Unable to set expected close date of prospect/lead based on current estimates/opportunities. |
| CANT\_SET\_INTERNALID | You cannot set internalId with upsert. |
| CANT\_SET\_STATUS | Unable to set status of prospect/lead based on current estimates. |
| CANT\_SWITCH\_ROLES\_FROM\_LOGIN | Role switching is not allowed from this login. |
| CANT\_SWITCH\_SHIP\_METHOD | Switching the shipping method to another carrier is an unsupported operation, because it requires reloading the item fulfillment form for that carrier. |
| CANT\_UPDATE\_ACCTNG\_PRDS | You cannot update accounting periods using SuiteScript or SOAP web services. Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_. |
| CANT\_UPDATE\_AMT | The amount on lines containing partially/fully recognized schedules can not be changed |
| CANT\_UPDATE\_DYNAMIC\_GROUP | You cannot update dynamic groups. Instead you must modify the saved search associated with the group |
| CANT\_UPDATE\_FLDR | These predefined folders cannot be updated |
| CANT\_UPDATE\_LINKED\_TRANS\_LINES | You cannot update linked transaction lines |
| CANT\_UPDATE\_PRODUCT\_FEED | This item has multiple product feeds. SOAP web services schema version 2\_6 or greater is required to modify product feeds for this item |
| CANT\_UPDATE\_RECRD\_HAS\_CHANGED | Cannot update bug. Record has changed since you last retrieved it. |
| CANT\_UPDATE\_RECUR\_EVENT | Event <id {1}> contains recurrence patterns that are not supported in your client application. You are not allowed to update recurrence pattern on this event. Contact your software vendor for the latest Web Services upgrade. |
| CANT\_UPDATE\_ROOT\_CATEGORY | Can not update root level website categories through SOAP web services. |
| CANT\_UPDATE\_STATUS\_TYPE | You cannot update the only status of type {1} |
| CANT\_VERIFY\_CARD | Card Verify not supported. Retry request. |
| CANT\_VOID\_TRANS | You cannot void this transaction because it is linked to by one or more transactions such as payments. You must delete or void those transactions first |
| CARD\_EXPIRED | Expired Card. Re-submit with valid expiration date. |
| CARD\_ID\_REQD | Card ID required. Provide a valid card ID. |
| CASE\_ALREADY\_ASSIGNED | This case cannot be grabbed because it is already assigned to another rep. To view the case, go back and click the case number. |
| CASE\_DSNT\_EXIST | Case doesn't exist or no customer is associated with case. |
| CASE\_NOT\_GROUP\_MEMBER | {1} this case record does not belong to your group. |
| CASH\_SALE\_EDIT\_DISALLWD | This cash sale cannot be edited while it has an Automated Clearing House transmission in process.</TD></TR><TR><TD class=text> </TD></TR><TR><TD class=text> To view the status of cash sales with ACH transmissions, go to Transactions > View Electronic Funds Transfer Status. |
| CC\_ACCT\_REQD | You must have a credit card account to perform this operation. |
| CC\_ACCT\_REQD | You must have a credit card account to perform this operation. Click <a href='/app/accounting/account/account.nl'>here</a> to add one. |
| CC\_ALREADY\_SAVED | That credit card is already saved. Please use the saved credit card. |
| CC\_EMAIL\_ADDRESS\_REQD | Please go back and provide an email address to CC store orders to. |
| CC\_NUM\_REQD | Please provide a credit card number. |
| CC\_PROCESSOR\_ERROR | An error occurred while processing the credit card. Please contact the merchant for assistance. |
| CC\_PROCESSOR\_ERROR | An unexpected error occurred while processing the credit card through MerchantE (reason code = {1}). Please contact NetSuite support. |
| CC\_PROCESSOR\_NOT\_FOUND | A suitable credit card processor was not found for this transaction. |
| CC\_SECURITY\_CODE\_REQD | This transaction requires the Credit Card Security Code. Please enter the required value in the {1} field and re-submit. |
| CERT\_AUTH\_EXPD | CA expired on {1} |
| CERT\_EXPD | Certificate expired on {1} |
| CERT\_UNAVAILABLE | Certificate unavailable (most likely has not been presented by client) |
| CHANGE\_PMT\_DATE\_AND\_REAPPROVE | The payment is more than 30 days past due and has NOT been sent. Edit the payment to change the date and reapprove. |
| CHAR\_ERROR | Character error on Line# {1} Column# {2} (Byte # {3}). {4} |
| CHECKOUT\_EMAIL\_REQD | Please go back and provide an email address to email checkout errors to. |
| CITY\_REQD | City is a required field and it cannot be null or empty. |
| CLASS\_ALREADY\_EXISTS | A class already exists with that name. Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| CLASS\_OR\_DEPT\_OR\_CUST\_REQD | only one of class, cust, and dept can be non-null |
| CLEAR\_AUTOCALC | For items that use the time phased replenishment method, you must clear the Auto-Calculate checkbox next to the Reorder Point and Preferred Stock Level fields. The mass update cannot be performed unless these settings are changed. |
| CLOSE\_PREVIOUSE\_PERIOD | Please close previous period before working on this one. |
| CLOSED\_TRAN\_PRD | The G/L impact of a transaction in a closed period cannot be changed. |
| CLOSED\_TRAN\_PRD | You cannot move a transaction to or from a closed period. |
| COGS\_ERROR | COGS lines not cleaned up |
| COGS\_ERROR | Cost of Goods Sold lines not in balance |
| COGS\_ERROR | LIFO/FIFO COGS count does not equal the number of items requested COGS ERROR 9765 itemsLinked={1}, itemsTotal={2} kdoc={3}, nid={4} |
| COMMSSN\_ALREADY\_CALCLTD | You have attempted to remove an active sales participant from a plan. Removing this participant is not permitted after commissions against the plan have been generated. |
| COMMSSN\_FEATURE\_DISABLED | You have not enabled the Commissions feature. |
| COMMSSN\_FEATURE\_DISABLED | You have not enabled the Partner Commissions/Royalties feature. |
| COMMSSN\_PAYROLL\_ITEM\_REQD | A commission payroll item must be added for each employee to be processed through payroll |
| COMP\_DELETED\_OR\_MERGED | The company you try to attach the context to has been deleted or merged. |
| COMPANION\_PROP\_REQD | Error - Items do not have companion property (column) {1} |
| COMPANY\_FLD\_REQD | The Company field is required for COD shipments. Go to _Setup > Accounting > Shipping_, set the Company field on your FedEx Registration record and re-submit. |
| CONCUR\_BILLPAY\_JOB\_DISALLWD | Your account currently has a bill pay approval job in progress. Only one bill pay approval job per account is allowed at a time. Please wait until this process completes before submitting another group of payments for approval. <BR><BR>Visit the <a href='/app/external/xml/upload/uploadlog.nl?displayType=BILLPAY'>status page </a> to track the progress of the current job. |
| CONCUR\_BULK\_JOB\_DISALLWD | This Account is already running a bulk processing job. Please visit the <a href='/app/external/xml/upload/uploadlog.nl?displayType=BULKFULFILL'>status page </a> to track the progress of the current job. |
| CONCUR\_MASS\_UPDATE\_DISALLWD | A mass update is currently running in this account. Please try again in a few minutes. |
| CONCUR\_SEARCH\_DISALLWD | Search aborted by concurrent {1} search. Only one search may run at a time. |
| CONSLD\_PRNT\_AND\_CHILD\_DISALLWD | A company can be a consolidated child or a consolidated parent but not both |
| CONTACT\_ALREADY\_EXISTS | A contact record with this name already exists. Every contact record must have a unique name. |
| CONTACT\_ALREADY\_EXISTS | A contact with the name \[{1}\] already exists |
| CONTACT\_NOT\_GROUP\_MEMBR | {1} this contact does not belong to your group. |
| COOKIES\_DISABLED | You have disabled cookies from being stored on your computer or turned off per-session cookies. Please enable this feature and try again |
| COUNTRY\_STATE\_MISMATCH | The country and state/province are mismatched, the country is {1} and the state/province is {2}. Please enter a state/province short name that matches the country. |
| CREATEDFROM\_REQD | Please enter a value for createdFrom. |
| CREDITS\_DISALLWD | Credits Not Allowed. Contact MerchantE to have credits enabled. |
| CRNCY\_MISMATCH\_BASE\_CRNCY | The currency you are registered to use is different from the base currency of this company. |
| CRNCY\_NOT\_UPDATED | The following currencies were not updated: {1} |
| CRNCY\_RCRD\_DELETED | This currency record has been deleted. You can create a new currency record at _Lists > Accounting > Currencies > New_. |
| CRNCY\_REQD | currency expected for pricing element |
| CSC\_SETUP\_REQD | To display the CSC field on the form, you must enable the "Use Card Security Code for Credit Card Transactions" preference, located on the _Setup > Accounting Preferences_ task. |
| CSTM\_FIELD\_KEY\_REQD | The specified custom field key is missing. |
| CSTM\_FIELD\_VALUE\_REQD | The specified custom field value is missing. |
| CSV\_DELIMITER\_ERROR | Values in the following CSV file(s) are not comma separated, and cannot be imported. Please reformat the file(s) and try again. For instructions, <a href='javascript:nlPopupHelp("DOC\_Reformatting\_Semi-Colon\_Separated\_CSV\_Files","help")'>visit this help topic.</a> |
| CUST\_ARLEADY\_HAS\_ACCT | Attempting to provision a new account to a customer with an existing account |
| CUST\_CNTR\_USER\_ACCESS\_ONLY | This form is only accesible to customer center users. |
| CUST\_LEAD\_NOT\_GROUP\_MEMBR | {1} this customer or lead does not belong to your group. |
| CYBERSOURCE\_ERROR | An unexpected error occurred while processing the credit card through CyberSource (reason code = {1}). Please contact NetSuite Customer Support. |
| CYBERSOURCE\_ERROR | : The credit card was declined by the card issuer. Use a different card for payment or contact the card issuer for more information. |
| CYBERSOURCE\_ERROR | The credit card transaction was denied by the issuing bank. Please try another card or contact the card issuer for more information. |
| CYBERSOURCE\_ERROR | The credit card has expired or the expiration date does not match the date on file with the card issuer. Please correct the expiration date or try another card. |
| CYBERSOURCE\_ERROR | The credit card transaction was denied due to insufficient funds. Please try another card or contact the card issuer for more information. |
| CYBERSOURCE\_ERROR | The credit card transaction could not be completed because the issuing bank was not available. Please try another card or wait a few minutes and try again. |
| CYBERSOURCE\_ERROR | Inactive card or card not authorized for card-not-present transactions. Please try another card or contact the card issuer for more information. |
| CYBERSOURCE\_ERROR | The card has reached the credit limit. Please try another card or contact the card issuer for more information. |
| CYBERSOURCE\_ERROR | Invalid card verification number. Please check to make sure you have provided the correct card verification number. |
| CYBERSOURCE\_ERROR | Invalid credit card account number. Please check to make sure you have provided the correct credit card account number. |
| CYBERSOURCE\_ERROR | The type of credit card provided is not accepted by this merchant. Please try another card or contact the merchant for more information. |
| CYBERSOURCE\_ERROR | Successful transaction. |
| CYBERSOURCE\_ERROR | The request is missing one or more required fields. Possible action: See the reply fields missingField\_0...N for which fields are missing. Resend the request with the complete information. |
| CYBERSOURCE\_ERROR | One or more fields in the request contains invalid data. Possible action: See the reply fields invalidField\_0...N for which fields are invalid. Resend the request with the correct information. |
| CYBERSOURCE\_ERROR | The merchantReferenceCode sent with this authorization request matches the merchantReferenceCode of another authorization request that you sent in the last 15 minutes. Possible action: Resend the request with a unique merchantReferenceCode value. |
| CYBERSOURCE\_ERROR | Error: General system failure. See the documentation for your CyberSource client (SDK) for information about how to handle retries in the case of system errors. |
| CYBERSOURCE\_ERROR | Error: The request was received but there was a server timeout. This error does not include timeouts between the client and the server. Possible action: To avoid duplicating the order, do not resend the request until you have reviewed the order status in the Business Center. See the documentation for your CyberSource client (SDK) for information about how to handle retries in the case of system errors. |
| CYBERSOURCE\_ERROR | Error: The request was received, but a service did not finish running in time. Possible action: To avoid duplicating the order, do not resend the request until you have reviewed the order status in the Business Center. See the documentation for your CyberSource client (SDK) for information about how to handle retries in the case of system errors. |
| CYBERSOURCE\_ERROR | The issuing bank has questions about the request. You do not receive an authorization code programmatically, but you might receive one verbally by calling the processor. Possible action: Call your processor or the issuing bank to possibly receive a verbal authorization. For contact phone numbers, refer to your merchant bank information. |
| CYBERSOURCE\_ERROR | Expired card. You might also receive this if the expiration date you provided does not match the date the issuing bank has on file. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | General decline of the card. No other information provided by the issuing bank. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | Insufficient funds in the account. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | Stolen or lost card. Possible action: Review the customers information and determine if you want to request a different card from the customer. |
| CYBERSOURCE\_ERROR | Issuing bank unavailable. Possible action: Wait a few minutes and resend the request. |
| CYBERSOURCE\_ERROR | Inactive card or card not authorized for card-not-present transactions. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | The card has reached the credit limit. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | Invalid card verification number. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | The customer matched an entry on the processors negative file. Possible action: Review the order and contact the payment processor. |
| CYBERSOURCE\_ERROR | Invalid account number. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | The card type is not accepted by the payment processor. Possible action: Request a different card or other form of payment. Also, check with CyberSource Customer Support to make sure your account is configured correctly. |
| CYBERSOURCE\_ERROR | General decline by the processor. Possible action: Request a different card or other form of payment. |
| CYBERSOURCE\_ERROR | There is a problem with your CyberSource merchant configuration. Possible action: Do not resend the request. Contact Customer Support to correct the configuration problem. |
| CYBERSOURCE\_ERROR | The requested amount exceeds the originally authorized amount. Occurs, for example, if you try to capture an amount larger than the original authorization amount. This reason code only applies if you are processing a capture through the API. See Using the API for Captures and Credits. Possible action: Issue a new authorization and capture request for the new amount. |
| CYBERSOURCE\_ERROR | Processor failure. Possible action: Tell the customer the payment processing system is unavailable temporarily, and to try their order again in a few minutes. |
| CYBERSOURCE\_ERROR | The authorization has already been captured. This reason code only applies if you are processing a capture through the API. See Using the API for Captures and Credits. Possible action: No action required. |
| CYBERSOURCE\_ERROR | The requested transaction amount must match the previous transaction amount. This reason code only applies if you are processing a capture or credit through the API. See Using the API for Captures and Credits. Possible action: Correct the amount and resend the request. |
| CYBERSOURCE\_ERROR | The card type sent is invalid or does not correlate with the credit card number. Possible action: Ask your customer to confirm that the card is the type that they indicated in your Web store, then resend the request. |
| CYBERSOURCE\_ERROR | The request ID is invalid. This reason code only applies when you are processing a capture or credit through the API. See Using the API for Captures and Credits. Possible action: Request a new authorization, and if successful, proceed with the capture. |
| CYBERSOURCE\_ERROR | You requested a capture through the API, but there is no corresponding, unused authorization record. Occurs if there was not a previously successful authorization request or if the previously successful authorization has already been used by another capture request. This reason code only applies when you are processing a capture through the API. See Using the API for Captures and Credits. Possible action: Request a new authorization, and if successful, proceed with the capture. |
| CYBERSOURCE\_ERROR | The capture or credit is not voidable because the capture or credit information has already been submitted to your processor. Or, you requested a void for a type of transaction that cannot be voided. This reason code applies only if you are processing a void through the API. See Using the API for Voids for information about voids. Possible action: No action required. |
| CYBERSOURCE\_ERROR | You requested a credit for a capture that was previously voided. This reason code applies only if you are processing a void through the API. See Using the API for Voids for information about voids. Possible action: No action required. |
| CYBERSOURCE\_ERROR | Error: The request was received, but there was a timeout at the payment processor. Possible action: To avoid duplicating the transaction, do not resend the request until you have reviewed the transaction status in the Business Center. |
| CYBERSOURCE\_ERROR | The authorization request was approved by the issuing bank but declined by CyberSource based on your Smart Authorization settings. Possible action: Do not capture the authorization without further review. Review the ccAuthReply\_avsCode, ccAuthReply\_cvCode, and ccAuthReply\_authFactorCode fields to determine why CyberSource rejected the request. |
| CYBERSOURCE\_ERROR | Unable to process credit card transaction. The code returned from CyberSource {1} is not a recognized reason code. Please contact NetSuite support. |
| CYCLE\_IN\_PROJECT\_PLAN | The changes made to this entity have cause a cycle in the project plan. Select a different parent and/or predecessors to avoid the cycle. |
| DASHBOARD\_LOCKED | Your dashboard has been set up and locked by an administrator. Please contact them for details. |
| DATA\_MUST\_BE\_UNIQUE | The update failed because every entry in this column must be unique. |
| DATA\_REQD | You need to provide a proper value for the required field: {1}. |
| DATA\_REQD | You are missing the following required field(s):{1} |
| DATE\_EXPECTED | You entered '{1}' into a field where a calendar date was expected.\\nPlease go back and change this value to the correct date. |
| DATE\_PARAM\_REQD | missing date parameter |
| DATE\_PRD\_MISMATCH | Your transaction date does not fall between the start and end dates of your accounting period. |
| DEFAULT\_CUR\_REQD | Default currency cannot be null |
| DEFAULT\_EXPENSE\_ACCT\_REQD | A default expense account must be specified to activate items on the list. Go to _Setup > Payroll > Set Up Payroll_ and click the Default Accounts subtab. In the Payroll Expenses Account field, choose a default general ledger account for your payroll expenses. Then, click Save. |
| DEFAULT\_ISSUE\_OWNER\_REQD | There is no default owner for the issue role {1}. This operation cannot be completed until this is corrected. |
| DEFAULT\_LIAB\_ACCT\_REQD | A default liability account must be specified to activate items on the list.nGo to _Setup > Payroll > Set Up Payroll_ and click the Default Accounts subtab. In the Payroll Liabilities Account field, choose a default general ledger account for your payroll liabilities. Then, click Save. |
| DEFAULT\_ROLE\_REQD | Login Failed because you do not have a default role for the company and email entered. Please Try Again. |
| DEFAULT\_TYPE\_DELETE\_DISALLWD | You cannot delete default types |
| DEFERRAL\_ACCT\_REQD | Lines with amortization templates must have a deferral account. |
| DEFERRAL\_ACCT\_REQD | Lines with revenue recognition templates must have a deferral account. |
| DEFERRED\_REV\_REC\_ACCT\_REQD | The {1} item does not have a Deferred Revenue Account specified. Please assign the item a Deferred Revenue Account using the standard User Interface, and then re-import the transaction. |
| DEPT\_IN\_USE | Your classes cannot be converted to departments because your existing department records are referred to by transactions or other records. These department records cannot be overwritten. |
| DFRNT\_SWAP\_PRICE\_LEVELS\_REQD | Please select different price levels to swap prices. |
| DISALLWD\_IP\_ADDRESS | The specified IP address rules must allow the login of your current IP Address. Your current IP address is {1}. For information on entering IP address rules, click Help at the top of the page. |
| DISCOUNT\_ACCT\_SETUP\_REQD | Please <a href='/app/setup/acctsetup.nl'>Set Up Discount Accounts</a> first. |
| DISCOUNT\_DISALLWD | You have attempted to save this transaction with one or more discounts and where all items have Permit Discount = Never. You must change one of the items to permit a discount, add a new item without the restriction or remove the discount from the transaction. |
| DISCOUNT\_DISALLWD\_VSOE | Posting discounts are not allowed on items in VSOE bundles. |
| DISCOUNT\_EXCEED\_TOTAL | Discount can not exceed item total. |
| DISTRIB\_REQD\_ONE\_DAY\_BFORE | All items must be distributed at least one day before they may be transferred. |
| DOMAIN\_IN\_USE | The domain {1} is already in use |
| DOMAIN\_WEBSITE\_REQD | Please select a Web Site for domain {1} |
| DROP\_SHIP\_ERROR | The following error occurred when updating the quantity on the drop ship {1:transaction type}: <p>{2:error message}</p> |
| DROP\_SHIP\_ERROR | The transaction was successfully saved, but an error occurred while running user events and email alerts after updating the drop ship {1:transaction type}(s) |
| DROP\_SHIP\_ERROR | The transaction was successfully saved, but an error occurred while running user events after updating the drop ship {1:transaction type}(s) |
| DROP\_SHIP\_OR\_SPECIAL\_ORD\_ALLWD | Items can be Drop Ship or Special Order but not both |
| DUE\_DATE\_BFORE\_START\_DATE | Due date occurs before start date |
| DUE\_DATE\_REQD | Please enter a value for {1} Due Date |
| DUP\_ACCT\_NAME | The account name you have chosen is already used.<br>Go <a href='javascript:history.go(-1);';>back</a>, change the name and resubmit. |
| DUP\_ACCT\_NOT\_ALLWD | You may not use duplicate accounts on an item. |
| DUP\_ACCT\_NUM | The account number you have chosen is already used. |
| DUP\_ACCT\_NUM | The account number you have chosen is already used.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the number and resubmit. |
| DUP\_ACCT\_ON\_TRANS | This transaction has duplicate accounts. The main line of the transaction and the line labeled '{1}' both use the account named '{2}'. |
| DUP\_BIN | A bin already exists with that name. Go back, change the name, and resubmit. |
| DUP\_BIN | There is already another bin with that number. Please choose a bin number that is not used by another bin. |
| DUP\_BUNDLE\_IN\_ACCT | That bundle has already been copied or installed in this account. |
| DUP\_BUNDLE\_IN\_ACCT | You cannot install this bundle as it is a copy of bundle {1} that you previously installed. |
| DUP\_CATEGORY | This category already exists |
| DUP\_CATEGORY\_NAME | A category already exists with that name. Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_COLOR\_THEME | This color theme already exists |
| DUP\_CSTM\_FIELD | This custom field already exists |
| DUP\_CSTM\_LAYOUT | This custom layout already exists |
| DUP\_CSTM\_LIST | There is already a Custom List or Custom List element with that name |
| DUP\_CSTM\_RCRD | There is already a Custom Record with that name |
| DUP\_CSTM\_RCRD\_ENTRY | There is already a Custom Record Entry with that name |
| DUP\_CSTM\_TAB | This custom tab already exists |
| DUP\_EMPL\_EMAIL | There is already an employee with external access to this account using that email address. All employees with external access must have a unique email address for login purposes. Go <a href="javascript:history.go(-1);";>back</a>, change the email address and resubmit. |
| DUP\_EMPL\_ENTITY\_NAME | There is already an employee with external access to this account using that entity name. All employees with external access must have a unique entity name for login purposes. Go <a href="javascript:history.go(-1);";>back</a>, change the entity name and resubmit. |
| DUP\_EMPL\_TMPLT | There is already an employee template with that name. Go <a href="javascript:history.go(-1);";>back</a>, change the template name and resubmit. |
| DUP\_ENTITY | This entity already exists. |
| DUP\_ENTITY\_EMAIL | There is already an external entity (eg. customer, vendor, or employee) with access to this account using that email address. All external entities with access must have a unique email address for login purposes. |
| DUP\_ENTITY\_NAME | There is already an external entity (eg. customer, vendor, or employee) with access to this account using that entity name. All external entities with access must have a unique entity name for login purposes. |
| DUP\_FEDEX\_ACCT\_NUM | There is an existing NetSuite registration for FedEx account number {1}. |
| DUP\_FINANCL\_STATMNT\_LAYOUT | This financial statement layout already exists. |
| DUP\_INFO\_ITEM | This information item already exists |
| DUP\_ISSUE\_NAME\_OR\_NUM | You cannot set {1:issue record name} {2:issue number} to be a duplicate of itself or one of its duplicates. |
| DUP\_ITEM | Uniqueness error - there is already an item with that name or name/parent combination. |
| DUP\_ITEM\_LAYOUT | This item/category layout already exists |
| DUP\_ITEM\_NAME | There is already an item with that name.<br>. Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_ITEM\_OPTION | A child item child with that combination of options already exists |
| DUP\_ITEM\_TMPLT | This item/category template already exists |
| DUP\_MATRIX\_OPTN\_ABBRV | Matrix option '{1}' already uses that abbreviation. Please choose another. |
| DUP\_MEMRZD\_TRANS | There is already a Memorized Transaction with that name.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_NAME | That name is already in use.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_PAYROLL\_ITEM | There is already a payroll item named {1} |
| DUP\_PRESNTN\_CAT | This presentation category already exists |
| DUP\_RCRD | A {1} already exists with that name. Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_RCRD | Matched more than one record for {1} |
| DUP\_RCRD | Matched more than one record (internalIds {1} and {2}) |
| DUP\_RCRD | This record already exists |
| DUP\_RCRD\_LINK | Link to that record already exists |
| DUP\_SALES\_TAX\_ITEM | You have entered a duplicate Sales Tax Item.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the name, city, state or zip code and resubmit. |
| DUP\_SHIPPING\_ITEM | You have entered a duplicate Shipping Item.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_SHORT\_NAME | Duplicate short name |
| DUP\_SITE\_THEME | This site theme already exists |
| DUP\_SOURCE\_ACCT | Duplicate source accounts are not allowed. |
| DUP\_TAX\_CODE | You have entered a duplicate Tax Code.<br>Go <a href="javascript:history.go(-1);";>back</a>, change the name and resubmit. |
| DUP\_TAX\_CODE | You have entered a duplicate Tax Code.<br>Go <a href=\\"javascript:history.go(-1);\\";>back</a>, change the name, city, state or zip code and resubmit. |
| DUP\_TRACKING\_NUM | You entered the following tracking number twice: {1}. Note that a single tracking number may not contain spaces or commas. A space or comma will be interpreted as the separator between different tracking numbers. For example, '1029 3847 465' will be interpreted as 3 different tracking numbers. It should be entered without spaces: '10293847465'. |
| DUP\_TRANS | Duplicate Trans. Unable to locate, no match. |
| DUP\_UPS\_ACCT\_NUM | There is an existing NetSuite registration for UPS account number {1}. |
| DUP\_VENDOR\_EMAIL | There is already a vendor with external access to this account using that email address. All vendors with external access must have a unique email address for login purposes. Go <a href='javascript:history.go(-1);';>back</a>, change the email address and resubmit. |
| DUP\_VENDOR\_NAME | There is already a vendor using that entity name. All vendors must have a unique entity name. Go <a href="javascript:history.go(-1);";>back</a>, change the entity name and resubmit. |
| DUPLICATE\_INVENTORY\_NUM | Duplicate inventory number found in entry: {1} |
| DUPLICATE\_INVENTORY\_NUM | Duplicate inventory number found on different lines of transaction |
| DUPLICATE\_KEYS | This record contains duplicated key or keys. Please correct it before next update. |
| DUPLICATE\_NAME\_FOR\_PRD | Please choose a different period name. "{1}" is already taken. |
| DUPLICATE\_NAME\_FOR\_ROLE | Please choose a different role name. "{1}" is already taken. |
| EARNING\_ITEM\_REQD | At least one employee in this payroll has no earning items.<br>Please make sure that every employee has at least one earning item. |
| EDITION\_DSNT\_SUPRT\_WORLDPAY | WorldPay is not supported in this edition. |
| EIN\_OR\_TIN\_REQD | You must set either the Employer Identification Number (EIN) or SSN/TIN (Social Security Number, Tax ID Number) to complete this fulfillment. Please go to _Setup > Company > Company Information_ to set either of these fields and re-submit. |
| EMAIL\_ADDRS\_REQD | Please enter your email address |
| EMAIL\_ADDRS\_REQD\_TO\_NOTIFY | Please enter an email address for this company. A notification email will be sent when this case record is saved. |
| EMAIL\_ADDRS\_REQD\_TO\_NOTIFY | The recipient you are sending this email to does not have an email address. Please enter one and try again |
| EMAIL\_REQ\_HANDLER\_ERROR | an error occurred while instantiating an email requesthandler |
| EMAIL\_REQ\_HANDLER\_ERROR | An Error occurred while performing system-level validation of email request for <{1}> from <{2}> |
| EMAIL\_REQ\_HANDLER\_ERROR | An Error occurred while POSTing data into requestHandlder: {1} |
| EMAIL\_REQ\_HANDLER\_ERROR | an error occurred while servicing an email requesthandler in state: {1} |
| EMAIL\_REQD | You must enter a valid email address to email the transaction. |
| EMAIL\_REQD\_ACCT\_PROVISION | Cannot provision an account without an email address for this customer: Was external access granted? |
| EMPL\_IN\_USE | You can't delete this employee, as commissions have been calculated for this employee. |
| EMPL\_IN\_USE | You can't delete this employee, as it is or has been referenced by other employees as a supervisor. |
| ERROR\_DELETE\_CARD\_DATA | Failed to delete card data. Retry request. |
| ERROR\_IN\_TERRITORY\_ASSGNMNT | Error Performing Initial Round\_Robin Assignment for Territory: {1} |
| ERROR\_IN\_TERRITORY\_ASSGNMNT | Error Performing Round\_Robin Assignment for Territory: {1} |
| ERROR\_PRCSSNG\_TRANS | There were errors processing the selected transactions. Please process them individually for more information. |
| ERROR\_REFUND\_TRANS | Failed to refund International transaction. Retry request. |
| ERROR\_REVERSE\_AUTH | Failed to reverse International authorization. Retry request. |
| ERROR\_SENDING\_TRAN\_EMAIL | The transaction was entered successfully, but an unexpected error occurred while sending the transaction email {1} |
| ERROR\_VOID\_TRANS | Failed to void International transaction. Retry request. |
| EVENT\_ID\_NOT\_FOUND | Event ID not found |
| EXCEEDED\_MAX\_ALLWD\_LOC | You have reached the maximum allowance of {1} location records. If you need to create additional location records, please contact our NetSuite Customer Support team for assistance |
| EXCEEDED\_MAX\_CONCUR\_RQST | The maximum number of concurrent requests has been exceeded. Please try your request again when an existing session has completed. |
| EXCEEDED\_MAX\_EMAILS | This account has {1} more bulk emails that can be sent. If you would like to purchase an additional block of emails, please contact your account manager. |
| EXCEEDED\_MAX\_EMAILS | The merge exceeds the number of bulk merge emails allotted to your account this year. This account has {1} more bulk emails that can be sent this year. Please contact your NetSuite account manager to purchase additional block of emails. |
| EXCEEDED\_MAX\_EMAILS | This campaign email event exceeds the number of emails ({1}) that can be sent per event without setting up a default campaign domain or specifying one on the campaign email template. |
| EXCEEDED\_MAX\_EMAILS | This merge operation exceeds the number of emails ({1}) that can be sent per execution without setting up a bulk merge domain or specifying one on the email template. |
| EXCEEDED\_MAX\_EMAILS | You cannot schedule more than {1} emails per year. If you'd like to purchase an additional block of emails, please contact your account manager. |
| EXCEEDED\_MAX\_FEATURED\_ITEMS | There is a limit of {1} featured items on this page. |
| EXCEEDED\_MAX\_FIELD\_LENGTH | Address line 1 cannot exceed 35 characters. Please check the shipper and recipient address to ensure the "Address 1" field is a maximum of 35 characters. |
| EXCEEDED\_MAX\_FIELD\_LENGTH | Address line 2 cannot exceed 35 characters. Please check the shipper and recipient address to ensure the "Address 2" field is a maximum of 35 characters. |
| EXCEEDED\_MAX\_FIELD\_LENGTH | The field {1} contained more than the maximum number ( {2} ) of characters allowed. |
| EXCEEDED\_MAX\_FIELD\_LENGTH | The string "{1}" contained more than the maximum number of characters allowed. |
| EXCEEDED\_MAX\_FIELD\_LENGTH | Too many characters for a field |
| EXCEEDED\_MAX\_MATRIX\_OPTNS | The total combination of subitems you have selected exceeds the maximum allowed of 2000. Please choose fewer options on the matrix tab. |
| EXCEEDED\_MAX\_MATRIX\_OPTNS | The total combination of subitems you have selected exceeds the maximum allowed of 2000. Please choose fewer options on the matrix tab. |
| EXCEEDED\_MAX\_PDF\_ELEMENTS | There is a maximum of 100 custom elements allowed on a PDF layout. |
| EXCEEDED\_MAX\_PDF\_EXPORT\_COL | PDF Export is limited to 30 columns. |
| EXCEEDED\_MAX\_PIN\_RETRIES | PIN entered incorrectly too often. |
| EXCEEDED\_MAX\_RCRD | You have reached the maximum allowance of {1} {2} records. If you need to create additional {2} records, please contact our NetSuite Customer Support team for assistance |
| EXCEEDED\_MAX\_REPORT\_COL | The option you selected in the Column field results in a report that exceeds the maximum number of columns allowed. Please select additional filters or select a shorter date/period range. |
| EXCEEDED\_MAX\_REPORT\_ROWS | Reports are limited to {1} rows. Please narrow your results. |
| EXCEEDED\_MAX\_REPORT\_SIZE | The results of this report are too large. Please narrow your results. |
| EXCEEDED\_MAX\_SESSIONS | Maximum active sessions exceeded. Please wait 5 minutes and login again. |
| EXCEEDED\_MAX\_SHIP\_PACKAGE | The maximum number of custom shipping packages has been exceeded: {1}. Please reduce item quantities to generate fewer packages, or enter the packages manually. |
| EXCEEDED\_MAX\_TIME | The operation has exceeded maximum allowed time for completion. Operation aborted. |
| EXCEEDED\_MAX\_TRANS\_LINES | Transactions may not contain more than {1} lines. |
| EXCEEDED\_MAX\_USERS\_ALLWD | The changes you have made to this employee's access have caused you to exceed either your full access or Employee Center allowance. To make these changes you must either adjust the number of employees assigned the Employee Center role or contact your account representative to purchase additional licenses. |
| EXCEEDED\_MAX\_USERS\_ALLWD | Assigning this role would exceed your full access licenses ({1}). To assign this role, you must remove another employee's full access roles or contact your account representative to purchase additional licenses. |
| EXCEEDED\_MAX\_USERS\_ALLWD | The changes you have made to this employee's access have caused you to exceed either your full access or Retail User allowance. To make these changes you must either adjust the number of employees assigned the Retail Clerk role or contact your account representative to purchase additional licenses. |
| EXCEEDED\_PER\_TRANS\_MAX | Exceeded per transaction maximum on account {1} |
| EXCEEDED\_RQST\_SIZE\_LIMIT | You have exceeded the permitted request size limit ({1}) |
| EXCEEDS\_ALLWD\_LICENSES | Adding access for this user exceeds the number of licenses you have purchased. To add another user, you must first remove access from an existing user or contact NetSuite to purchase additional licenses. |
| EXCEEDS\_ALLWD\_LICENSES | Adding a {1} would exceed the number of licenses you have purchased. Please contact NetSuite for additional licenses. |
| EXPENSE\_ENTRY\_DISALLWD | {1} does not allow expense entry. |
| EXPIRED\_SEARCH\_CRITERIA | Your search criteria expired. The criteria for a specific search generally expire after 15 minutes of inactivity. Please return to the search definition page and re-submit your search. |
| EXT\_CAT\_LINK\_SETUP\_REQD | Error - you have not properly set up links from your External Catalog Site back into {1}! |
| EXTERNALID\_NOT\_SUPPORTED | Field {1} does not support externalId |
| EXTERNALID\_REQD | This operation requires a value for externalId. |
| FAILED\_FEDEX\_LABEL\_VOID | Failed FedEx Label Void |
| FAILED\_FORM\_VALIDATION | Form validation failed. You cannot submit this record. |
| FAILED\_UPS\_LABEL\_VOID | Failed UPS Label Void |
| FAX\_NUM\_REQD | You must enter a fax number. |
| FAX\_NUM\_REQD | You must enter a fax number for this recipient before performing a fax merge operation. |
| FAX\_NUM\_REQD | You must enter a valid fax number to fax the transaction. |
| FAX\_SETUP\_REQD | Before you can send faxes, you need to go to the <a href='/app/setup/printing.nl'>Set Up Printing, Fax & Email</a> page and set up the fax service. |
| FEATURE\_DISABLED | You do not have the correct features enabled to search on {1}. |
| FEATURE\_DISABLED | The ''{1}'' feature is not enabled in your {2} account. |
| FEATURE\_DISABLED | The feature '{1}' required to access this page is not enabled in this account. |
| FEATURE\_UNAVAILABLE | <b>{1} Trial does not allow access to this feature.</b> If you would like more information about this feature, please contact your account manager. |
| FEATURE\_UNAVAILABLE | Error - This business does not have the External Catalog Site feature enabled. |
| FEATURE\_UNAVAILABLE | Test Drive does not allow access to this feature. If you would like more information about this feature, please contact your account manager. |
| FEATURE\_UNAVAILABLE | That feature is only available to Plus users |
| FEATURE\_UNAVAILABLE | The {1} feature is not available to your company. |
| FEATURE\_UNAVAILABLE | This feature is not available to your company. |
| FED\_ID\_REQD | Must have Federal Identification Number to process 1099-MISC forms. |
| FED\_WITHHOLDING\_REQD | Your employee record does not have current Federal Withholding information.<p>Please contact your supervisor to set up your record with the appropriate information.</p> |
| FEDEX\_ACCT\_REQD | The FedEx Account Number has not been set. |
| FEDEX\_CANT\_INTEGRATE\_FULFILL | The fulfillment cannot be integrated with {1} because the Shipping Integration Carrier is set to UPS. |
| FEDEX\_DROPOFF\_TYP\_REQD | The FedEx Dropoff Type has not been set. |
| FEDEX\_INVALID\_ACCT\_NUM | This account number was not recognized by FedEx. Please re-enter your account number, or contact FedEx to open a new account. |
| FEDEX\_ITEM\_CONTENTS\_REQD | For international shipments, {1} requires specific information about the item contents. |
| FEDEX\_METER\_NOT\_RETRIEVED | A FedEx Meter Number was not retrieved for account number {1}. Please try your request again in a few minutes. |
| FEDEX\_METER\_REQD | The FedEx Meter Number has not been set. |
| FEDEX\_ONE\_PACKG\_ALLWD | The selected FedEx service allows only one package per fulfillment. If more than one package is required, please break up the shipment into multiple fulfillments of one package each. |
| FEDEX\_ORIGIN\_COUNTRY\_US\_REQD | The origin country must be United States (US) for all Item Fulfillments when using a FedEx shipping method. |
| FEDEX\_RATING\_SRVC\_UNAVAILBL | The FedEx rating services application is currently unavailable. Please try your request again in a few minutes. |
| FEDEX\_REG\_NOT\_FOUND | A valid FedEx Registration was not found for the specified location: |
| FEDEX\_SHIP\_SRVC\_REQD | The FedEx Shipping Service has not been set. |
| FEDEX\_SHIP\_SRVC\_UNAVAILBL | The FedEx shipping services application is currently unavailable. Please try your request again in a few minutes. |
| FEDEX\_UNSUPRTD\_ORIGIN\_COUNTRY | The origin country {1} is currently not supported for Item Fulfillments when using a FedEx shipping method. |
| FEDEX\_USD\_EXCHANGE\_RATE\_REQD | Cannot retrieve FedEx realtime rates: USD Exchange Rate is required when requesting FedEx realtime rates. |
| FEDEX\_VOID\_ERROR | The FedEx Void failed due to a system error. |
| FIELD\_CALL\_DATE\_REQD | Missing Required Field: Call Date |
| FIELD\_DEFN\_REQD | Field definition not found |
| FIELD\_NOT\_SETTABLE\_ON\_ADD | You are not allowed to set the nsKey for a record |
| FIELD\_PARAM\_REQD | Please enter a value for {1} |
| FIELD\_PARAM\_REQD | Please enter values for {1}. |
| FIELD\_REQD | Mandatory Field Missing |
| FIELD\_REQD | You must first select a field |
| FILE\_ALREADY\_EXISTS | A file with the same name already exists in the selected folder. |
| FILE\_ALREADY\_EXISTS | Note: You are attempting to upload a file with a name matching an existing file in the selected folder. Please rename this file or select another folder, and then upload your file. |
| FILE\_DISALLWD\_IN\_ROOT\_FLDR | You attempted to copy a file to the root directory. Only folders can exist in the root directory. |
| FILE\_DISALLWD\_IN\_ROOT\_FLDR | You attempted to move a file to the root directory. Only folders can exist in the root directory. |
| FILE\_MISSING | File Missing |
| FILE\_NOT\_DOWNLOADABLE | Illegal request for a file that isn't downloadable |
| FILE\_NOT\_FOUND | File/Media Item {1} not found. |
| FILE\_NOT\_FOUND | File not found. Please try your download again. |
| FILE\_REQD | You must enter a file before submitting this form. |
| FILE\_REQD | You must upload a file before creating this media item |
| FILE\_UPLOAD\_IN\_PROGRESS | Files are currently being uploaded to this account. |
| FILTER\_BY\_AMT\_REQD | Please enter an amount to filter by. |
| FINANCE\_CHARGE\_SET\_PREFS | Finance Charge Item cannot be edited as an item. Please go to the finance charge preferences page to make changes |
| FINANCE\_CHARGE\_SETUP\_REQD | Please set <a href='/app/setup/finchargepref.nl'>Finance Charge Preferences</a> first. |
| FIRST\_LAST\_NAMES\_REQD | Please enter both your first and last name. |
| FIRST\_QTY\_BUCKET\_MUST\_BE\_ZERO | Quantity defined for first quantity bucket must be zero |
| FLD\_VALUE\_REQD | Results are incomplete. You must provide a value for field {1}. |
| FLD\_VALUE\_TOO\_LARGE | Value for field {1} is too large to be processed. |
| FOLDER\_ALREADY\_EXISTS | A folder with the same name already exists in the selected folder. |
| FORM\_RESUBMISSION\_REQD | You have logged in to a different user since you navigated to this form. You must re-submit this form as the new user. |
| FORM\_SETUP\_REQD | No appropriate forms are enabled for this role. Please contact your Administrator. |
| FORM\_UNAVAILBL\_ONLINE | This form is not available online |
| FORMULA\_ERROR | Your formula has an error in it. It could resolve to the wrong datatype, use an unknown function, or have a syntax error. Please go back, correct the formula, and re-submit. |
| FRIENDLY\_NAME\_REQD | Missing Friendly Name. Friendly Name is a required field and it cannot be null or empty. |
| FULFILL\_REQD\_FIELDS\_MISSING | For the listed items, please edit the item record and provide values for the specified fields, and retry the fulfillment. |
| FULFILL\_REQD\_FIELDS\_MISSING | The {1} field is required to complete this fulfillment. Please return to the International tab on the item fulfillment and provide a value for the specified field and retry the fulfillment. |
| FULFILL\_REQD\_PARAMS\_MISSING | Could not perform operation '{1}' since {2} parameter was not set. |
| FULL\_DISTRIB\_REQD | You must fully distribute all {1} numbers for {1} numbered items. |
| FULL\_USERS\_REQD\_TO\_INTEGRATE | Only full {1} users can integrate with partners. |
| FX\_MALFORMED\_RESPONSE | Received malformed response from Foreign Exchange source. |
| FX\_RATE\_REQD\_FEDEX\_RATE | Cannot retrieve {1} realtime rates: {2} Exchange Rate is required when requesting {3} realtime rates. |
| FX\_TRANS\_DISALLWD | FX transactions not accepted for this account. Contact MerchantE. |
| GETALL\_RCRD\_TYPE\_REQD | The getAll record type is required. |
| GIFT\_CERT\_AMT\_EXCEED\_AVAILBL | Gift certificate redemption amount exceeds available amount on the gift certificate |
| GIFT\_CERT\_AUTH\_ALREADY\_EXISTS | Gift certificate authorization code {1} already exists |
| GIFT\_CERT\_CAN\_BE\_USED\_ONCE | A gift certificate may only be used one time on a transaction |
| GIFT\_CERT\_CODE\_REQD | Gift certificate codes are missing |
| GIFT\_CERT\_CODE\_REQD | Missing gift certificate authorization code(s). Please go back and enter authorization codes on the {1}. |
| GIFT\_CERT\_CODE\_REQD | You must specify a gift certificate code. |
| GIFT\_CERT\_IN\_USE | Another user is using gift certificate {1} |
| GIFT\_CERT\_IN\_USE | Gift certificate code {1} is already in use |
| GIFT\_CERT\_INVALID\_NUM | Gift certificate numbers may not contain the '{1}' character. |
| GROUP\_DSNT\_EXIST | That group does not exist |
| GROUP\_REQD | You cannot perform a bulk merge operation with an empty group |
| GROUP\_TYPE\_REQD | The group type is required. |
| GRTR\_QTY\_PRICE\_LEVEL\_REQD | Each quantity pricing level must be greater than the previous quantity pricing level. |
| ILLEGAL\_ID | Illegal ID. Please enter a name. |
| ILLEGAL\_PERIOD\_STRUCTURE | Illegal period structure. Date {1} is in multiple periods. |
| INACTIVE\_CC\_PROFILE | The credit card processing profile provided is inactive. |
| INACTIVE\_RCRD\_FOR\_ROLE | The record for this role has been made inactive. |
| INAVLID\_FILE\_TYP | A change has been made to this file's format. You cannot upload this type of file. |
| INAVLID\_FILE\_TYP | You attempted to upload a restricted file type. Please try again with a selection from the list below: |
| INAVLID\_ITEM\_TYP | Invalid item type \[{1}\] for item \[{2}\]. |
| INAVLID\_PRICING\_MTRX | Invalid Quantity Pricing Matrix for quantity level {1} : Quantity {2}, Base Price {3} |
| INCOMPATIBLE\_ACCT\_CHANGE | The account change you have made is incompatible with old transactions. If you need to swap two accounts, you need to do it in 3 steps. For example, to change the income and asset accounts for an item:<ul><li>(1) Change the income account to a temporary account and save</li><li>(2) Change asset account to the old income account and save</li><li>(3) Change the income to the old asset account and save</li></ul>Please contact customer support if you need assistance with this. |
| INCOMPATIBLE\_ACCT\_CHANGE | The account change you have made is incompatible with old transactions. Please either change the account selection appropriately or do not request to update past transactions. |
| INCOMPLETE\_BILLING\_ADDR | Billing address is incomplete. |
| INCOMPLETE\_FILE\_UPLOAD | The upload did not complete correctly. Please try uploading the file again. If you have repeatedly received this error message, please send mail to <a href="mailto:{1}">{2} NetSuite Customer Support</a>. |
| INCRCT\_ORD\_INFO | The order contains incorrect information and was not placed. |
| INITIALIZE\_ARG\_REQD | The initialize reference id is required. |
| INITIALIZE\_ARG\_REQD | The initialize reference type is required. |
| INITIALIZE\_ARG\_REQD | The initialize type is required. |
| INITIALIZE\_AUXREF\_REQD | The initialize auxReference type is required. |
| INSTALL\_SCRIPT\_ERROR | Installation Script Error |
| INSUFCNT\_NUM\_PRDS\_FOR\_REV\_REC | Not enough accounting periods in range specified for revenue recognition. |
| INSUFCNT\_OPEN\_PRDS\_FOR\_REV\_REC | Not enough open accounting periods available for revenue recognition. |
| INSUFFICIENT\_CHARS\_IN\_SEARCH | Global searches must contain at least three characters to prevent excessive matches. |
| INSUFFICIENT\_FLD\_PERMISSION | You are attempting to read an unauthorized field: {1} |
| INSUFFICIENT\_FLD\_PERMISSION | You cannot access this search because it includes restricted fields. Please contact your administrator. |
| INSUFFICIENT\_FUND | Decline. Insufficient funds. |
| INSUFFICIENT\_PERMISSION | For security reasons, only an administrator is allowed to edit an administrator record. |
| INSUFFICIENT\_PERMISSION | Global search is not permitted from this role. |
| INSUFFICIENT\_PERMISSION | Insufficient privileges |
| INSUFFICIENT\_PERMISSION | Your issue DB access has been inactivated. Please contact your issue DB administrator. |
| INSUFFICIENT\_PERMISSION | Your current login role does not have an associated Issue Role. Please change to a different role or contact your Issue administrator. |
| INSUFFICIENT\_PERMISSION | Only the owner can make a contact private |
| INSUFFICIENT\_PERMISSION | Only the super user can update or delete bug entries |
| INSUFFICIENT\_PERMISSION | Permission error: you may not edit this role. |
| INSUFFICIENT\_PERMISSION | Permission Violation: partners do not have access to this report. |
| INSUFFICIENT\_PERMISSION | Permission Violation: partners may not delete saved reports. |
| INSUFFICIENT\_PERMISSION | Permission Violation: You cannot delete saved reports not created by yourself. |
| INSUFFICIENT\_PERMISSION | <b>Test Drive does not allow access to this feature.</b> If you would like more information about this feature, please contact your account manager. |
| INSUFFICIENT\_PERMISSION | The restriction settings on your role deny you access to this item. |
| INSUFFICIENT\_PERMISSION | This folder does not exist or you do not have permission to access this folder. |
| INSUFFICIENT\_PERMISSION | This folder does not permit the direct addition of files |
| INSUFFICIENT\_PERMISSION | This order has been partially or fully processed and may not be edited by a user without permission to approve sales orders. |
| INSUFFICIENT\_PERMISSION | User permission level could not be established |
| INSUFFICIENT\_PERMISSION | You do not have permissions to set a value for element {1} due to one of the following reasons: 1) The field is read-only; 2) An associated feature is disabled; 3) The field is available either when a record is created or updated, but not in both cases. |
| INSUFFICIENT\_PERMISSION | Your role does not have permission to provision accounts. |
| INSUFFICIENT\_PERMISSION | You are not allowed to approve your own transactions. |
| INSUFFICIENT\_PERMISSION | You are not authorized to change this event's organizer. Public events may only have their organizer changed by administrators, the event's organizer, or delegates with edit permission to the event's calendar. Private or busy events may only have their organizer changed by the owner. |
| INSUFFICIENT\_PERMISSION | You cannot update a system defined template. |
| INSUFFICIENT\_PERMISSION | You cannot update cases using this form. |
| INSUFFICIENT\_PERMISSION | You can not access this page unless you are logged in as the consolidated parent company. |
| INSUFFICIENT\_PERMISSION | You can only delete notes that you created. |
| INSUFFICIENT\_PERMISSION | You do not have access to the activity history for that record |
| INSUFFICIENT\_PERMISSION | You do not have access to the media item you selected. |
| INSUFFICIENT\_PERMISSION | You do not have access to this page |
| INSUFFICIENT\_PERMISSION | You do not have access to this template |
| INSUFFICIENT\_PERMISSION | You do not have permission to access this list. |
| INSUFFICIENT\_PERMISSION | You do not have permission to access this register. |
| INSUFFICIENT\_PERMISSION | You do not have permission to access this type of transaction. |
| INSUFFICIENT\_PERMISSION | You do not have permission to create this type of record. Please choose a different record type. |
| INSUFFICIENT\_PERMISSION | You do not have permission to email transactions. |
| INSUFFICIENT\_PERMISSION | You do not have permission to perform this operation. |
| INSUFFICIENT\_PERMISSION | You do not have permission to print {1} |
| INSUFFICIENT\_PERMISSION | You do not have permission to view this page. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to approve commissions. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to create commissions. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to create this transaction. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to perform that operation. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to perform this action. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to perform this operation |
| INSUFFICIENT\_PERMISSION | You do not have privileges to use this page. |
| INSUFFICIENT\_PERMISSION | You do not have privileges to view this account |
| INSUFFICIENT\_PERMISSION | You do not have privileges to view this page |
| INSUFFICIENT\_PERMISSION | You may not create a new Liability Adjustment or edit existing Liability Adjustments. |
| INSUFFICIENT\_PERMISSION | You may not delete built-in audiences. |
| INSUFFICIENT\_PERMISSION | You may not delete built-in categories. |
| INSUFFICIENT\_PERMISSION | You may not delete built-in items. |
| INSUFFICIENT\_PERMISSION | You may not delete built-in tabs. |
| INSUFFICIENT\_PERMISSION | You must have either 'Transactions -> Invoice' or 'Transactions -> Cash Sale' permission to bill sales orders. |
| INSUFFICIENT\_PERMISSION | You must have either 'Transactions -> Invoice' or 'Transactions -> Cash Sale' permission to fulfill sales orders. |
| INSUFFICIENT\_PERMISSION | You must have 'Transactions -> {1}'permission to build work orders. |
| INSUFFICIENT\_PERMISSION | You must have 'Transactions -> Fulfill Sales Orders' view permission to view sales order fulfillments. |
| INSUFFICIENT\_PERMISSION | You must have 'Transactions -> Fulfill Sales Orders' edit permission to fulfill sales orders. |
| INSUFFICIENT\_PERMISSION | You need employee access to delete this record. |
| INSUFFICIENT\_PERMISSION | {1} The {2} restrictions on your role deny you access to this record. |
| INSUFFICIENT\_PERMISSION | {1} The {2} restrictions on your role prevent you from seeing this record. |
| INSUFFICIENT\_PERMISSION | {1} The customer restrictions on your partner role prevent you from seeing this record. |
| INSUFFICIENT\_PERMISSION | {1} The restrictions on your role deny you access to this record. |
| INSUFFICIENT\_PERMISSION | {1} The restrictions on your role do not allow you to modify this record. |
| INSUFFICIENT\_PERMISSION | {1} You need {2} the '{3}' permission to access this page. Please contact your account administrator. |
| INSUFFICIENT\_PERMISSION | {1} You need a higher level of the '{2}' permission to access this page. Please contact your account administrator. |
| INSUFFICIENT\_PERMISSION | {1} You need a higher permission for custom record type {2} to access this page. Please contact your account administrator. |
| INTEGER\_REQD\_FOR\_QTY | Quantity must be an integer for numbered items. |
| INTL\_FEDEX\_ONE\_PACKG\_ALLWD | International FedEx fulfillments allow only one package. If more than one package is required, please break up the shipment into multiple fulfillments of one package each. |
| INTL\_SHIP\_EXCEED\_MAX\_ITEM | The maximum number of items for FedEx International shipping has been exceeded: {1} |
| INVALID\_ABN | Invalid ABN registration number {1}. |
| INVALID\_ACCT | Invalid login. No such account. |
| INVALID\_ACCT | Invalid account number. |
| INVALID\_ACCT\_NUM\_CSTM\_FIELD | The account number custom field does not exist!! Consult billing cell. |
| INVALID\_ACCT\_PRD | You can not create an accounting period that is not a year or does not belong to a year. |
| INVALID\_ACCT\_TYP | Invalid account type \[ {1} \]. |
| INVALID\_ACCT\_TYP | There is no account of type: {1} |
| INVALID\_ACCT\_TYP | The account and its parent have different account type. |
| INVALID\_ACCT\_TYP | You cannot change an account to or from A/R or A/P |
| INVALID\_ACTION | You have attempted an unsupported action. |
| INVALID\_ADDRESS\_OR\_SHIPPER\_NO | An error has occurred. Please ensure that the address information and shipper number are correct, then resubmit the form. |
| INVALID\_ADJUSTMENT\_ACCT | The account you selected in Adjustment Account is the same as the asset account for one of the items you are adjusting. Please go back and change the account. Normally, the adjustment account would be an expense account. |
| INVALID\_AES\_FTSR\_EXEMPTN\_NUM | The AES/FTSR Exemption Number is invalid. |
| INVALID\_ALLOCTN\_METHOD | You have attempted to allocate landed costs to a transaction using an allocation method that results in no allocation for any lines in the transaction. The allocation method you chose is {1}. To correct this problem, go back to the transaction and choose a different allocation method, or modify the items/lines on the transaction so that there will be some cost allocated to the lines. |
| INVALID\_AMORTZN\_ACCT | The destination account for the amortization schedule could not be determined. |
| INVALID\_AMT | Amount applied greater than total payments and credits |
| INVALID\_AMT | Foreign currency transactions that use Revenue Commitments cannot have a non-discount line with a negative amount. Please use a non-posting discount item instead. |
| INVALID\_AMT | Amount Error (credit) Insufficient Funds (debit). Transaction amount is 0 or too long. Re-submit transaction with a valid amount. |
| INVALID\_AMT | No Action Taken (credit) PIN entry necessary (debit). Reversal amount larger then original amount. No action to take, transaction may not qualify for best level of Interchange. |
| INVALID\_AMT | Base and consumer amounts are inconsistent with the FX rate. Correct provided amounts. |
| INVALID\_APP\_ID | Invalid application id: {1} |
| INVALID\_ASSIGN\_STATUS\_COMBO | Invalid assignee/status combination({1}/{2}) |
| INVALID\_ASSIGN\_STATUS\_COMBO | Invalid assignee/status combination (assignee {1}, status {2}, issue #{3}). No default owner for issue role? |
| INVALID\_ASSIGN\_STATUS\_COMBO | Invalid assignee/status combination ({1},{2}) |
| INVALID\_AUTH | Invalid double authorization. The order is currently authorized for {1}, valid until {2}. |
| INVALID\_AUTH\_CODE | You have entered an invalid authorization code for this campaign email address. Please check the authorization code in the email message, and enter it again. |
| INVALID\_AUTOAPPLY\_VALUE | Ambiguous data: <autoApply> has been selected and lines have been selected in the <applyList> element. |
| INVALID\_AVS\_ADDR | AVS Address Length Error. Please correct the AVS Address and re-submit. |
| INVALID\_AVS\_ADDR | Invalid AVS address or zip data. Please correct the AVS data and re-submit. |
| INVALID\_AVS\_ZIP | AVS Zip Length Error. Please correct the AVS Zip and re-submit. |
| INVALID\_BALANCE\_RANGE | Your balance is not within the allowed range. |
| INVALID\_BILLING\_SCHDUL | The billing schedule definition is incompatible with this transaction. Please modify the current billing schedule or select a different one. |
| INVALID\_BILLING\_SCHDUL\_DATE | Billing schedules may not extend beyond 500 years from today |
| INVALID\_BILLING\_SCHDUL\_ENTRY | You cannot create a billing schedule with two entries on the same date. Please go back and edit the billing schedule or start date. |
| INVALID\_BIN\_NUM | Bin numbers may not contain the '{1}' character |
| INVALID\_BOM\_QTY | Inventory/Assembly quantities cannot be negative |
| INVALID\_BOOLEAN\_VALUE | Checkbox / boolean data must be either 'T' or 'F' |
| INVALID\_BUG\_NUM | Bug number specified was incorrect. ("{1}" isn't a number.) |
| INVALID\_CAMPAIGN\_CHANNEL | You cannot use this channel to setup this event |
| INVALID\_CAMPAIGN\_GROUP\_SIZE | While in {1}, you can only send {2} emails per campaign event. Please modify one or more of your target groups to contain {2} members or less. All campaign emails will be sent to your {1} login email address. |
| INVALID\_CAMPAIGN\_STATUS | You cannot set the status of this campaign event back to 'In Progress' because it already has some activity. |
| INVALID\_CARD | Missing Card Holder Account Data. Please provide valid card data and re-submit. |
| INVALID\_CARD | Card not in authorizers database. |
| INVALID\_CARD | The referencing transaction (i.e. reversal request) was not carried out with the same card as the original transaction. Re-submit with original card. |
| INVALID\_CARD\_ID | Invalid Card ID. Provide a valid card ID. |
| INVALID\_CARD\_NUM | Invalid Card Number. Please provide a valid card number and re-submit. |
| INVALID\_CARD\_NUM | Card No. Error. Card number has unknown Bank Identification Number (BIN) or fails check digit edit. Re-try card number again, verify with merchant it is a valid card with proper logos for card types the merchants accept. |
| INVALID\_CARD\_TYP | Card Type Not Accepted. Contact MerchantE to add the card type. |
| INVALID\_CARD\_TYP | Merchant doesn't accept the transaction's card type. |
| INVALID\_CASE\_FORM | You cannot create cases using this form. |
| INVALID\_CATGRY\_TAX\_AGENCY\_REQ | A Vendor must be created in a cateogry with the Tax Agency checkbox checked. |
| INVALID\_CC\_EMAIL\_ADDRESS | The email address to CC store orders to is invalid. Please go back and correct it. |
| INVALID\_CC\_NUM | Credit card numbers must contain between 13 and 20 digits. |
| INVALID\_CC\_NUM | Credit card number is not valid. Please check that all digits were entered correctly. |
| INVALID\_CC\_NUM | Credit card number must contain only digits. |
| INVALID\_CERT | Intercompany Transfer Orders cannot be entered when the _Setup > Accounting > Accounting Preferences > Order Management > Use Item Cost as Transfer Cost_ preference is enabled. |
| INVALID\_CERT | Invalid CA certificate |
| INVALID\_CERT | Invalid certificate key |
| INVALID\_CERT | Invalid certificate |
| INVALID\_CERT | Failed to verify client certificate, send email to {1} for help. |
| INVALID\_CERT\_AUTH | The indicated CA is not the issuer of this certificate |
| INVALID\_CHARGE\_AMT | Charge amount too large. This order can't be charged for more than {1} |
| INVALID\_CHARS\_IN\_EMAIL | Email address contains invalid characters. |
| INVALID\_CHARS\_IN\_NAME | The From Name field cannot contain apostrophes, quotation marks, commas, or greater than or less than signs. |
| INVALID\_CHARS\_IN\_NAME | You cannot use the colon ':' character in the topic name - please remove it . |
| INVALID\_CHARS\_IN\_PARAM\_FIELD | The Additional Parameters field can not contain any of the following characters: "?\\<>|/!@#$%^\*()+,.:;'"". Please remove them and try again |
| INVALID\_CHARS\_IN\_URL | Spaces are not allowed in the {1}url.<p>Examples of a valid {1}url are:<br><b>http://www.example.com/image.gif</b> or <b>https://one.two.org/user-name/test.jpg</b> |
| INVALID\_CHARS\_IN\_URL | The URL component you have chosen contains a space or one of the following prohibited character: &?\\<>|/!@#$%^&\*()+=,.:;'". Please remove them and try again |
| INVALID\_CHECKOUT\_EMAIL | The email address to email checkout errors to is invalid. Please go back and correct it. |
| INVALID\_CITY | Merchant City Length Error. Reduce the city name length. |
| INVALID\_COLUMN\_NAME | Invalid column name in get\_invtitem\_col\_sum\_all\_locs: {1} \[ {2} \] |
| INVALID\_COLUMN\_VALUE | An attempt was made to set a column to an invalid value. Dynamic SQL being executed \[ {1} \] |
| INVALID\_CONTENT\_TYPE | Invalid content type. You can only use application/json, application/xml or text/plain with RESTlets. |
| INVALID\_COSTING\_METHOD | SERIAL and LOT are the only costing methods that may be passed as parameters to this page. |
| INVALID\_CRNCY\_EXCH\_RATE | Invalid currency conversion rate. |
| INVALID\_CRYPT\_KEY | {1} is not a valid cryptographic key written as a hexadecimal number. |
| INVALID\_CSTM\_FIELD\_DATA\_TYP | The customfield \[{1}\] reference object does not match its data type. |
| INVALID\_CSTM\_FIELD\_RCRD\_TYP | Invalid custom field record type |
| INVALID\_CSTM\_FIELD\_REF | The specified custom field reference {1} is invalid. |
| INVALID\_CSTM\_FORM | {1} is an invalid custom form |
| INVALID\_CSTM\_RCRD\_KEY | Invalid custom record key \[{1}\]. |
| INVALID\_CSTM\_RCRD\_QUERY | Invalid custom record object in query. |
| INVALID\_CSTM\_RCRD\_TYPE\_KEY | Invalid custom record type |
| INVALID\_CSTM\_RCRD\_TYPE\_KEY | Invalid custom record type key. |
| INVALID\_CSTM\_RCRD\_TYPE\_KEY | {1} refers to a custom list. To get the contents of this list, use the 'get' or 'getAll' operation with a RecordRef of type 'customList' |
| INVALID\_CSTM\_RCRD\_TYP\_KEY | Invalid custom record type key in query. |
| INVALID\_CUR | You have entered an invalid currency symbol or internal ID: {1}. |
| INVALID\_CURR\_CODE | Failed to find a currency code for the currency symbol {1}. Verify your currency symbol is ISO-compliant and re-submit. |
| INVALID\_CURRENCY\_CODE | Failed to find currency code for the requested country code. Check country code and retry request. |
| INVALID\_CURRENCY\_CODE | Request currency code must match FX rate currency code. Retry request with a currency code that matches the FX currency code. |
| INVALID\_CURRENCY\_TYP | Currency Type Not Accepted. Contact MerchantE to add the currency type. |
| INVALID\_CUSTOMER\_RCRD | This customer record {1} is not valid. Please create the customer first. |
| INVALID\_DATA | Invalid data combination, can not set {1} to {2} and {3} to {4} |
| INVALID\_DATA\_FORMAT | Invalid data format. You should return a JavaScript object. |
| INVALID\_DATA\_FORMAT | Invalid data format. You should return TEXT. |
| INVALID\_DATE | Date Error. Invalid date. |
| INVALID\_DATE | The date < {1} > is invalid. You must specify a date after < {2} >. |
| INVALID\_DATE\_FORMAT | Date field not in your preferred date format |
| INVALID\_DATE\_RANGE | The date range you specified does not enclose all its child periods. |
| INVALID\_DATE\_RANGE | Invalid time range. The {1} "{2}" start time ({3}) must be earlier than its end time ({4}). |
| INVALID\_DATE\_RANGE | Invalid Date Range - the To Date value must be on or after the From Date value |
| INVALID\_DATE\_RANGE | The date range you specified does not fall inside that of the parent period. |
| INVALID\_DEAL\_RANGE | Invalid Deal Range - low must be less than projected and high must be greater than projected. |
| INVALID\_DEAL\_RANGE | Invalid Deal Range - low must be less than projected and high must be greater than projected. |
| INVALID\_DELETE\_REF | Either RecordRef or CustomRecordRef should be used for 'delete' operation. |
| INVALID\_DESTINATION\_FLDR | The destination folder is the same as the current folder. |
| INVALID\_DESTNTN\_COUNTRY | The destination Country is invalid or has not been set. |
| INVALID\_DESTNTN\_POST\_CODE | The destination Postal Code is invalid or has not been set. |
| INVALID\_DESTNTN\_STATE | The destination State is invalid or has not been set. |
| INVALID\_DETACH\_RECORD\_TYP | Missing or Invalid RecordType for DetachFrom. |
| INVALID\_DETACH\_RECORD\_TYP | Detaching of record type {1} from {2} is not supported. |
| INVLAID\_DISCOUNT\_MARKUP | Posting and non-posting discounts/markups are not allowed on the same transaction |
| INVALID\_DOMAIN\_KEY | The private domain key is invalid, please enter a valid private domain key. |
| INVALID\_DOMAIN\_NAME | Invalid domain name {1}, please enter a valid domain name. |
| INVALID\_DUP\_ISSUE\_REF | Cannot set this issue to be a duplicate of itself or of an issue that is a duplicate of this issue. |
| INVALID\_EMAIL | Email address is not valid. |
| INVALID\_EMAIL | Your email or code is invalid. Please try again |
| INVALID\_EMAIL | You have entered an invalid email address. Please try again. |
| INVALID\_EMAIL\_ADDR | Some of the email addresses you have entered are invalid: {1:list of invalid email addresses} |
| INVALID\_EMAIL\_ADDR | The email address for the web store is invalid. Please go back and correct it. |
| INVALID\_END\_DATE | You entered an end date ({1}) that is before the start date ({2}) |
| INVALID\_END\_DATE | {1} \[{2}\] recurrence end date is invalid |
| INVALID\_END\_TIME | invalid 'end' time |
| INVALID\_ENTITY\_INTERNALID | Attempt to insert entity with nkey -1 or 0 |
| INVALID\_ENTITY\_STATUS | You entered an invalid entity status. |
| INVALID\_EVENT\_TIME | You cannot make the time that close to the start or end of the day, because it shifts the event across a day boundary. |
| INVALID\_EXP\_DATE | Invalid expiration date. Please correct the expiration date and re-submit. |
| INVALID\_EXPNS\_ACCT\_SUB | The expense account associated with expense category '{1:expense category}' is not available in the subsidiary of customer '{2:customer}'. |
| INVALID\_EXPRESSION | ERROR: Invalid Expression |
| INVALID\_FAX\_NUM | The Fax Number is invalid. |
| INVALID\_FAX\_PHONE\_FORMAT | Invalid FaxPhoneNumber. The format of FaxPhoneNumber must contain area code plus seven digit number. |
| INVALID\_FIELD\_FOR\_RCRD\_TYP | Record type {1} does not support field {2} |
| INVALID\_FIELD\_NAME\_FOR\_NULL | The specified name \[{1}\] must exactly match an existing field name. |
| INVALID\_FILE | Verify that you have a valid file to upload. |
| INVALID\_FILE\_ENCODING | The file encoding: {1} is not valid. Please refer to the documentation for a list of supported file encodings. |
| INVALID\_FILE\_TYP | Invalid file type. File is not a compressed/zip file. |
| INVALID\_FILE\_TYP | Invalid file type. File is not a compressed zip file. |
| INVALID\_FILE\_TYP | The media file type you uploaded was not recognized. Please try again. |
| INVALID\_FLD | ERROR: Field Not Found |
| INVALID\_FLD\_RANGE | Value outside of valid min/max range for this field |
| INVALID\_FLD\_TYPE | Application error: NLField of type {1} is not supported. |
| INVALID\_FLD\_VALUE | You have entered an Invalid Field Value {1} for the following field: {2} |
| INVALID\_FLDR\_SIZE | Error in update\_folder\_size |
| INVALID\_FORMAT\_IN\_PARAM\_FIELD | The Additional Parameters field is not formatted correctly. Please reformat and try again |
| INVALID\_FORMULA | Your formula contains a reference to an encrypted field. This is not allowed. |
| INVALID\_FORMULA | Your formula could result in a divide by zero error. Please go back, correct the formula and resumbit. |
| INVALID\_FORMULA\_FIELD | Your formula has an unrecognized field in it. Please go back and correct the formula and resubmit. |
| INVALID\_FROM\_DATE | invalid 'from' date |
| INVALID\_FROM\_TIME | invalid 'from' time |
| INVALID\_FULFILMNT\_ITEM | You have an invalid item {1} in the fulfillment request. |
| INVALID\_FX\_BASE\_CURRENCY | FX amount in base currency is required. Provide the base amount. |
| INVALID\_FX\_RATE | Exchange Rate must be 1 for vendors in your currency. |
| INVALID\_GET\_REF | Either RecordRef or CustomRecordRef should be used for 'get' operation. |
| INVALID\_GIFT\_CERT | Invalid gift certificate |
| INVALID\_GIFT\_CERT\_AMT | The remaining amount on a gift certificate can not be negative |
| INVALID\_GIFT\_CERT\_CODE | Gift certificate code must contain only letters and digits. |
| INVALID\_GROUP\_TYP | This type of group cannot be defined based on another group of the same type. |
| INVALID\_GROUP\_TYP | You cannot define this group type using this search. |
| INVALID\_GROUP\_TYPE | The group type {1} is invalid. |
| INVALID\_GRP | This type of group cannot be defined based on another group. |
| INVALID\_GST\_PST\_AGENCIES | The GST or PST agencies are not valid. Please review your company preferences |
| INVALID\_ID | No order found with id {1} |
| INVALID\_ID | Identifiers can contain only digits, alphabetic characters, or "\_" with no spaces |
| INVALID\_ID | You have provided an invalid script id or internal id: {1} |
| INVALID\_ID | The externalId attribute is not supported for {1} |
| INVALID\_INITIALIZE\_ARG | The reference type {1} and initialize type {2} are not matched. |
| INVALID\_INITIALIZE\_ARG | InitializeRef should be used for 'initialize' operation. |
| INVALID\_INITIALIZE\_AUXREF | Invalid initialize operation argument 'auxReference'. |
| INVALID\_INITIALIZE\_REF | You can not initialize {1}: invalid reference {2}. |
| INVALID\_INITIALIZE\_REF | Can not initialize customerPayment: invalid customer reference {1}. |
| INVALID\_INITIALIZE\_REF | Can not initialize customerPayment: invalid invoice reference {1}. |
| INVALID\_INITIALIZE\_REF | You have an invalid sales order {1} or the order is already billed |
| INVALID\_INITIALIZE\_REF | You have an invalid sales order {1} or the order is already closed. |
| INVALID\_INSURED\_VALUE | The Insured Value cannot exceed the total sum of the items being shipped. |
| INVALID\_INTERNAL\_ID | The specified internal id is not allowed. |
| INVALID\_INTERNALID | Unparseable Internal Id, did you mean to lookup this field by Name or External ID? |
| INVALID\_INV\_DATE | Invoice date on billing schedule may not be after {1} |
| INVALID\_INVENTORY\_NUM | Invalid set of inventory numbers: values must be separated by commas, spaces, tabs, or line feeds. |
| INVALID\_INV\_DATE | Invoice date on billing schedule may not be after {1} |
| INVALID\_IP\_ADDRESS\_RULE | The following IP Address rule is not valid: {1} |
| INVALID\_ISSUE\_BUILD\_VERSION | Cannot set issue {1} to {2} {3} and {4} {5} because that version is not associated with that build. |
| INVALID\_ISSUE\_PRIORITY | Severity 1 issues must have priority 1. |
| INVALID\_ISSUE\_PRODUCT | Cannot set issue {1} to {2} {3} and {4} {5} because that product is not associated with that build. |
| INVALID\_ISSUE\_PRODUCT | Cannot set issue {1} to {2} {3} and {4} {5} because that product is not associated with that module. |
| INVALID\_ISSUE\_STATUS | Cannot set issue {1} to status {2} and assignee {3} because that status requires an assignee with issue role {4}. |
| INVALID\_ITEM\_OPTION | Invalid item option {1} for item {2} |
| INVALID\_ITEM\_OPTIONS | The options for item '{1}' are no longer available. Please change your order and try again. |
| INVALID\_ITEM\_SUBTYP | Invalid item subtype \[{1}\] for item \[{2}\]. |
| INVALID\_ITEM\_TYP | The item \[{1}\] does not have a valid item type. |
| INVALID\_ITEM\_WEIGHT | The total item weight must be > 0.0 |
| INVALID\_JOB\_ID | You have specified an invalid Job Id |
| INVALID\_KEY\_OR\_REF | The specified key is invalid. |
| INVALID\_KEY\_OR\_REF | Invalid {1} reference key {2}. |
| INVALID\_KEY\_OR\_REF | Invalid {1} reference key {2} for {3} {4}. |
| INVALID\_KEY\_PASSWORD\_REQD | This key is invalid or may require a password |
| INVALID\_LINE\_ID | No line items match the entered id(s) {1}. |
| INVALID\_LINK\_SUM | Links sum to more than applied transaction amount |
| INVALID\_LINK\_SUM | Links sum to more than original transaction amount |
| INVALID\_LIST\_ID | You must specify a valid line ID. Please set {1}. |
| INVALID\_LIST\_KEY | Could not perform operation ''{1}'' on an invalid line \[{2}\]. |
| INVALID\_LIST\_KEY | Could not perform operation 'add' on an existing line \[{1}\]. |
| INVALID\_LOC | Item Fulfillment/Item Receipt location does not match the location on the Transfer Order |
| INVALID\_LOC\_SUB\_RESTRICTN | You may not add inventory to a location that is incompatible with the subsidiary restrictions for this item. |
| INVALID\_LOGIN | Invalid login. Online Form access is disabled. |
| INVALID\_LOGIN | Invalid login. Supplier access is disabled. |
| INVALID\_LOGIN\_ATTEMPT | Invalid login attempt. |
| INVALID\_LOGIN\_CREDENTIALS | A problem occured verifying the presented email address, password, roleName or account number, please verify these pieces of information and try again |
| INVALID\_LOGIN\_CREDENTIALS | You have entered an invalid email address or account number. Please try again. |
| INVALID\_LOGIN\_CREDENTIALS | You have entered an invalid email address or password. Please try again. |
| INVALID\_LOGIN\_CREDENTIALS | You have entered an invalid login password. Please try again. |
| INVALID\_LOGIN\_CREDENTIALS | You have entered an invalid password. Please try again. |
| INVALID\_LOGIN\_IP | Invalid login. IP Address does not match any of the IP Address rules specified for this entity. |
| INVALID\_LOT\_NUM\_FORMAT | Lot numbers must be entered using this format: LOT#(Quantity).nFor example, to enter a quantity of 100 items as Lot number ABC1234, enter "ABC1234(100)" in the Lot Numbers field. |
| INVALID\_ MACRO\_ID | The Macro ID: {1} is not valid! Please refer to the documentation for a list of supported macro IDs. |
| INVALID\_MARKUP\_DISCOUNT | Markup/Discount % must be between -999% and 999% |
| INVALID\_MCC | Merchant Category Code Length Error. Provide a valid MCC. |
| INVALID\_MEMBER\_HIERARCHY | You have defined a group/kit/assembly item that contains a loop in the member hierarchy. You must remove any group/kit/assembly member items that contain this item as a member. |
| INVALID\_MEMRZD\_TRANS | A memorized transaction may not contain any serial or lot numbers. Go back, remove the numbers, and try to re-Memorize the transaction. Posting transactions such as Bills or Cash Sales may not use serial or lot numbered items. Non-Posting transactions such as Purchase Orders or Sales Orders may use serial or lot numbered items but may not contain serial or lot numbers. |
| INVALID\_MERCHANT\_KEY | Merchant key is not supplied or incorrect. |
| INVALID\_MERCHANT\_NAME | Merchant Name Length Error. Reduce the merchant name length. |
| INVALID\_NAME | Invalid savepoint name. Must start with an alphabet character and can only contain alphanumeric, underscore, dollar, and hash characters. |
| INVALID\_NEXUS | Transaction Nexus is incorrect: it is {1} but should be {2} |
| INVALID\_NUM | Invalid Decimal Number |
| INVALID\_NUMBER | Invalid Decimal Number |
| INVALID\_NUMBER | Invalid Integer |
| INVALID\_NUMBER | Invalid integer {1} |
| INVALID\_NUMBER | Invalid number {1} |
| INVALID\_NUMBER | You entered "{1}" into a field where a numeric value was expected. Please go back and change this value to a number. |
| INVALID\_NUMBER | You entered an invalid number: <br>Go <a href="javascript:history.go(-1);";>back</a>, change this value and resubmit. |
| INVALID\_OBJ | There are no objects of this type |
| INVALID\_ONLINE\_FORM | Online Form not found |
| INVALID\_ONLINE\_FORM | This online form is inactive or not available online. |
| INVALID\_ONLINE\_FORM\_URL | You cannot submit Online forms from this URL. Use the live version: {1} instead |
| INVALID\_OPENID\_DOMAIN | This is not a valid domain. Please go back and enter your domain name without prefixes such as 'http://' or 'www'. |
| INVALID\_OPERATION | That operation is not supported for this record type: {1} |
| INVALID\_ORD\_STATUS | This order has been partially or fully processed and may not be reset to 'Pending Approval'. |
| INVALID\_ORIGIN\_COUNTRY | The origin Country is invalid or has not been set. |
| INVALID\_ORIGIN\_POSTCODE | The origin Postal Code is invalid or has not been set. |
| INVALID\_ORIGIN\_STATE | The origin State is invalid or has not been set. |
| INVALID\_PAGE\_INDEX | Job {1} does not have a page {2} |
| INVALID\_PAGE\_PARAM | Invalid page parameter. Unable to view page. |
| INVALID\_PAGER\_NUM | The Pager Number is invalid. |
| INVALID\_PARAM | Please select either {1} or {2} parameter but not both. |
| INVALID\_PARENT | An account cannot be its own parent |
| INVALID\_PARTNER\_CODE | An account for this customer cannot be provisioned unless its partnercode ({1}) is empty or numeric. |
| INVALID\_PARTNER\_ID | Invalid partner id: {1} |
| INVALID\_PASSWORD | Invalid key password |
| INVALID\_PAYCHECK\_DATE | Paychecks for {1} must be on or after {2} |
| INVALID\_PERIOD | A period may be only an adjustment period, a quarter, or a year. |
| INVALID\_PHONE | The phone number of the {1} address is invalid. Please verify the phone number is correctly formatted and includes the area code. |
| INVALID\_PHONE\_FAX\_PAGER\_NUM | The Phone, Fax, or Pager Number is invalid. |
| INVALID\_PHONE\_NUM | The Phone Number is invalid. |
| INVALID\_PICKUP\_POSTAL\_CODE | An error has occurred. Pickup Postal Code {1} is not the postal code associated with Shipper Number {2}. |
| INVALID\_PIN | Incorrect PIN. PIN number may have been entered incorrectly. Re-submit with proper PIN. |
| INVALID\_PIN\_DEBIT\_TRANS\_TYP | Invalid pin debit transaction type. Only a sale (D) is supported. |
| INVALID\_PORTLET\_TYP | unsupported portlet type \[{1}\], id \[{2}\] processed by cardMetaDataGenerator |
| INVALID\_POST | Invalid Post |
| INVALID\_PRESENTATION\_TYP | Presentation Type not recognized |
| INVALID\_PROBABILITY\_RANGE | Probability must be between 0 and 100. |
| INVALID\_PROFILE\_ID | Invalid Profile ID or Profile Key. Correct the profile ID and profile key, and re-submit. |
| INVALID\_PROJ\_BILLING\_TYP | The project billing type is incompatible with the billing schedule on the transaction. Please select a different billing schedule. |
| INVALID\_PST\_TAX\_VALUE | PST tax value is not a valid number: {1} |
| INVALID\_PSWD | Email address "{1}" has been previously registered under a different password from the new password you just provided. For security reasons, you will first need to go back and supply the correct new password for "{1}" to merge the accounts. |
| INVALID\_PSWD | Invalid Password. The password must be between 6 and 10 character with at least one numeric and one alphabetic character. |
| INVALID\_PSWD | Password must be at least 6 characters long. |
| INVALID\_PSWD | Password must be at least 6 characters long and contain at least one number or special character. |
| INVALID\_PSWD | Password must contain at least one letter (A-Z). |
| INVALID\_PSWD | Password must contain at least one number or special character. |
| INVALID\_PSWD | The current password you supplied is incorrect. |
| INVALID\_PSWD | Your new password must be at least {1} characters, contain at least one non-letter, and be substantially different from the current password. |
| INVALID\_PSWD | Your new password must be at least 6 characters, contain at least one non-letter, and be substantially different from the current password. |
| INVALID\_PSWD | Your password cannot be the same as your login. Please choose a new password. |
| INVALID\_PSWD | Your password must be at least 6 characters |
| INVALID\_PSWD | You've used that password before. Please choose a new password. |
| INVALID\_PSWD\_HINT | Your hint is too similar to your password. Please choose something less obvious. |
| INVALID\_PSWD\_ILLEGAL\_CHAR | Password contains an illegal character. |
| INVALID\_PURCHASE\_TAX\_CODE | Purchase tax code not defined properly for item |
| INVALID\_QTY | The new quantity and new value must be either both positive or both negative. |
| INVALID\_QTY | You may not receive a larger quantity than you shipped. |
| INVALID\_QUANTITY | Serial and lot number quantities must be integers |
| INVALID\_QUANTITY | Serial and lot number quantities must be positive. |
| INVALID\_QUESTION | Please select a different question. |
| INVALID\_QUESTION | Please select a question. |
| INVALID\_RCRD | Invalid record specification: {1} |
| INVALID\_RCRD\_CONVERSION | Only customer records can be converted to child or parent records. Please select only customer records for this duplicate merge operation. |
| INVALID\_RCRD\_HEADER\_ | Invalid record header: Unable to parse field name from {1} |
| INVALID\_RCRD\_HEADER\_ | Invalid record header: Unable to parse record id from {1} |
| INVALID\_RCRD\_HEADER\_ | Invalid record header: Unable to parse record type from {1} |
| INVALID\_RCRD\_ID | Invalid id {1} to create a record. |
| INVALID\_RCRD\_INITIALIZE | You have entered an invalid default value for this record initialize operation. |
| INVALID\_RCRD\_OBJ | You do not have a valid record object. |
| INVALID\_RCRD\_REF | Invalid RecordRef internalId {1} for field {2} |
| INVALID\_RCRD\_REF | Invalid record reference. |
| INVALID\_RCRD\_REF | Invalid record reference |
| INVALID\_RCRD\_TRANSFRM | You have entered an invalid default value for this record transformation operation. |
| INVALID\_RCRD\_TRANSFRM | That type of record transformation is not allowed. Please see the documentation for a list of supported transformation types |
| INVALID\_RCRD\_TRANSFRM | That is not a valid record transformation. |
| INVALID\_RCRD\_TYPE | Invalid Record Type |
| INVALID\_RCRD\_TYPE | {1}: type argument {2} is not a valid record or is not available in your account. Please see the documentation for a list of supported record types. |
| INVALID\_RCRD\_TYPE | The record type \[{1}\] is invalid. |
| INVALID\_RCRD\_TYPE | The record type is invalid. |
| INVALID\_RECIPIENT | Recipient internal id does not match an existing entity. |
| INVALID\_RECR\_REF | Could not update {1} to {2} because referenced record does not exist |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its duration is either negative or longer than one day. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its end-by date is before its start date. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its end time and duration do not match. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its end time is more than one day after its start time. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its end time is not after its start time. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its start time or end time/duration is empty. {1} |
| INVALID\_RECUR\_DATE\_RANGE | This event recurrence is invalid because its times are not in order. {1} |
| INVALID\_RECUR\_DESC\_REQD | This event recurrence is invalid because it has no description. {1} |
| INVALID\_RECUR\_DOW | This event recurrence has an invalid day-of-week field. {1} |
| INVALID\_RECUR\_DOWIM | This event recurrence has an invalid day-of-week-in-month value. {1} |
| INVALID\_RECUR\_DOWMASK | This event recurrence is invalid because its day-of-week mask is not 7 characters long. {1} |
| INVALID\_RECUR\_FREQUENCY | This event recurrence has an invalid frequency. {1} |
| INVALID\_RECUR\_PATTERN | This event does not have a valid recurrence pattern. |
| INVALID\_RECUR\_PATTERN | This event recurrence is invalid because it is not a monthly or yearly event and it has day-of-week and day-of-week-in-month field values. {1} |
| INVALID\_RECUR\_PATTERN | This event recurrence is invalid because it only has one recurrence time and it must have either none or at least two. {1} |
| INVALID\_RECUR\_PATTERN | This event recurrence is invalid because one of its times is out of the range 0 to 86399. {1} |
| INVALID\_RECUR\_PATTERN | This event recurrence is invalid because only one of the day-of-week and day-of-week-in-month fields is set. Both must be set or both must be unset. {1} |
| INVALID\_RECUR\_PATTERN | This event recurrence is invalid either because it is not weekly and it has a day-of-week mask, or it is weekly and it has no day-of-week mask. {1} |
| INVALID\_RECUR\_PATTERN | This single day event is invalid since it contains a recurrence pattern. |
| INVALID\_RECUR\_PERIOD | This event recurrence has an invalid period. {1} |
| INVALID\_RECUR\_TIME\_ZONE\_REQD | This event recurrence in invalid because it has no time zone. {1} |
| INVALID\_REF\_CANT\_INITIALIZE | Cannot initialize customerRefund: invalid creditMemo reference {1}. |
| INVALID\_REF\_CANT\_INITIALIZE | Cannot initialize customerRefund: invalid customer reference {1}. |
| INVALID\_REF\_CANT\_INITIALIZE | You can not initialize {1} by referencing {2}. |
| INVALID\_REF\_KEY | Invalid externalId {1}. |
| INVALID\_REF\_KEY | Invalid reference key \[{1}\]. |
| INVALID\_REFFERER\_EMAIL | The refferer email address you have entered is not valid. Please try again. |
| INVALID\_REFUND\_AMT | Refund amount must be between zero and the original amount. Correct amount and retry request. |
| INVALID\_REFUND\_AMT | The amount you can refund is {1} because the the order has already been refunded for {2} |
| INVALID\_REPORT | The referenced Report and Row are no longer valid, because the layout containing them has changed. Please edit this reference row to reselect Report and Row. |
| INVALID\_REPORT\_ID | Invalid report ID. |
| INVALID\_REPORT\_ROW | Invalid Reference Row |
| INVALID\_REPORT\_ROW | Invalid Report Row Reference |
| INVALID\_REQUEST | invalid request (failed isValid() check). Email request handler unable to service request for address= <{1}> . |
| INVALID\_RESOURCE\_TIME | Total resource time for '{1}' cannot exceed {2} planned time entries. |
| INVALID\_RESULT\_SUMMARY\_FUNC | The result field {1} cannot be grouped. Please edit the search and omit this field or use a different summary function. |
| INVALID\_RETURN\_DATA\_OBJECT | The return value of the RESTlet function cannot be used to create a well-formed XML document. |
| INVALID\_RETURN\_DATA\_OBJECT | The XML document does not contain a root element because the RESTlet function does not return a JavaScript Object. |
| INVALID\_REV\_REC\_DATE\_RANGE | Rev rec end date can not be before rev rec start date. |
| INVALID\_ROLE | The specified role is invalid. |
| INVALID\_ROLE | Your role does not give you permission to view this page. |
| INVALID\_ROLE\_FOR\_EVENT | You seem to have been invited to this {1} in a different role. Please change your role to view the {1}. |
| INVALID\_RQST\_CONTACTS\_EXIST | it has associated primary contacts. |
| INVALID\_RQST\_PARENT\_REQD | it has associated contact records that would be left with no parent company. |
| INVALID\_RQST\_SBCUST\_JOBS\_EXIST | it has associated sub-customers or jobs. |
| INVALID\_SAVED\_SRCH | Missing or invalid saved search for Custom KPI. The search must have a date column as an available filter. Please see help next to Custom KPI dropdown list on KPI setup page. |
| INVALID\_SAVEDSEARCH | A saved search with the internal ID {1} does not exist. |
| INVALID\_SAVEDSEARCH | We cannot return search columns for summary saved search {1}. |
| INVALID\_SCHDUL\_AMT | The total amount on the schedule must equal the sum of the individual recognition amounts. |
| INVALID\_SCHDUL\_AMT | The total amount on the schedule must be equal to the amount of the source transaction line. |
| INVALID\_SCHDUL\_FORMAT | To create a valid schedule, please enter the bracket values in ascending orders without gaps. |
| INVALID\_SCRIPT\_ID | A saved search with the script ID {1} does not exist. |
| INVALID\_SEARCH | That search or mass update does not exist. |
| INVALID\_SEARCH | You may search by {1} or {2} but not both |
| INVALID\_SEARCH\_CRITERIA | Can't search transactions: invalid cross reference key |
| INVALID\_SEARCH\_CRITERIA | Global Search supports at most three keywords and requires at least one. Keywords are composed of only letters, digits, and dashes. |
| INVALID\_SEARCH\_FIELD\_KEY | search field keys are not consistent({1}/{2}) |
| INVALID\_SEARCH\_FIELD\_NAME | search field names are not consistent({1}/{2}) |
| INVALID\_SEARCH\_FIELD\_OBJ | {1} is not a valid search custom field |
| INVALID\_SEARCH\_FIELD\_OBJ | {1} must be used to search custom field {2} |
| INVALID\_SEARCH\_FIELD\_OBJ | Server application error: invalid search customfield object. |
| INVALID\_SEARCH\_FIELD\_OBJ | Invalid search field object: {1} |
| INVALID\_SEARCH\_JOIN\_ID | Invalid Search Join ID |
| INVALID\_SEARCH\_MORE | Invalid searchMore operation. Please make sure that you have had a successful search operation before you can perform any searchMore operation. |
| INVALID\_SEARCH\_OPERATOR | You need to provide a valid search field operator. |
| INVALID\_SEARCH\_OPERATOR | You can not use this operator '{1}' for internalId search. |
| INVALID\_SEARCH\_PAGE\_INDEX | Invalid search page index. |
| INVALID\_SEARCH\_PAGE\_SIZE | Invalid search page size. |
| INVALID\_SEARCH\_PREF | You cannot set returnSearchColumns to false while you specify search columns. |
| INVALID\_SEARCH\_PREF | You cannot set returnSearchColumns to true without specifying search columns or referencing a saved search. |
| INVALID\_SEARCH\_SELECT\_OBJ | Invalid search select field object: {1} |
| INVALID\_SEARCH\_VALUE | You need to provide a search value. |
| INVALID\_SEARCH\_VALUE | You need to provide search values. |
| INVALID\_SECONDARY\_EMAIL | Invalid secondary email address. The email address must be in a valid format. |
| INVALID\_SECPAY\_CREDENTIALS | The username or password used to process the transaction with SECPay was not valid. Please make sure you have entered the correct username, password, and remote password in your SECPay account setup. |
| INVALID\_SERIAL\_NUM | No items match the entered serial number |
| INVALID\_SERIAL\_OR\_LOT\_NUMBER | Serial and lot numbers may not contain the '{1}' character. |
| INVALID\_SESSION | A valid NLSession is required to generate record xml |
| INVALID\_SESSION | A valid session is required. Please log in first. |
| INVALID\_SHIP\_DATE | The Future Ship Date is invalid. Please verify the entered Future Ship Date is no more than 7 days in the future, and resubmit the fulfillment. |
| INVALID\_SHIP\_FROM\_STATE | The Ship From State/Province Code is missing or invalid. Please enter the 2 to 5 character abbreviation for the state or province of the address that contains it. |
| INVALID\_SHIP\_GRP | You cannot add shipping groups when creating a transaction that has multiple shipping routes enabled. You must first add the items, then get the transaction and update the shipping groups separately. |
| INVALID\_SHIP\_SRVC | The selected service is not valid for international shipments. Please choose an international service and retry your request. |
| INVALID\_SHIP\_TO\_SATE | The Ship To State/Province Code is missing or invalid. Please enter the 2 to 5 character abbreviation for the state or province of the address that contains it. |
| INVALID\_SHIPPER\_STATE | The Shipper State/Province Code is missing or invalid. Please enter the 2 to 5 character abbreviation for the state or province of the address that contains it. |
| INVALID\_SITE\_CSTM\_FILE | File is not a NetSuite site customization export file: it cannot be imported. |
| INVALID\_SOAP\_HEADER | Invalid SOAP Header: '{1}'. Value is '{2}'. |
| INVALID\_SRCH | That search or mass update does not exist (internal id={1}) |
| INVALID\_SRCH\_CRITERIA | The field rule value "{1}" is invalid for field type {2} with criterion "{3}." |
| INVALID\_SRCH\_CSTM\_FLD | This search refers to custom field with id = {1} which either is restricted or is not applied to this record type. |
| INVALID\_SRCH\_FUNCTN | An nlobjSearchColumn contains an invalid function: {1}. |
| INVALID\_SRCH\_SORT | An nlobjSearchColumn that is not sortable contains a sort specification: {1}. |
| INVALID\_SRCH\_SUMMARY\_TYP | An nlobjSearchFilter contains an invalid summary type: {1}. |
| INVALID\_SRCH\_TYP | Search Type not allowed as standalone search |
| INVALID\_SRVC\_ITEM\_SUB | The service item '{1:service item}' is not available in the subsidiary of customer '{2:customer}'. |
| INVALID\_SSO | Invalid SuiteSignOn reference: {1}. That SuiteSignOn object does not exist or has been marked as inactive. |
| INVALID\_SSS\_DEBUG\_SESSION | You have exceeded the maximum allowable idle time for debugging scripts. To debug another script, simply reload the script debugger page and start a new debugging session. |
| INVALID\_SSS\_DEBUG\_SESSION | You have canceled your current script debugging session. |
| INVALID\_STATE | Merchant State Length Error. Provide a valid state. |
| INVALID\_STATE | Signup prospect state '{1}' is invalid. |
| INVALID\_STATUS | You may not change this issue''s status from ''{1}'' to ''{2}''. |
| INVALID\_SUB | The subsidiary restrictions on this record are incompatible with those defined for account: {1}. Subsidiary access on this record must be a subset of those permitted by the account. |
| INVALID\_SUB | The subsidiary restrictions on this record are incompatible with those defined for account: {1}. Subsidiary access on this record must be a superset of those permitted by the account. |
| INVALID\_SUB | The subsidiary restrictions on this record are incompatible with those defined for department: {1}. Subsidiary access on this record must be a subset of those permitted by the department. |
| INVALID\_SUB | The subsidiary restrictions on this record are incompatible with those defined for item: {1}. Subsidiary access on this record must be a superset of those permitted by the item. |
| INVALID\_SUB | The subsidiary restrictions on this record are incompatible with those defined for location: {1}. Subsidiary access on this record must be a subset of those permitted by the location. |
| INVALID\_SUB | The Subsidiary selected doesnt match the bank account selected. |
| INVALID\_SUB | This record does not support multiple subsidary restrictions. You must choose a single subsidiary. |
| INVALID\_SUB | Transaction references multiple subsidiaries |
| INVALID\_SUB | You may not add members to a group/kit/assembly unless the subsidiaries for those members completely contain the subsidiaries of the group/kit/assembly. |
| INVALID\_SUB | {1} can not be used with the selected subsidiary |
| INVALID\_SUBLIST\_DESC | Invalid sublist description - all sublists must appear exactly as they do in the WSDL (eg end with 'List') |
| INVALID\_SUBSCRIPTION\_STATUS | You cannot change the global subscription status from its current value of {1:status name}. |
| INVALID\_SUBSCRIPTION\_STATUS | You cannot set the global subscription status to the value {1:status name}. |
| INVALID\_SUMMARY\_SRCH | In a summary search, you must sort by a result field with a summary function. Please go back and correct the sort by field on the results tab. |
| INVALID\_SUPERVISOR | Employees can not be their own supervisor. |
| INVALID\_SUPERVISOR | You can't insert this employee record as it would create a loop in the supervisor hierarchy. |
| INVALID\_TASK\_ID | The task ID: {1} is not valid. Please refer to the documentation for a list of supported task IDs. |
| INVALID\_TASK\_ID | You have specified an invalid task Id |
| INVALID\_TAX\_AMT | Invalid tax amount. Correct tax amount and retry request. |
| INVALID\_TAX\_CODE | Invalid Canadian Tax Code: {1} |
| INVALID\_TAX\_CODE\_FOR\_SUB | The selected tax code is not available in subsidiary. |
| INVALID\_TAX\_CODES | Invalid Tax Code(s): {1} |
| INVALID\_TAX\_PMT | You may not commit tax payment information prior to the start date of the Payroll Service. |
| INVALID\_TAX\_VALUE | GST and PST amount cannot be negative! |
| INVALID\_TAX\_VALUE | GST tax value is not a valid number: {1} |
| INVALID\_TIME\_FORMAT | {1} is not a valid time and it should use the following format h:mm a. |
| INVALID\_TO\_DATE | invalid 'to' date |
| INVALID\_TRACKING\_NUM | The tracking number is not valid. |
| INVALID\_TRACKING\_NUM | You have entered a tracking number that exceeds the maximum size of {1} characters: {2}. Multiple tracking numbers must be separated by spaces, tabs, or commas. Slash (/), semicolon (;), colon (:), or any other character that is not a space or a comma will be interpreted as a part of the tracking number. |
| INVALID\_TRAN\_ITEM\_LINE | Item {1} can not be included on the {2} because it is not distributed as of the transaction date |
| INVALID\_TRANS | This transaction is not valid. |
| INVALID\_TRANS\_COMPNT | You have entered an invalid component for this transaction. |
| INVALID\_TRANS\_ID | Invalid Transaction ID. Correct the transaction ID, then re-submit. |
| INVALID\_TRANS\_ID | Only sale transactions can be refunded. Provide a valid transaction ID. |
| INVALID\_TRANS\_SUB\_ACCT | Transaction subsidiary {1} is not valid for account {2}. Please choose a different account. |
| INVALID\_TRANS\_SUB\_CLASS | Transaction subsidiary {1} is not valid for class {2}. Please choose a different class. |
| INVALID\_TRANS\_SUB\_DEPT | Transaction subsidiary {1} is not valid for department {2}. Please choose a different department. |
| INVALID\_TRANS\_SUB\_ENTITY | Transaction subsidiary {1} is not valid for entity {2}. Please choose a different entity. |
| INVALID\_TRANS\_SUB\_ITEM | Transaction subsidiary {1} is not valid for item {2}. Please choose a different item. |
| INVALID\_TRANS\_SUB\_LOC | Transaction subsidiary {1} is not valid for location {2}. Please choose a different location. |
| INVALID\_TRANS\_TYP | Transaction type specified is incorrect. |
| INVALID\_TRANSACTIO\_DATE | There are no Accounting Periods that cover this transaction date. |
| INVALID\_TRANSACTION\_DATE | Transaction date {1} is not valid. Transaction dates may be at most {2} years in the past and {3} years in the future. |
| INVALID\_TRIAL\_TYP | The trialtype is not availabe in the product specified. |
| INVALID\_TYP | Invalid type {1}, use {2} |
| INVALID\_UNIT\_TYP | On serialized items, you may not choose a units type that has fractional conversion rates. |
| INVALID\_UNSUPRTD\_RCRD\_TYP | Invalid or unsupported record type: {1} |
| INVALID\_UPS\_ACCT | An invalid UPS Account Number was entered. Please verify you have entered the correct Shipper Number and re-submit the form. |
| INVALID\_UPS\_PACKG\_WEIGHT | UPS requires a minimum package weight of .1 LBS and a maximum package weight of 150 LBS. Please adjust the package weights accordingly and resubmit the fulfillment. |
| INVALID\_UPS\_VALUES | UPS did not accept the entered values for the following fields. Please go back and correct these values: |
| INVALID\_URL | Please begin the {1} url with <b>http://</b> or <b>https://</b><p>Examples of a valid {1}url are:<br><b>http://www.example.com/image.gif</b> or <b>https://one.two.org/user-name/test.jpg</b> |
| INVALID\_URL | Request for invalid URL: {1} |
| INVALID\_URL\_PARAM | Error: URL param {1}="{2}" - expected an integer. |
| INVALID\_VALUE | You have entered an invalid value {1} for {2}. |
| INVALID\_VAT\_AMOUNT | VAT amount cannot be negative |
| INVALID\_VAT\_REGSTRTN\_NUM | Invalid VAT registration number {1}. |
| INVALID\_VSOE\_ALLOCTN | VSOE allocations must be greater than or equal to 0 |
| INVALID\_WEBSITE\_SECTION | The Web site section you entered does not exist. |
| INVALID\_WO | You have an invalid work order {1} or the order is already closed. |
| INVALID\_WO\_ITEM | Special Work Order Items can not be Drop Ship or Special Order |
| INVALID\_WORLDPAY\_ID | Exchange source does not recognize your WorldPay ID. Please check that it is correct. |
| INVALID\_WS\_VERSION | The async operation has been submitted through different endpoint version: {1}. |
| INVALID\_YEAR | Invalid year {1} |
| INVALID\_YEAR\_FORMAT | Illegal year format or value. Examples: 1999, 2000, 2001, etc. |
| INVALID\_ZIP\_CODE | Merchant Zip Length Error. Provide a valid 5 digit zip. |
| INVALID\_ZIP\_FILE | Invalid archive. Zip file must contain at least one file. |
| INVALID\_ZIP\_POST\_CODE | The submitted Zip/Postal Code is invalid. This field may only contain a maximum of 16 digits, spaces, and the dash character (-). |
| INVENTORY\_NUM\_DISALLWD | Inventory numbers are only allowed on items with serial numbered or lot numbered items. |
| INVLAID\_BOOLEAN\_VALUE | You have entered an invalid boolean value. Please use true, false, T, or F for boolean values and resubmit your import. |
| IP\_REQUEST | Your IP address {1} does not match any of the ipaddress rules specified for this account. |
| ISSUE\_ASSIGNEE\_DISALLWD | The specified assignee is disallowed for this issue's status. |
| ISSUE\_PRODUCT\_VERSION\_MISMATCH | Cannot set issue {1} to {2} {3} and {4} {5} because that product is not associated with that version. |
| ISSUE\_VERSION\_BUILD\_MISMATCH | Issue version and build do not match. |
| ITEM\_ACCT\_REQD | One of the items on this transaction has an amount but no account. Please fix the item and resubmit the transaction. |
| ITEM\_ACCT\_REQD | One of the items on this transaction has an amount but no account. Please fix the item and resubmit the transaction. It might be that you have recently elected to charge for shipping and have not assigned an account to the shipping item that is included in this transaction. |
| ITEM\_ACCT\_REQD | You must specify asset and COGS accounts for this inventory item. |
| ITEM\_COUNT\_MISMATCH | COGS\_CORRECTION: 2 means of calculating the item count do not match for item: {1} vs {2}) |
| ITEM\_COUNT\_MISMATCH | COGS\_CORRECTION: 2 means of calculating the item count do not match for item: {1} vs {2}) There are transactions in the system in which this item is used but the asset account for that item is not the current Asset Account in the item record |
| ITEM\_IS\_UNAVAILABLE | (Item is unavailable) |
| ITEM\_NAME\_MUST\_BE\_UNIQUE | An item with that name already exists. Please choose another name |
| ITEM\_NOT\_UNIQUE | The item \[{1}\] is not unique. |
| ITEM\_PARAM\_REQD\_IN\_URL | Error - Item parameter (id=nnn) was not provided on the URL |
| ITEM\_QTY\_AMT\_MISMATCH | Inventory and assembly items cannot have zero quantity and non-zero amount. |
| ITEM\_TYP\_REQS\_UNIT | Items of type {1} require {2} unit |
| ITEM\_TYP\_REQS\_UNIT | Items of type {1} subtype {2} require {3} unit |
| JE\_AMOUNTS\_MUST\_BALANCE | The amounts in the journal entry must balance. |
| JE\_LINE\_MISSING\_REQD\_DATA | {1} are mandatory on all lines of the journal entry. |
| JE\_MAX\_ONE\_LINE | Journal Entries can have a maximum of {1} lines. |
| JE\_REV\_REC\_IN\_PROGRESS | This account is currently processing Revenue Recognition Journal Entries. Only one such process is allowed at a time. |
| JE\_UNEXPECTED\_ERROR | Journal Entries failed to be created due to unexpected error. |
| JOB\_NOT\_COMPLETE | The specified job is not complete yet |
| JS\_EXCEPTION | A JavaScript Exception was thrown |
| KEY\_REQD | Empty key not allowed for {1} |
| KPI\_SETUP\_REQD | Please enable the Forecast ({1}) & Quota KPIs |
| KPI\_SETUP\_REQD | Please enable the Forecast & Quota KPIs |
| KPI\_SETUP\_REQD | please enable the Sales & Forecast KPIs |
| KPI\_SETUP\_REQD | Please enable the Sales & Forecast ({1}) KPIs |
| KPI\_SETUP\_REQD | Please enable the Sales & Quota KPIs |
| LABEL\_REQD | Please enter a value for Label |
| LANGUAGE\_SETUP\_REQD | Please go to company preference to add language to translate. |
| LINK\_LINES\_TO\_ONE\_ORD | Lines on this record can only be linked to a single order. |
| LINKED\_ACCT\_DONT\_MATCH | You are attempting to link transaction line items, but items on the lines do not match. This can happen when you create a fulfillment from a sales order, a receipt from a purchase order, an invoice from a sales order, a vendor bill from a purchase order, or a reimbursement from a purchase. Please verify that items in the transaction you are creating match the items in the originating transaction. |
| LINKED\_ENTITIES\_DONT\_MATCH | You are attempting to link transactions, but the entities on the transactions do not match. |
| LINKED\_ITEMS\_DONT\_MATCH | Linked items don't match |
| LIST\_ID\_REQD | Required field missing in a related list. You must set {1}. |
| LIST\_KEY\_REQD | There is no list key for field {1} of list {2}. Please assign a key and resubmit your task. |
| LOCATIONS\_IN\_USE | Your classes cannot be converted to locations because your existing location records are referred to by transactions or other records. These location records cannot be overwritten. |
| LOCATIONS\_SETUP\_REQD | You must first define locations (Lists->Locations->New) before you can distribute inventory. |
| LOCATIONS\_SETUP\_REQD | You must first define locations (Lists->Locations->New) before you can transfer inventory. |
| LOCATION\_REQD | You must specify a location to use {1} numbers when Multi-Location Inventory is enabled |
| LOCKED\_DASHBOARD | Your dashboard has been set up and locked by an administrator. Please contact them for details. |
| LOGIN\_DISABLED | Invalid login. Customer access is disabled. |
| LOGIN\_DISABLED | Login access has been disabled for this role. |
| LOGIN\_DISABLED | Your access to {1} has been deactivated. Please contact the company's administrator to re-activate your access. |
| LOGIN\_DISABLED | Your access to this account has been removed or disabled. Please contact the account adminstrator. |
| LOGIN\_DISABLED\_PARTNER\_CTR | Disabled login: Advanced Partner Center access has been disabled by the account administrator. |
| LOGIN\_DISABLED\_PARTNER\_CTR | Disabled login: Standard Partner Center access has been disabled by the account administrator. |
| LOGIN\_EMAIL\_REQD | Invalid login. You must provide an email address. |
| LOGIN\_NAME\_AND\_PSWD\_REQD | Please enter both a user name and a password. |
| LOGIN\_REQD | You must <a href='/pages/login.jsp' target='\_self'>log in</a> before accessing this page. |
| LOST\_UPSELL\_CRITERIA | Your upsell criteria were lost. This is probably due to a transient condition such as a server reboot. Click <a href=# onclick='history.go(-1);'>here</a> to go back and try again. |
| MACHN\_LIST\_KEY\_NAMES\_REQD | Server application error: no list key names are defined for field {1} of record of type {2}. |
| MANDATORY\_PRD\_TYPE\_REQD | Please select the mandatory period type... |
| MASS\_UPDATE\_CRITERIA\_LOST | Your mass update criteria were lost. This is probably due to a transient condition such as a server reboot. Click <a href=# onclick='history.go(-1);'>here</a> to go back and try again. |
| MATCHING\_CUR\_SUB\_REQD | The parent specified must have the same currency and subsidiary as the child |
| MATCHING\_SERIAL\_NUM\_REQD | The serial numbers on a transfer order receipt must have been fulfilled |
| MATRIX\_INFO\_TEMP\_LOST | Matrix item information was lost. This was probably due to a transient condition like a server reboot. Please try again. |
| MATRIX\_SUBITEM\_NAME\_TOO\_LONG | The following matrix sub-item name is too long (80 character max):<p> {1} <p> Please shorten your parent item name or your option abbreviations. |
| MAX\_200\_LINES\_ALLWD\_ON\_TRANS | Journal Entries can have a maximum of 200 lines. |
| MAX\_BARCODE\_PRINT\_EXCEEDED | A maximum of {1} barcodes can be printed at a time. |
| MAX\_BULK\_MERGE\_RCRDS\_EXCEEDED | You cannot perform a bulk merge operation with a group larger than {1} records |
| MAX\_EMAILS\_EXCEEDED | This campaign email event exceeds the number of emails ({1}) that can be sent per month without setting up a default campaign domain or specifying one on the campaign email template. |
| MAX\_EMAILS\_EXCEEDED | This merge operation exceeds the number of emails ({1}) that can be sent per month without setting up a bulk merge domain or specifying one on the email template. |
| MAX\_RCRDS\_EXCEEDED | The maximum number ( {1} ) of records allowed for a {2} operation has been exceeded. |
| MAX\_VALUES\_EXCEEDED | Too many values specified for a MultiSelectField, the maximum is 1000 |
| MEDIA\_FILE\_INVALID\_JSCRIPT | Media file was of type javascript and would not compile. Error on line: |
| MEDIA\_NOT\_FOUND | Media item not found {1} |
| MEDIA\_NOT\_INITIALIZED | Media Item cannot be initialized |
| MEMORIZED\_TRANS\_ERROR | failed retrieving 'chargeit' record from trancard while processing memorized tran |
| MEMORIZED\_TRANS\_ERROR | A failure occurred while trying to enter one of your automated memorized transactions. The reason for this failure is shown in the description field on this page. Because of the failure, the system has changed this memorized transaction from an automated one to a reminder. You may click the link above to view the memorized transaction in question and make any needed changes to it. When you are done with the changes, click Memorize and then Cancel. This will modify your existing memorized transaction rather than creating a new one. When filling out the Memorized Transaction Form, you may choose to select 'Automatic' to resume automated posting of this transaction. |
| MERGE\_OPERATION\_DISALLWD | You cannot perform merge operations on records that belong to your group. |
| MERGE\_RCRD\_REQD | You must specify a record to merge into |
| MISMATCH\_EVENT\_ISSUE\_STATUS | Event status ({1}) and issue base status ({2}) do not match |
| MISMATCH\_ISSUE\_PRODUCT\_VERSION | Issue product and version do not match. |
| MISMATCH\_SALES\_CONTRIBUTION | Sales team sales rep total does not equal 100%, {1} sales reps, {2} total contribution. |
| MISMATCHED\_CURRENCY | The transaction currency does not match the names currency |
| MISMATCHED\_QTY\_PRICING | Quantities do not match across pricings. |
| MISMATCHED\_SEARCH\_PARENTHESIS | Search error: Parentheses are unbalanced. |
| MISSING\_ACCT\_PRD | You are attempting to create an amortization or revenue recognition schedule outside the range of available accounting periods. Please adjust the periods on this transaction or go to Setup>Accounting>Manage Accounting Periods to set up more periods. |
| MISSING\_CRNCY\_EXCH\_RATE | No currency conversion rate defined |
| MISSING\_ENUM | No Enumerated Value {1} for Enumerated Type {2} |
| MISSING\_REQD\_FLD | Missing required value for mandatory field: {1} |
| MISSING\_REQD\_FLD | The Company record does not have all required fields set. Please ensure the State, Zip/Postal Code, and Country fields are set and try your request again. |
| MISSNG\_ACCT\_PRD | Unable to find an Accounting Period for the allocation date. |
| MISSNG\_REV\_REC\_RCRD | Unable to locate Revenue Recognition records. |
| MISSNG\_SO\_REV\_REC\_PARAMS | Unable to get Revenue Recognition parameters from originating sales order. |
| MISSNG\_SO\_START\_END\_DATES | Unable to acquire start and end date from Sales Order. |
| MLI\_REQD | Multi-location Inventory Error (MLI\_LOCATION\_REQUIRED): this transaction or its items must have locations. |
| MLTPLE\_TAX\_LINES\_DISALLWD | Multiple Tax lines for line item in transaction: |
| MSNG\_FIELD\_OWRTE\_MUST\_BE\_TRUE | The missingFieldOverwrite attribute must be true when updating a salesOrder. |
| MST\_UPDATE\_ITEMS\_THEN\_RATES | You cannot update items and shipping rates at the same time on transactions that have multiple shipping routes enabled. You must first update the items, then get the transaction and update the shipping rates separately. |
| MULTI\_ACCT\_CANT\_CHANGE\_PSWD | The password cannot be changed here because the email address is associated with multiple accounts. The user must change their password via the link in the settings portal of the home page. |
| MULTI\_LOC\_INVT\_ERROR | Multi-Location Inventory Error: You may not create an Assembly Build transaction with an assembly item that has not been distributed and member items that have been distributed. You must create an Inventory Distribution transaction for the assembly item before building it. You also may not create an Assembly Build transaction on a date prior to the distribution date of the assembly but after the distribution date of any of the member items. |
| MULTI\_PRIMARY\_PARTNER\_DISALLWD | You are not allowed to select multiple primary partners. |
| MULTI\_SHIP\_ROUTES\_REQD | {1} {2} has multiple shipping routes enabled, which is only supported in version 2008\_2 and newer. You are not allowed to update any shipping fields on this record. |
| MULTISELECT\_TYPE\_REQD | Server application error: no multiselect type is defined for field {1} of {2} record type. |
| MUST\_DEFINE\_BASE\_UNIT | One unit must be designated as the base unit. |
| MUST\_RESUBMIT\_RCRD | Configuration changes have been made to your account. You must resubmit your record. |
| NAME\_ALREADY\_IN\_USE | A mass update has already been saved with that name. Please use a different name. |
| NAME\_ALREADY\_IN\_USE | A search has already been saved with that name. Please use a different name. |
| NAME\_REQD | Missing Name. Name is a required field and it cannot be null or empty. |
| NAME\_TYPE\_FLDR\_FIELDS\_REQD | missing required fields : name, type, and folder |
| NARROW\_KEYWORD\_SEARCH | Please provide more detailed keywords so your search does not return too many results. |
| NEED\_BILL\_VARIANCE\_ACCT | Bill variance account is missing |
| NEGATIVE\_PAYMENT\_DISALLWD | Negative payments not allowed |
| NEGATIVE\_TAX\_RATE\_DISALLWD | A Tax rate cannot be negative |
| NEW\_CONNECTION\_DISALLWD | Not allowed to create new connections. |
| NEXUS\_REQD | No tax agency defined for subsidiary: subsidiary {1} is not linked to nexus {2} |
| NO\_DATA\_FOUND | No data was found |
| NO\_EXPENSES\_FOR\_PRD | The Allocation sources or destinations did not have any expenses associated with them for the selected period. |
| NO\_ITEMS\_TO\_PRINT | There are no items to print |
| NO\_MASS\_UPDATES\_RUNNING | There are currently no mass updates running. |
| NO\_MTRX\_ITEMS\_TO\_UPDATE | There are no matrix subitems to update. |
| NO\_ORD\_SHPMNT | There is no shipment on that order. |
| NO\_RCRD\_FOR\_USER | There is no record for this user in the company's entity table. (emaillogin.semail='{1}', kentity={2}) |
| NO\_RCRDS\_MATCH | No Records matched your request. |
| NO\_SCHDUL\_APPLIED | There were no schedules that need to applied to the particular period. |
| NO\_SCHDUL\_APPLIED | There were no schedules that need to be applied to the input accounting period. |
| NON\_ADMIN\_CANNOT\_INITIATE\_LINK | This user cannot integrate with a partner. |
| NONMATCHING\_EMAILS | Email addresses don't match |
| NONUNIQUE\_INDEX\_VALUE | An attempt was made to insert a row with a non-unique index value. Dynamic SQL being executed \[ {1} \] |
| NONZERO\_AMT\_REQD | You did not enter non-zero amounts for any accounts. |
| NONZERO\_QTY\_REQD | Build quantity must be greater than zero. |
| NONZERO\_WEIGHT\_REQD | Selected service must have a weight greater than zero. |
| NOT\_AN\_INVITEE | You are not on the invitee list for event. |
| NOT\_IN\_INVT | You may not distribute {1} numbers that are not currently in inventory. You attempted to distribute the following {1} numbers that were not in inventory: {2} |
| NULL\_CHECK\_NUMBER | Null Check Number |
| NUM\_ITEMS\_GRTR\_THAN\_QTY | The number of {1} entered ({2}) is greater than the item quantity ({3}) |
| NUM\_ITEMS\_NOT\_EQUAL\_TO\_QTY | The number of {1} entered ({2}) is not equal to the item quantity ({3}) |
| NUM\_REQD\_FOR\_FIRST\_LABEL | No number was specified for the first label. |
| NUMERIC\_CHECK\_NUM\_REQD | Invalid Check Number. Check number must be a numeric value and can be at most 7 digits long. |
| NUMERIC\_REF\_NUM\_REQD | Reference Number Must Be Numeric. Please provide a valid number and re-submit. |
| OI\_FEATURE\_REQD | You have not enabled Outlook Integration feature for your account. |
| OI\_PERMISSION\_REQD | You do not have permission to access Outlook Integration feature. |
| ONE\_ADMIN\_REQD\_PER\_ACCT | This operation would leave your account without an active Administrator. To successfully perform the mass update, please deselect at least one entity with an Administrator role. |
| ONE\_ADMIN\_REQD\_PER\_ACCT | You can't delete this employee. No administrators for this account would remain. |
| ONE\_ADMIN\_REQD\_PER\_ACCT | You can't inactivate {1}. The account would be left with no active administrators. |
| ONE\_ADMIN\_REQD\_PER\_ACCT | You can't remove the administrator role from this user. No administrators for this account would remain. |
| ONE\_EMPL\_REQD | At least one employee is required to process payroll |
| ONE\_PAY\_ITEM\_PER\_EMPL | An employee may not have multiple instances of payroll items. Go <a href="javascript:history.go(-1);";>back</a>, remove these items and resubmit. |
| ONE\_POSITIVE\_VALUE\_REQD | You must enter at least one positive value for at least one item. |
| ONE\_RCRD\_REQD\_FOR\_MASS\_UPDATE | Please create at least one {1} before using this mass update. |
| ONE\_ROLE\_REQD | You can't inactivate all roles. You would not be able to log in. |
| ONLINE\_BANK\_FILE\_REQD | You must first upload an Online Bank file before using the Online Bank Statement. |
| ONLINE\_FORM\_DSNT\_EXIST | This online form does not exist. |
| ONLINE\_FORM\_EMPTY | The online form you requested is empty. |
| ONLINE\_FORM\_ID\_REQD | Missing required online form ID |
| ONLINE\_FORM\_USER\_ACCESS\_ONLY | This form is only accesible to online form users. |
| ONLINE\_ORD\_FEATURE\_DISABLED | Can't open store for {1}. This company does not have the <b>Use Sales Orders</b> feature enabled. The feature is required for customers to make online purchases. |
| ONLY\_ONE\_CONTRIB\_ITEM\_REQD | Only one instance of a company contribution item is allowed on an employee record. |
| ONLY\_ONE\_DEDCT\_ITEM\_REQD | Only one instance of a deduction item is allowed on an employee record. |
| ONLY\_ONE\_DISTRIB\_ALLWD | You may not distribute {1} numbers more than one time. You attempted to distribute the following {1} numbers more than one time: {2} |
| ONLY\_ONE\_EARNING\_ITEM\_REQD | Only one instance of an earning item is allowed on an employee record. |
| ONLY\_ONE\_LOT\_NUM\_ALLWD | You may not enter more than a single serial/lot number before an item is selected. |
| ONLY\_ONE\_PREF\_BIN\_ALLWD | There may be at most one preferred bin per location for an item. The following location has more than one preferred bin for this item: {1} |
| ONLY\_ONE\_PREF\_BIN\_ALLWD | You may not have more than one preferred bin per item. |
| ONLY\_ONE\_UNIT\_AS\_BASE\_UNIT | Only one unit may be designated as the base unit. |
| ONLY\_ONE\_UPLOAD\_ALLWD | You cannot upload more than one file at a time |
| ONLY\_ONE\_WITHLD\_ITEM\_REQD | Only one instance of a withholding item is allowed on an employee record. |
| OPENID\_DOMAIN\_IN\_USE | This domain is already in use by another NetSuite account, and a domain cannot be used by multiple accounts. |
| OPENID\_NOT\_ENABLED | The OpenID Single Sign-on feature is not enabled in this account. |
| OPRTN\_UNAVAILBL\_TO\_GATEWAY |  |
| ORD\_ALREADY\_APPRVD | You cannot cancel this order because it has already been approved. |
| ORD\_UNAVAILBL\_TO\_FULFILL | This order is not available for fulfillment. The current Google Order Financial State is {1} |
| ORDER\_DSNT\_EXIST | That order does not exist. |
| OTHER\_PMT\_AUTH\_IN\_PROGRESS | Another payment authorization is currently in progress for this order. Pleaase try again in a few minutes. |
| OVER\_FULFILL\_DISALLWD | You can not over-fulfill an item unless you have selected the 'Allow Overage on Item Fulfillments' preference. |
| OVER\_FULFILL\_RECEIV\_DISALLWD | Transfer orders can not be overfulfilled or overreceived |
| OVERAGE\_DISALLWD | Overage is not allowed. |
| OVERLAPPING\_PRDS\_DISALLWD | Illegal period structure. Overlapping periods. |
| OVERLAPPING\_PRDS\_DISALLWD | There is an overlapping period. Please check your Active or Inactive Periods to ensure that there is not an existing period. |
| OWNER\_REQD | You cannot make a contact private without an owner |
| PACKAGE\_WEIGHT\_REQD | Attempted to create a package without specifying a nonzero package weight. |
| PACKG\_LEVEL\_REF\_DISALLWD | Package level reference numbers are not allowed for shipments whose origin/destination pair is not US/US or Puerto Rico/Puerto Rico. |
| PACKG\_VALUE\_TOO\_LARGE | Package declared value cannot be greater than $999.00 USD |
| PARENT\_CANT\_ITSELF\_BE\_MEMBER | Parent item can not be a member of itself |
| PARENT\_MUST\_BE\_MATRIX\_ITEM | A Child matrix item's parent must be a matrix item |
| PARENT\_REQD | A Child matrix item must have its parent specified |
| PARSING\_ERROR | Unable to parse value into the correct type. Problem occured on record type: {1}, internalid: {2}, field : {3}, value: {4} |
| PARTIAL\_FULFILL\_RCEIV\_DISALLWD | Transfer orders can not be partially fulfilled or partially received |
| PARTNER\_ACCESS\_DENIED | Partners do not have access to this item. |
| PARTNER\_ACCT\_NOT\_LINKED | Account ({1}) from partner ({2} is not linked. |
| PARTNER\_CODE\_ALREADY\_USED | A partner with that partner code ({1}) already exists. |
| PAY\_HOLD\_ON\_SO | This sales order cannot be fulfilled because it has a payment hold. |
| PAYCHECK\_ALREADY\_PAID | You are trying to edit a paycheck that is already paid by direct deposit. A paycheck cannot be edited after funds have been processed by the Automated Clearing House (ACH). |
| PAYCHECK\_IN\_USE | You cannot clear this paycheck because it is linked to by one or more liability payments. You must delete or void those transactions first |
| PAYPAL\_FUND\_SOURCE\_REQD | Please return to PayPal to select a different funding source. |
| PAYPAL\_INVALID\_PMT\_METHOD | Paypal is unable to process this payment. Please select an alternate payment method. |
| PAYPAL\_INVALID\_PMT\_METHOD | Your PayPal account is not configured to use Express Checkout. Please follow directions on the PayPal payment method record. |
| PAYPAL\_PMT\_NOTIFICATION | PayPal Payment Notification |
| PAYPAL\_SETUP\_REQD | The account referenced by this paypal id is not setup to use express checkout. Please return to the paypal setup page and follow directions for setting up paypal express checkout. |
| PAYROLL\_COMMITTED | You are trying to edit a paycheck reversal that is in a committed Payroll Batch. |
| PAYROLL\_COMMITTED | You are trying to edit a paycheck that is in a committed Payroll Batch. |
| PAYROLL\_COMMITTED | You are trying to modify a committed payroll batch or a document on a committed payroll batch. |
| PAYROLL\_EXPENSE\_ACCT\_REQD | Please select an expense account for payroll item <a href='/app/common/item/payrollitem.nl?id={1}&e=T'>{2}</a> |
| PAYROLL\_EXPENSE\_ACCT\_REQD | Please select a expense account for payroll item <a href='/app/common/item/payrollitem.nl?id={1}&e=T'>{2}</a> |
| PAYROLL\_FEATURE\_DISABLED | You have not enabled the Payroll feature. |
| PAYROLL\_FEATURE\_UNAVAILABLE | You are trying to edit a Pay Cheque - Payroll is not available in NetSuite Canada. |
| PAYROLL\_IN\_PROCESS | A payroll process is currently running in this account. Please try again in a few minutes. |
| PAYROLL\_ITEM\_DELETE\_DISALLWD | Unable to remove payroll item: {1} - There are existing transactions for this payroll item. You may mark it inactive instead. |
| PAYROLL\_LIABILITY\_ACCT\_REQD | Please select a liability account for payroll item <a href='/app/common/item/payrollitem.nl?id={1}&e=T'>{2}</a> |
| PAYROLL\_MAINTENANCE | The Payroll feature in your account is undergoing routine maintenance from {1} Pacific Time on {2} to {3} Pacific Time on {4}. We apologize for any inconvenience this causes you. |
| PAYROLL\_SETUP\_REQD | The default payroll expense account is missing.<br>Please go to Setup -> Payroll -> Set Up Payroll and set the default payroll expense account. |
| PAYROLL\_SETUP\_REQD | You are trying to create a paycheck before your payroll setup is complete. Please complete your payroll setup. |
| PAYROLL\_SETUP\_REQD | You are trying to process payroll before your payroll setup is complete. Please complete your payroll setup. |
| PAYROLL\_UPDATE\_REQD | You made changes that require you to update your payroll information. Click <a href="https://docs.oracle.com/app/payroll/managepayroll.nl">here</a> to commit updates to the payroll service. |
| PERMISSION\_VIOLATION | Permission Violation: you may not access this record. |
| PERMISSION\_VIOLATION | Permission Violation: you may no longer edit this record. |
| PHONE\_NUM\_REQD | Please provide a phone number. |
| PIN\_DEBIT\_TRANS\_DISALLWD | Non-USD pin debit transactions are not supported. PINNED Debit for USD transactions only. |
| PLAN\_IN\_USE | This plan has already been used to generate commission calculations and can't be deleted. |
| PLAN\_OVERLAP\_DISALLWD | Plan overlap is not permitted. You have attempted to assign someone to this plan for a time period that overlaps with another plan. |
| PMT\_ALREADY\_APPRVD | The payment has already been approved and sent to the bill pay carrier for processing. |
| PMT\_ALREADY\_EXISTS | A payment with the same amount and date already exists for this payee. |
| PMT\_EDIT\_DISALLWD | Access to this Bill Pay transaction is restricted, and it cannot be modified. Transactions can only be modified until 3PM CST on the payment date. |
| POSITIVE\_BIN\_QTY\_REQD | Bin quantities must be positive or zero. |
| POSITIVE\_QTY\_REQD | Assembly member items must have positive quantities |
| POSITIVE\_UNITCOST\_REQD | Lines cannot have a negative unit cost. |
| POSTING\_DISCOUNT\_DISALLWD | Posting Discounts are not allowed on lines with Revenue Recognition Schedules. |
| POSTING\_PRD\_SETUP\_REQD | Creation of Journal Entries require a single Accounting Period value across all Revenue Recognition events. Please setup a 'Posting Period' filter. |
| PRDS\_DISALLWD\_NAMES\_NOT\_UNIQUE | After adding new periods, not all names would be unique. |
| PRD\_SETUP\_REQD | You must change your period definitions to contain fiscal years. Please visit 'Setup->Manage Accounting Periods' and click 'Set Up Year'. |
| PRD\_SETUP\_REQD | You must define the periods of the prior fiscal year. Please visit 'Setup->Manage Accounting Periods' and click 'Set Up Year'. |
| PRDS\_DISALLWD\_NAMES\_NOT\_UNIQUE | After adding new periods, not all names would be unique. |
| PREF\_VENDOR\_COST\_REQD | Drop ship/Special Order items must have a preferred vendor and a purchase price. |
| PREF\_VENDOR\_REQD | Drop ship/Special Order items must have a preferred vendor for each of the {1} the item is accessible to. |
| PREFERRED\_TAX\_AGENCY\_REQD | A preferred Tax Agency has been deleted - Please choose a new one in <a href="https://docs.oracle.com/app/setup/acctsetup.nl";>Set Up Accounting</a> |
| PREFERRED\_TAX\_AGENCY\_REQD | Error: No preferred Tax Agencies have been set up (go to <a href='/app/setup/acctsetup.nl';>Set Up Accounting</a>) |
| PRIVATE\_RCRD\_ACCESS\_DISALLWD | You cannot view or edit this record because it is marked private |
| PRIVATE\_STATUS\_CHNG\_DISALLWD | You cannot make this contact private. |
| PSWD\_EXPIRED | Password has expired. Please change your NetSuite password before continuing. |
| PSWD\_REQD | A password must be entered when granting login access privileges to this record. |
| PSWD\_REQD | Password is empty. |
| PSWD\_REQD | Please type your password into both fields. |
| PSWD\_REQD | You must provide a password to give this person access to your account. |
| PWSDS\_DONT\_MATCH | New passwords don't match. |
| PWSDS\_DONT\_MATCH | The passwords you entered do not match. Please reenter your passwords. |
| PWSDS\_DONT\_MATCH | The Passwords you entered do not match. Please reenter your passwords. |
| PWSDS\_DONT\_MATCH | The passwords you have entered do not match. |
| QTY\_EXCEEDED\_QTY\_BUCKETS | More quantities defined than there are quantity buckets |
| QTY\_REQD | Quantities must be defined |
| RATE\_REQUEST\_SHPMNT\_REQD | The rate request shipment value has not been set. |
| RATE\_SRVC\_UNAVAILBL | The rate for this service is not available for the specified source and destination addresses. |
| RCRD\_DELETED\_SINCE\_RETRIEVED | Items you have requested in the record have been deleted since you retrieved the form |
| RCRD\_DELETED\_SINCE\_RETRIEVED | The record has been deleted since you retrieved it. |
| RCRD\_DSNT\_EXIST | Group Record Not Found |
| RCRD\_DSNT\_EXIST | That record does not exist.{1} |
| RCRD\_DSNT\_EXIST | There are no records of this type. |
| RCRD\_EDITED\_SINCE\_RETRIEVED | The record has been edited since you retrieved it. Hit the back button and click Refresh/Reload to retrieve the updated record, then resubmit your changes. |
| RCRD\_HAS\_BEEN\_CHANGED | Record has been changed |
| RCRD\_ID\_NOT\_INT | Record id is not integer: {1} |
| RCRD\_LOCKED\_BY\_WF | This record has been locked by a user defined workflow. |
| RCRD\_NOT\_FOUND | Could not find any records by this name. |
| RCRD\_PREVSLY\_DELETED | This record has already been deleted. |
| RCRD\_PREVSLY\_DELETED | This record has been deleted since the list was generated. |
| RCRD\_REF\_RCRD\_TYP\_MISMATCH | The record type and its object reference are not matched. |
| RCRD\_SUB\_MISMATCH\_WITH\_CLASS | The subsidiary restrictions on this record are incompatible with those defined for class: {1}. Subsidiary access on this record must be a subset of those permitted by the class. |
| RCRD\_TYPE\_REQD | The record type is required. |
| RCRD\_UNEDITABLE | That record is not editable. |
| REACHED\_LIST\_END | You have reached the end of the list. |
| REACHED\_LIST\_START | You have reached the start of the list. |
| REC\_TYP\_REQD | You must provide either standard or custom record type information. |
| RECALCING\_PLAN\_SCHDUL | Cannot inactivate a plan when schedules in the plan are recalculating. Try again when recalculation is complete. |
| RECUR\_EVENT\_DISALLWD | A yearly event cannot be on the 29th of February |
| RECURSV\_REF\_DISALLWD | ERROR: Recursive Reference |
| REPORT\_EXPIRED | Your report request has expired. A newly created report definition will normally expire after 15 minutes of inactivity unless the definition is saved. Click back to the report definition page and re-submit your report request. |
| REQD\_FORM\_TAG\_MISSING | Your HTML template file is missing some mandatory fields or a form tag. Please make the changes to the form and try again |
| REQD\_FORM\_TAG\_MISSING | Your Online HTML Form template is missing a required closing FORM tag |
| REQD\_FORM\_TAG\_MISSING | Your Online HTML Form template is missing one or more of the required following required tags: <HTML>, <HEAD> |
| REQD\_FORM\_TAG\_MISSING | Your Online HTML template is missing the required form tag for the main form: <NLFORM> |
| REQD\_LOC\_FIELDS\_MISSING | Location {1} does not have all required fields set. Please ensure the State, Zip/Postal Code, and Country fields are set and try your request again. |
| REQD\_SUB\_FIELDS\_MISSING | The Subsidiary {1} does not have all required fields set. Please ensure the State, Zip/Postal Code, and Country fields are set and try your request again. |
| REQUEST\_PARAM\_REQD | This request is missing a required parameter. |
| REV\_REC\_DATE\_REQD | No Revenue Recognition Start Date Specified |
| REV\_REC\_TMPLT\_DATA\_MISSING | One or more line items on this transaction have Variable Revenue Recognition Templates, but do not have the required {1} also populated. Please either change the Template for these items or indicate which {1} will be used to schedule the recognition of revenue. |
| REV\_REC\_UPDATE\_DISALLWD | Modification of revenue recognition related information on this item is not allowed because revenue has been recognized for this or related lines. |
| REVERSAL\_DATE\_WARNING | Reversal Date is in a closed accounting period. Please go to Manage Accounting Periods and re-open the accounting period. |
| ROLE\_REQD | Please specify a role to which access should be granted |
| ROLE\_REQUIRED | To login, a role is required unless a default has been previously set. |
| ROUNDING\_DIFF\_TOO\_BIG | rounding difference too big -> tax1: {1} /tax2: {2} |
| ROUNDING\_ERROR | Rounding Error: {1} |
| ROUTING\_NUM\_REQD | Missing Routing Number. Bank routing number is a required field and it cannot be null or empty. |
| SALES\_DISCOUNT\_ACCT\_REQD | Please set the Sales Discount Account Preference |
| SAME\_ACCT\_TYP\_REQD\_FOR\_PARENT | Parent acccount must be of same account type. |
| SAVED\_SRCH\_EMAIL\_ERROR | E-mail Alert Failure using saved search '{1}'. Reason: {2} |
| SCHDUL\_EDIT\_DISALLWD | This schedule cannot be edited as it has already been used for commission calculations. Please go back and select 'save as new' instead. |
| SCHEDULED\_REPORT\_ERROR | NetSuite encountered an error while trying to generate your scheduled report. |
| SCHEDULED\_REPORT\_ERROR | NetSuite encountered an error while trying to generate your scheduled report. Please click {1}here{2} to notify NetSuite Support. |
| SCHEDULED\_REPORT\_ERROR | NetSuite encountered an error while trying to generate your scheduled report. This error most likely occurred because the query was too large. To run this report successfully, try using filters, or select a different date/period range to narrow the query. |
| SCHEDULED\_REPORT\_ERROR | NetSuite encountered an error while trying to generate your scheduled report. This error most likely occurred because the query was too large. To run this report successfully, try using filters, or select a different date/period range to narrow the query. If you continue to encounter errors, please click {1}here{2} to notify NetSuite Support. |
| SEARCH\_DATE\_FILTER\_REQD | The search must have a date column as an available filter |
| SEARCH\_ERROR | Unable to search - Unexpected error in search engine. |
| SEARCH\_INTEGER\_REQD | Please enter an integer number to search on. |
| SEARCH\_TIMED\_OUT | Your search has timed out. If your search includes the '{1}' operator, try using '{2}' instead. If your search includes broad search criteria, try narrowing the criteria. |
| SEARCH\_TIMED\_OUT | Your search has timed out. This might be avoided by using a smaller page size. |
| SECURE\_TRANS\_REQD\_ON\_CHECKOUT | Store Server Error: As configured, this server does not permit secure transactions, required by store checkout. |
| SERIAL\_NUM\_MATCH\_MULTI\_ITEMS | {1} different items match this serial number. Select an item from the item dropdown list. |
| SESSION\_TERMD\_2ND\_LOGIN\_DECTD | You can have a maximum of {1} active users at a time in {2}. If you would like to add active users, please contact your account manager to discuss your upgrade options. Or, you may choose to inactivate an existing user before adding a new one. Note that Employee Center users are not included in this total |
| SESSION\_TERMD\_2ND\_LOGIN\_DECTD | You can have a maximum of {1} active users at a time that are enabled for Offline Sales Client. If you would like to add active users, please contact your account manager to discuss your upgrade options. Or, you may choose to disable Offline Sales Client on an existing user before enabling a new one. |
| SESSION\_TIMED\_OUT | Your connection has timed out. Please log in again. |
| SESSION\_TIMED\_OUT | Your connection has timed out. Please <a href='/pages/login.jsp' target='\_self'>log in</a> again. |
| SESSION\_TIMED\_OUT | Your session has timed out. Please re-enter your information and try again. |
| SESSION\_TIMED\_OUT | Your session has timed out. Please re-print the document(s). |
| SET\_SHIPPING\_PICKUP\_TYP | Please verify that you have selected a pickup type under setup shipping. |
| SETUP\_METER\_REQD | Please set up this meter |
| SHIP\_ADDR\_REQD | Shipping address is incomplete. |
| SHIP\_MANIFEST\_ALREADY\_PRCSSD | A Shipping Manifest has already been processed for the requested date/time {1}. |
| SHIP\_MANIFEST\_ERROR | No Shipments found to generate a Shipping Manifest for close date {1} for meter {2}. |
| SHIP\_MANIFEST\_ERROR | No Shipping Manifest files found in FedEx Directory for report only request for meter {1}. |
| SHIP\_SETUP\_REQD | No {1} registration was found for the location selected. Please select a different shipping item, or go to Setup > Set Up Shipping to register a {2} account for this location. |
| SHIP\_TALBE\_UNBALNCD | The Shipping Table is not balanced. Please review the table and ensure there is a Charge for every Range Value, and that there are no duplicates |
| SHIPFROM\_ADDRESS\_NOT\_SET | A shipping label could not be generated because the Phone Number of the "Ship From" address is not set. Please go to $(regex) to enter the "Ship From" Phone Number. |
| SHIPMNT\_INSURANCE\_NOT\_AVAILABLE | Insurance is not available when shipping to the destination country: {1} |
| SINGLE\_VALUE\_REQD | Multiple values found for a dropdown field that can only take one. |
| SITE\_DOMAIN\_NAME\_REQD | Notice: URL Components cannot be used until you have established a domain name for your site |
| SITE\_TAG\_ALREADY\_EXISTS | This site tag already exists |
| SITEMAP\_GEN\_ERROR | An error occurred while trying to generate the Sitemap. |
| SO\_HAS\_CHILD\_TRANS | This salesOrder has a one or more child transactions associated with it, and cannot be updated. |
| SO\_LINE\_HAS\_PO | Error: A Drop Ship/Special Order already exists for sales order {1}, line {2}. |
| SRVC\_UNAVAILBL\_FOR\_LOC | The requested service is unavailable between the selected locations. |
| SSS\_AUTHOR\_MUST\_BE\_EMPLOYEE | The author internal id or email must match an employee. |
| SSS\_CONNECTION\_TIME\_OUT | The host you are trying to connect to is not responding. |
| SSS\_DEBUG\_DISALLWD | Script Debugging is not allowed on this server. |
| SSS\_DRIP\_EMAIL\_RAN\_OUT\_OF\_COUPON\_CODES | Campaign event ran out of coupon codes. |
| SSS\_DUP\_DRIP\_EMAIL | You are attempting to send the same campaign email twice to the same recipient. |
| SSS\_FILE\_SIZE\_EXCEEDED | The file you are trying to load exceeds the maximum allowed file size of {1} megabyte. |
| SSS\_INSTRUCTION\_COUNT\_EXCEEDED | Script Execution Instruction Count Exceeded. |
| SSS\_INVALID\_ATTACH\_RECORD\_TYPE | Attaching of record type {1} to {2} is not supported. |
| SSS\_INVALID\_BCC\_EMAIL | One or more bcc emails are not valid. |
| SSS\_INVALID\_CC\_EMAIL | One or more cc emails are not valid. |
| SSS\_INVALID\_CMPGN\_EVENT\_ID | That campaign event is invalid, disabled, or is not a Lead Nurturing Email event. Please select an active Lead Nurturing Email campaign event. |
| SSS\_INVALID\_EMAIL\_TEMPLATE | That email template is invalid, disabled, or no longer exists. Please select an active email template. |
| SSS\_INVALID\_FORM\_ELEMENT\_NAME | You have entered an invalid form element name. It must be prefixed with "custpage", unique, and cannot contain any non-alphanumeric characters to be added to the form or sublist. |
| SSS\_GSO\_FLTR\_OPRTOR | SSS Invalid GetSelectOption Filter Operator {1}, must be one of the following: {2} |
| SSS\_INVALID\_HEADER | One or more headers are not valid. |
| SSS\_INVALID\_HOST\_CERT | An untrusted, unsupported, or invalid certificate was found for this host. You may also receive this error if the domain name is spelled incorrectly or does not use valid syntax. Verify that the domain name:
-   Has 63 or fewer characters
-   Contains alphanumeric characters (a-z, A-Z, 0-9) or hyphens
-   Starts with a letter
-   Ends with a letter or digit

 |
| SSS\_INVALID\_LIST\_COLUMN\_NAME | You have entered an invalid list column name. It must be unique and cannot contain any non-alphanumeric characters. |
| SSS\_INVALID\_LOCK\_WAIT\_TIME | You have entered an invalid wait time ({1}) for acquiring a lock. The wait time must be greater than 0ms and less than 5000ms. |
| SSS\_INVALID\_LOG\_TYPE | Execution log type must be one of AUDIT, DEBUG, ERROR, or EMERGENCY. |
| SSS\_INVALID\_PORTLET\_INTERVAL | You have entered an invalid refresh interval of {1} seconds. It must not be negative. |
| SSS\_INVALID\_PORTLET\_INTERVAL | You have entered an invalid refresh interval of {1} seconds. It must be at least {2} seconds if not in testing status. |
| SSS\_INVALID\_SCRIPTLET\_ID | That Suitelet is invalid, disabled, or no longer exists. |
| SSS\_INVALID\_SRCH\_COL | An nlobjSearchColumn contains an invalid column, or is not in proper syntax: {1}. |
| SSS\_INVALID\_SRCH\_COLUMN\_JOIN | An nlobjSearchColumn contains an invalid column join ID, or is not in proper syntax: {1}. |
| SSS\_INVALID\_SRCH\_COLUMN\_SUM | An nlobjSearchColumn contains an invalid column summary type, or is not in proper syntax: {1}. |
| SSS\_INVALID\_SRCH\_FILTER | An nlobjSearchFilter contains invalid search criteria: {1}. |
| SSS\_INVALID\_SRCH\_FILTER\_JOIN | An nlobjSearchFilter contains an invalid join ID, or is not in proper syntax: {1}. |
| SSS\_INVALID\_SRCH\_OPERATOR | An nlobjSearchFilter contains an invalid operator, or is not in proper syntax: {1}. |
| SSS\_INVALID\_SUBLIST\_OPERATION | You have attempted an invalid sublist or line item operation. You are either trying to cannot access a field on a non-existent line or you are trying to add or remove lines from a static sublist. |
| SSS\_INVALID\_SUBMIT\_OPTION | You have entered an invalid submit option for this record type: {1} |
| SSS\_INVALID\_TYPE\_ARG | You have entered an invalid type argument: {1} |
| SSS\_INVALID\_UI\_OBJECT\_TYPE | That operation is not supported for this type of UI object: {1}. It is only supported for type: {2}. |
| SSS\_INVALID\_URL | The URL must be a fully qualified HTTP or HTTPS URL if it is referencing a non-NetSuite resource. |
| SSS\_INVALID\_URL\_CATEGORY | The URL category must be one of RECORD, TASKLINK or SUITELET. |
| SSS\_INVALID\_WF\_RCRD\_TYPE | You have entered an invalid record type {1}. Workflow automation is not supported for this type of record. |
| SSS\_MEMORY\_USAGE\_EXCEEDED | Script Out Of Memory. |
| SSS\_MISSING\_REQD\_ARGUMENT | {1}: Missing a required argument: {2} |
| SSS\_QUEUE\_LIMIT\_EXCEEDED | Script Queue Usage Limit Exceeded |
| SSS\_RECORD\_TYPE\_MISMATCH | The record you are attempting to load has a different type: {1} from the type specified: {2}. |
| SSS\_REQUEST\_LIMIT\_ EXCEEDED | Request Limit Exceeded! |
| SSS\_REQUEST\_TIME\_EXCEEDED | The host you are trying to connect to is not responding or has exceeded the maximum allowed response time. |
| SSS\_SCRIPT\_DESERIA LIZATION\_FAILURE | Scheduled Script deserialization failure |
| SSS\_SEARCH\_TIMEOUT | Your search request has timed out. You may need to refine your search or combine the results of multiple searches to achieve the desired result. |
| SSS\_SSO\_CONFIG\_REQD | The SuiteSignOn object {1} is not configured for use with this script. You must specify the script as a connection point for this SuiteSignOn. |
| SSS\_STACK\_FRAME\_DEPTH\_EXCEEDED | Script Stack Frame Depth Exceeded. It means that somewhere in your code, you are calling a function which in turn calls another function and so forth, until you hit the call stack limit. You need to simplify your code or check it for recursive call loops. |
| SSS\_TIME\_LIMIT\_EXCEEDED | Script Execution Time Exceeded. |
| SSS\_TRANS\_IN\_PROGRESS | You cannot call nlapiBeginTransaction() because there is already a transaction in progress. |
| SSS\_TRANSACTION\_REQD | That operation can only be performed when there is a transaction in progress |
| SSS\_UNKNOWN\_HOST | The host you requested {1} is unknown or cannot be found. |
| SSS\_USAGE\_LIMIT\_EXCEEDED | Script Execution Usage Limit Exceeded |
| START\_DATE\_AFTER\_END\_DATE | The start date must preceed the end date. |
| START\_DATE\_REQD | Please enter a value for {1} Start Date |
| STATE\_ALREADY\_EXISTS | A State/Province/County with the same name already exists. |
| STATE\_REQD | State is a required field and it cannot be null or empty. |
| STATUS\_ASSIGNEE\_REQD | The issue status {1} does not define an assignee issue role. That status may not be used until this is corrected. |
| STORAGE\_LIMIT\_EXCEEDED | You entered a value that will exceed the internal storage limit of {1}. Please reduce the number. |
| STORE\_ALIAS\_UNAVAILABLE | The Store alias you chose "{1}" is already taken. Please go back and choose another. |
| STORE\_DOMAIN\_UNAVAILABLE | The store domain name you chose '{1}' is already taken. Please go back and choose another. |
| SUB\_MISMATCH | Resources for Time and Material projects must be in the customer's subsidiary. The following resources are in a different subsidiary: {1} |
| SUB\_RESTRICT\_VIEW\_REQD | Subsidiary Restrict View Required: You must first restrict your view to a subsidiary before running this report (Home > Set Preferences ><a href="https://docs.oracle.com/app/center/userprefs.nl?whence={1}">Restrict View</a>). |
| SUB\_TAX\_AGENCY\_REQD | No tax agency defined for subsidiary |
| SUBITEM\_REQD | You must first select the new subitems on the matrix tab you want to add. |
| SUBITEM\_REQD | You must first select the subitems on the matrix tab you want to create. |
| SUBSIDIARY\_MISMATCH | The employee and billable customer must be in the same subsidiary. |
| SUCCESS\_TRANS | The transaction was entered {1} successfully, {2} |
| SUPRT\_CNTR\_LOGIN\_ERROR | {1} Support Center login error: we are unable to find the customer record for account={2} |
| TAG\_ALREADY\_EXISTS | That tag name is already being used. Please go back and rename it. |
| TAG\_SUBSTITUTN\_ERROR | Error: Tag substitution loop encountered. Tag substitution sequence: {1} |
| TAG\_SUBSTITUTN\_ERROR | Error: Tag substitution result is too large. Tag substitution sequence: {1} |
| TAGATA\_ALREADY\_ENDORSED | The Receivable Tegata has already been endorsed. |
| TAX\_ACCT\_SETUP\_REQD | Tax Accounts Not Defined. |
| TAX\_CODE\_REQD | No default tax code is defined for country {1} |
| TAX\_CODES\_SETUP\_PROBLEM | The tax codes haven't been set properly |
| TAX\_CODES\_SETUP\_REQD | Can't open store for {1}. This company does not have its tax codes fully set up. This is required to properly calculate taxes on international, other-province and same-province orders. |
| TAX\_CODES\_SETUP\_REQD | The company is not usable. Administrator hasn't set up the tax codes. |
| TAX\_GROUP\_SETUP\_REQD | You have not created tax groups in your NetSuite account. To ensure that your customers are charged the correct amount of sales tax, you must create tax groups by entering them manually at Lists > Accounting > Tax Groups > New. |
| TAX\_PRD\_REQD | No Current Tax Period is defined. <a href='/app/setup/period/taxperiods.nl'>Click here</a> to create a tax period. |
| TAX\_SETUP\_REQD | The tax period range {1} has not been defined. Please visit '<A href='{2}'>Setup > Accounting > Manage Tax Periods</A>' to define this period or set up your year. |
| TEMPLATE\_NOT\_FOUND | Template not found |
| TEMPLATE\_NOT\_FOUND | Template Record not found |
| THIRD\_PARTY\_BILLING\_ACCT\_REQD | A 3rd Party Billing Account Number must be provided when selecting a 3rd Party Billing Type. |
| TICKET\_NOT\_LOCATED | The ticket {1} cannot be located in the error database. If this is from a customer logged case, the error may not yet be inserted into the system. |
| TIME\_ENTRY\_DISALLWD | {1} does not allow time entry. |
| TIMEOUT\_THE\_RECORD\_DOESNT\_EXIST\_ANYMORE | Timeout: the record doesn't exist anymore. |
| TOPIC\_REQD | You must select and add a topic to this solution. |
| TRAN\_DATE\_REQD | Missing transaction date. |
| TRAN\_LINE\_FX\_AMT\_REQD | Missing foreign currency amount on non-variance transaction line |
| TRAN\_LINK\_FX\_AMT\_REQD | Missing foreign currency amount on non-variance transaction link |
| TRAN\_PERIOD\_CLOSED | The action is causing generation of foreign exchange variance in a closed period. Please retry with {1} as the exchange rate. |
| TRAN\_PERIOD\_CLOSED | You are not allowed to change the revenue recognition status for one or more lines on this transaction as it would impact a closed period. |
| TRAN\_PERIOD\_CLOSED | You cannot change the G/L impact of a transaction in a closed period. |
| TRAN\_PRD\_CLOSED | This action cannot be completed because it requires modification of the transaction in a closed period due to foreign exchange variance. You may either open the period for this transaction or use the same rate ({1})between the transactions that will be linked. |
| TRANS\_ALREADY\_REFUNDED | Transaction Already refunded. A refund has already been performed on the transaction. |
| TRANS\_ALREADY\_SETTLED | Transaction Already Settled. Void failed because transaction has already settled, submit credit. |
| TRANS\_ALREADY\_VOIDED | Transaction Already Voided. Void failed because transaction is already voided. |
| TRANS\_AMTS\_UNBALNCD | Transaction is not in balance! amounts+taxes+shipping: {1}, total amount: {2} |
| TRANS\_APPLIED\_AMTS\_UNBALNCD | Transaction is not in balance! Total to apply of ${1} does not equal sum of applied ${2} and unapplied ${3} |
| TRANS\_APPLIED\_AMTS\_UNBALNCD | Transaction is not in balance! Total to apply of ${1} does not equal sum of payment ${2} and credits ${3} and deposits ${4} |
| TRANS\_CLASS\_UNBALNCD | Transaction out of balance for class {1} total = {2}. |
| TRANS\_DEPT\_UNBALNCD | Transaction out of balance for department {1} total = {2}. |
| TRANS\_DOES\_NOT\_EXIST | No transaction exists for that entity. |
| TRANS\_DSNT\_EXIST | The transaction you are attempting to access does not exist. |
| TRANS\_EDIT\_DISALLWD | This transaction is in a period that has been closed. You may not edit it. |
| TRANS\_EDIT\_DISALLWD | You cannot edit this transaction. {1} does not support the imported transaction. |
| TRANS\_FORGN\_CRNCY\_MISMATCH | Transaction and foreign currency account use different currencies. |
| TRANS\_FORGN\_CUR\_UNBALNCD | Transaction was not in balance (Foreign currency). Posting total = {1} |
| TRANS\_FORGN\_CUR\_UNBALNCD | Transaction was not in balance (Foreign currency). Total = {1} |
| TRANS\_IN\_USE | This transaction cannot be deleted because it is linked to by one or more transactions. Click <a href='/app/accounting/transactions/payments.nl?id={1}&label={2}&type={3}&alllinks=T'>here>/a> to see the list of linked transactions. |
| TRANS\_LINE\_AND\_PMT\_UNBALNCD | Transaction is not in balance! Line item sum of ${1} not equal to payment amount ${2} |
| TRANS\_LINES\_UNBALNCD | Transaction is not in balance! Line item sum of ${1} does not equal amount of ${2} |
| TRANS\_LINES\_UNBALNCD | Transaction is not in balance! Line item sum of ${1} does not equal applied amount of ${2} |
| TRANS\_LOC\_UNBALNCD | Transaction out of balance for location {1} total = {2}. |
| TRANS\_NOT\_CLEANED | Transaction not cleaned up. |
| TRANS\_NOT\_COMPLETED | Transaction was not complete. |
| TRANS\_PRCSSNG\_ERROR | Errors occurred while processing the selected transaction. Please process it individually for more information. |
| TRANS\_UNBALNCD | The debits and credits are not balanced on this transaction because amounts entered include more decimal places than are supported for this currency. Please round off the amount of each line to a maximum of {1} decimal places. |
| TRANS\_UNBALNCD | Transaction is not in balance! {1} |
| TRANS\_UNBALNCD | Transaction is not in balance! {1},{2} othercount = {3} |
| TRANS\_UNBALNCD | Transaction out of balance for {1} {2} total = {3}. |
| TRANS\_UNBALNCD | Transaction was not in balance. Posting total = {1} |
| TRANS\_UNBALNCD | Transaction was not in balance. Total = {1} |
| TRANSACTION\_DELETED | The transaction you are attempting to access has been deleted. |
| TRANSORD\_SHIP\_REC\_MISMATCH | You can not recieve more from a transfer order than you have shipped |
| TWO\_FA\_AUTH\_REQD | All your other roles require a one-time key at login. Please click "Go Back" to enter a one-time key or contact the company's administrator if you have questions. |
| TWO\_FA\_REQD | Two-Factor Authentication required |
| UNABLE\_TO\_PRINT\_CHECKS | Unable to print checks. |
| UNABLE\_TO\_PRINT\_DEPOSITS | Unable to print deposits. |
| UNAUTH\_CAMPAIGN\_RSPNS\_RQST | Unauthorized campaign response request |
| UNAUTH\_UNSUBSCRIBE\_RQST | Unauthorized unsubscribe request |
| UNDEFINED\_ACCTNG\_PRD | The accounting period range {1} has not been defined. Please visit '<A href='/app/setup/period/fiscalperiods.nl'>Setup > Accounting > Manage Accounting Periods</A>' to define this period or set up your year. |
| UNDEFINED\_ACCTNG\_PRD | The comparison accounting period range {1} has not been defined. Please visit '<A href='/app/setup/period/fiscalperiods.nl'>Setup > Accounting > Manage Accounting Periods</A>' to define this period or set up your year. |
| UNDEFINED\_ACCTNG\_PRD | The default accounting period for this report has not been defined. Please visit '<A href='/app/setup/period/fiscalperiods.nl'>Setup > Accounting > Manage Accounting Periods</A>' to define this period or set up your year. |
| UNDEFINED\_CSTM\_FIELD | Undefined customfield. |
| UNDEFINED\_TAX\_PRD | The default tax period for this report has not been defined. Please visit '<A href='/app/setup/period/taxperiods.nl'>Setup > Accounting > Manage Tax Periods</A>' to define this period or set up your year. |
| UNEXPECTED\_ERROR | An error occurred while processing item options. |
| UNEXPECTED\_ERROR | An unexpected error has occurred. |
| UNEXPECTED\_ERROR | An unexpected error has occurred. A FedEx Shipping Label was not generated. |
| UNEXPECTED\_ERROR | An unexpected error has occurred while generating this content.<p>Our Customer Support staff have been notified and are looking into the problem. |
| UNEXPECTED\_ERROR | An unexpected error has occurred while synching a record. Click \[OK\] to skip the record and continue. |
| UNEXPECTED\_ERROR | An unexpected error has occurred. NetSuite Customer Support has been alerted to this problem. |
| UNEXPECTED\_ERROR | An unexpected error occurred while extracting email from SMTP server |
| UNEXPECTED\_ERROR | An unexpected error occurred while logging email request completion |
| UNEXPECTED\_ERROR | An unexpected error occurred while logging email request failure |
| UNEXPECTED\_ERROR | An unexpected error occurred while logging email request start |
| UNEXPECTED\_ERROR | An unexpected error occurred while processing the payment. |
| UNEXPECTED\_ERROR | An unexpected error occurred with the group SQL |
| UNEXPECTED\_ERROR | An Unexpected JavaScript Error has occurred |
| UNEXPECTED\_ERROR | Error |
| UNEXPECTED\_ERROR | Error: {1} |
| UNEXPECTED\_ERROR | Please specify an scompid |
| UNEXPECTED\_ERROR | Problem during commission calculation |
| UNEXPECTED\_ERROR | An unexpected error occurred. |
| UNEXPECTED\_ERROR | Dto java class is not defined for {1}. |
| UNEXPECTED\_ERROR | Server error: no dto class is defined for record of type {1} |
| UNEXPECTED\_ERROR | Server error: missing database entries in WSRecordElement and WSNameSpace table for object of {1} |
| UNEXPECTED\_ERROR | Application error: no form request class is defined for record of type {1} |
| UNIQUE\_CONTACT\_NAME\_REQD | . Contact names must be unique |
| UNIQUE\_CUST\_EMAIL\_REQD | A customer record with this email address already exists. You must enter a unique customer email address for each record you create. |
| UNIQUE\_CUST\_EMAIL\_REQD | A customer record with this email address already exists. You must enter a unique customer email address for each record you create. To correct this record, click <a href='javascript:history.go(-1);';>back</a> and enter a new customer email address in the Customer field. Then, click Submit. |
| UNIQUE\_CUST\_ID\_REQD | A customer record with this ID already exists. You must enter a unique customer ID for each record you create. |
| UNIQUE\_CUST\_ID\_REQD | A customer record with this ID already exists. You must enter a unique customer ID for each record you create. To correct this record, click <a href='javascript:history.go(-1);';>back</a> and enter a new customer ID in the Customer field. Then, click Submit. |
| UNIQUE\_ENTITY\_NAME\_REQD | multiple sub-customers or jobs have name '{1}' which would create a naming conflict upon merge. All names must be unique. Before merging, you must change one of the subs named '{2}' to something else. |
| UNIQUE\_GROUPID\_REQD | You must specify exactly one numeric groupId |
| UNIQUE\_PARTNER\_CODE\_REQD | {1:name of partner record} Code "{2:partner code}" already exists. Please select a unique code for each record. |
| UNIQUE\_QTY\_REQD | Quantities must be unique |
| UNIQUE\_RCRD\_ID\_REQD | A record with this ID already exists. You must enter a unique ID to create or update this record. |
| UNIQUE\_SOLUTION\_CODE\_REQD | A solution with this particular solution code already exists. Please assign a different code. |
| UNITS\_TYP\_IN\_USE | This units type is used by {1} {2}. You must delete the {2} and all associated transactions to delete this units type. |
| UNKNOWN\_CARRIER | Package Tracking is not available for id {1}. Unknown carrier. |
| UNKNOWN\_RCRD\_TYPE | Unknown record type |
| UNKNOWN\_SCRIPT\_TYP | Unknown Script Type |
| UNKNWN\_ALLOCTN\_SCHDUL\_FREQ\_TYP | Unable to determine allocation schedule frequency type. |
| UNKNWN\_EMAIL\_AUTHOR | The author of this email cannot be found. |
| UNKNWN\_EXCHANGE\_RATE | Unable to determine the exchange rate for currency symbol {1}. Please create a currency item with an exchange rate for this currency. |
| UNRECOGNIZED\_METHOD | unrecognized method '{1}' |
| UNSUBSCRIBE\_REQD | Unsubscribe is mandatory, please enter a value for this field. |
| UNSUPPORTED\_METHOD | Unsupported method |
| UNSUPPORTED\_WS\_VERSION | TBA not supported in this SuiteTalk endpoint version |
| UNSUPRTD\_DOC\_TYP | You attempted to upload an unsupported document type. Please try again with a selection from the list below: |
| UPDATE\_DISALLWD | Update is not allowed |
| UPDATE\_PRICE\_AMT\_REQD | Please specify an amount to update prices. |
| UPGRADE\_WS\_VERSION | Could not set '{1}' to field '{2}' of record number {3} due to schema enumeration restriction. |
| UPGRADE\_WS\_VERSION | Please consider upgrading to endpoint {1} |
| UPGRADE\_WS\_VERSION | Sales order <id {1}> contains item serial/lot numbers that are not supported in your client application. You are not allowed to update serial/lot numbers on this sales order. Contact your software vendor for the latest SOAP web services upgrade. |
| UPGRADE\_WS\_VERSION | Sales order <id {1}> has items with more than one serial/lot numbers that is not supported in your client application. The serial/lot numbers have been removed to successfully return the sales order. Contact your software vendor for the latest SOAP web services upgrade. |
| UPGRADE\_WS\_VERSION | This {1} has multiple {2}s. SOAP web services schema version {3} or greater is required to modify {2} for this {1} |
| UPGRADE\_WS\_VERSION | {1} {2} has multiple shipping routes enabled, which is only supported in version 2008\_2 and newer. The shipping information has been omitted to successfully return this record. |
| UPS\_CANT\_INTEGRATE\_FULFILL | The fulfillment cannot be integrated with UPS because the Shipping Integration Carrier is not set to UPS. |
| UPS\_CONFIG\_ERROR | A UPS configuration error occured. Please contact tech support. |
| UPS\_LICENSE\_AGREEMNT\_REQD | You must agree to the UPS license agreement |
| UPS\_ONLINE\_RATE\_UNAVAILBL | The UPS Online Realtime Rates System is temporarily unavailable. Please resubmit your rate request in a few minutes. |
| UPS\_ONLINE\_RATE\_UNAVAILBL | UPS did not return any rates for the specified origin and destination addresses. |
| UPS\_ONLINE\_SHIP\_UNAVAILBL | The UPS Online Shipping System is temporarily unavailable. Please resubmit your fulfillment in a few minutes. |
| UPS\_REG\_NUM\_IN\_USE | The submitted UPS Registration Number, {1}, is already in use. Please resubmit the registration with a different UPS registration Number. |
| UPS\_SETUP\_REQD | No UPS registration was found. Please register your UPS account with NetSuite before attempting to send a fulfillment request to UPS. |
| UPS\_VOID\_ERROR | The UPS Void failed due to a system failure. |
| UPS\_XML\_ERROR | XML Sent to UPS. UPS returned error code/text: |
| URL\_ID\_PARAM\_REQD | URL is missing the id parameter. The file could not be retrieved. |
| URL\_REQD | You must enter a URL for this media item. |
| USER\_CONTEXT\_REQD | User context is not set |
| USER\_DISABLED | user disabled |
| USER\_ERROR | Application ID mandatory but missing. |
| USER\_ERROR | An error occurred during your last update. |
| USER\_ERROR | A User Error Has Occurred |
| USER\_ERROR | Detach requires an AttachBasicReference |
| USER\_ERROR | Either internalId or externalId is required. |
| USER\_ERROR | Folder cannot be made a subfolder of itself. |
| USER\_ERROR | Gift Certificate From, Recipient Name, and Recipient Email are required. |
| USER\_ERROR | Invalid Attachment record combination |
| USER\_ERROR | Missing Item Weight or Weight Unit. |
| USER\_ERROR | Missing or Invalid RecordType for AttachTo |
| USER\_ERROR | Must submit a non-abstract instance of baseRef (eg RecordRef, CustomRecordRef) NOT a baseRef |
| USER\_ERROR | Must submit a non-abstract instance of record or searchRecord (eg customer or customerSearchBasic). |
| USER\_ERROR | No budget inserted or updated. |
| USER\_ERROR | {1} |
| USER\_ERROR | Please enter value(s) for: Company Name, Subsidiary |
| USPS\_ACCT\_NUM\_ALREADY\_EXISTS | There is an existing NetSuite registration for Endicia account number {1}. |
| USPS\_INVALID\_INSURED\_VALUE | Insured value exceeds the {1} maximum allowed by Endicia. |
| USPS\_INVALID\_PACKAGING | The Carrier Packaging that you have selected is not valid for this item fulfillment. <br>Usually this indicates the selected packaging cannot be used with the selected USPS shipping method, or the package weight is invalid. <br>Please check the documentation for more details. |
| USPS\_INVALID\_PSWD | The Endicia Web Password does not match the Web Password for this USPS Registration account number. |
| USPS\_LABEL\_VOIDED | This error required 1 or more labels created for this transaction to be voided at Endicia. |
| USPS\_LABEL\_VOIDED | This error required 1 or more labels created for this transaction to be voided at Endicia.<br> |
| USPS\_MAX\_ITEM\_EXCEEDED | International USPS fulfillments allow a maximum of 5 unique items per package, due to customs documentation. If more than one package is required, please break up the shipment into multiple fulfillments. |
| USPS\_ONE\_PACKAGE\_ALLWD | International USPS fulfillments allow only one package. If more than one package is required, please break up the shipment into multiple fulfillments of one package each. |
| USPS\_PASS\_PHRASE\_NOT\_UPDATED | The Endica Pass Phrase was not updated: {1} |
| USPS\_REFUND\_FAILED | Failed Endicia Refund Request |
| USPS\_REFUND\_FAILED | The Endicia Refund Request failed due to a system error. |
| USPS\_RETRY | A response was not received for the USPS funding request. Please try again in a few minutes. |
| USPS\_VALIDATE\_ADDR | The address you entered could not be validated. Please verify the city, state, and/or zip code.<br><br>You can validate an address by visiting the <a href="http://zip4.usps.com/zip4/welcome.jsp" target="\_blank">U.S. Postal Service</a> web site, or the <a href="http://www.endicia.com/Developers/ZipLookup/" target="\_blank">Endicia</a> web site. |
| USPS\_VERIFY\_TRACKING\_NUM | Please verify that the following tracking numbers were created and voided in your Endicia account before proceeding. |
| USPS\_VOID\_ERROR | An error was detected during the Endicia Void operation: |
| USPS\_VOID\_ERROR | An error was detected during the Endicia Void operation:<br> |
| VALID\_EMAIL\_REQD | Missing or invalid email address. Email address is a required field and it cannot be null or empty. The email address must be in a valid format. |
| VALID\_EMAIL\_REQD\_FOR\_LOGIN | Please enter a valid email address when granting login access privileges to this record. |
| VALID\_FIRST\_NAME\_REQD | Missing or invalid First Name. Users first name is a required field and cannot be null or empty. |
| VALID\_LAST\_NAME\_REQD | Missing or invalid Last Name. Users last name is a required field and cannot be null or empty. |
| VALID\_LINE\_ITEM\_REQD | You must have at least one valid line item for this transaction. |
| VALID\_PHONE\_NUM\_REQD | Missing or invalid Home phone number. The Home phone number is a required field and it cannot be null or empty. The format of the Home phone number must contain area code plus seven digit number. |
| VALID\_PRD\_REQD | Insert Transaction Failure: No valid, open, posting period for date - {1}. Please visit Setup > Manage Accounting Periods to set up a new accounting period. |
| VALID\_PRD\_REQD | Insert Transaction Failure: No valid, open, tax period for date - {1}. Please visit Setup > Manage Tax Periods to set up a new tax period. |
| VALID\_PRD\_REQD | Update Transaction Failure: No valid, open, {1} period for date - {2} |
| VALID\_URL\_REQD | Please go back and provide a valid URL for all five fields on the External tab. |
| VALID\_VERSION\_REQD\_IN\_URL | If the version parameter is passed through the URL, it MUST contain a valid version in a phased release environment. Valid: {1} |
| VALID\_WORK\_PHONE\_REQD | Missing or invalid Work phone number. The Work phone number is a required field and it cannot be null or empty. The format of the Work phone number must contain area code plus seven digit number. |
| VALID\_ZIPCODE\_REQD | Missing or invalid ZIP code field. ZIP code is a required field and it cannot be null or empty. ZIP code and state values are checked against an internal database to make sure that ZIP code specified exists in state specified. |
| VENDOR\_TYPE\_REQD | No Vendor Type was specified. If creating a Tax Agency, please ensure that the vendor type is active and marked as a tax agency. |
| VERIFY\_DESTNTN\_ZIP\_CODE | Please verify that the destination zipcode is correctly specified. |
| VERIFY\_PAYROLL\_FUND\_ACCT | The payroll funding account has not been verified. Please verify the payroll funding account |
| VERIFY\_ZIP\_CODE\_SETUP | Please verify that you have correctly set your zip code under setup company. If you have multi-location enabled, verify that you have set a correct zipcode for each location. |
| VISA\_ERROR | Communication error with Visa. Please retry. |
| VOID\_FAILED | Void Failed. Failed to void transaction, retry void or issue credit. |
| VOIDING\_REVERSAL\_DISALLWD | You may not create a voiding reversal for transactions with inventory impact. To reverse the inventory impact of the transaction, you will need to create an inventory adjustment. |
| VSOE\_CANT\_ADD\_ITEM\_GROUP | When the <b>Is VSOE bundle</b> box is checked, Items for Purchase cannot be added to item groups. |
| VSOE\_REV\_REC\_TMPLT\_REQD | All Lines in a VSOE Bundle with a VSOE Allocation must have a revenue recognition template. |
| VSOE\_TOTAL\_ALLOCATION\_ERROR | The total vsoe allocation in a bundle must equal the total bundle sales amount. |
| VSOE\_TRAN\_VSOE\_BUNDLE\_ERROR | You have indicated that you would like this transaction to be treated as a Bundle (multi-element arrangement) for VSOE purposes. Please either uncheck the 'Transaction Is VSOE Bundle' checkbox or remove the Item Groups that have the 'Is VSOE Bundle' option specified. |
| WF\_EXEC\_USAGE\_LIMIT\_EXCEEDED | Workflow Execution Usage Limit Exceeded |
| WORK\_DAYS\_REQD | Select one or more working days. |
| WORLDPAY\_ERROR | A failure occurred while attempting to connect to WorldPay. |
| WORLDPAY\_ERROR | There was a problem with your WorldPay credentials. Please be sure you are using the correct combination of Installation ID, Merchant Code and XML Password |
| WRITE\_OFF\_ACCT\_REQD | To receive items without restocking, you must first set a value for the write-off account. To set the value of the write-off account, go to _Accounting > Accounting Preferences > Order Management > Write-Off Account for Returns_. |
| WS\_CONCUR\_SESSION\_DISALLWD | Someone has logged in as this user from a different SOAP web services session. Only one person may login as a particular user at a time. As a consequence, this session has been terminated. |
| WS\_CONCUR\_SESSION\_DISALLWD | Only one request may be made against a session at a time |
| WS\_EXCEEDED\_CONCUR\_USERS\_ALLWD | You can have a maximum of {1} active concurrent WS users at a time in {2} |
| WS\_FEATURE\_REQD | You have not enabled SOAP web services feature for your account. |
| WS\_INVALID\_SEARCH\_OPERATN | When using request-level credentials, you must use the {1} operation instead of {2} |
| WS\_LOG\_IN\_REQD | You must log in before performing a web service operation. |
| WS\_PERMISSION\_REQD | You do not have permission to access SOAP web services feature. |
| WS\_REQUEST\_BLOCKED | SuiteTalk concurrent request limit exceeded. Request blocked. |
| ZIP\_FILE\_CONTAINS\_VIRUS | The zip file contains a virus {1}. Upload abort. |

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Development Considerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3421363.html)
-   [SOAP Web Services Warnings, Errors, and Faults](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536574.html)
-   [SOAP Faults for Each Operation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3536956.html)
-   [SOAP Fault Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3539420.html)
-   [Warning Status Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3599699.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
