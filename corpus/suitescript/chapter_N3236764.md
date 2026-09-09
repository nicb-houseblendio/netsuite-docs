---
id: "chapter_N3236764"
type: "chapter"
title: "Permission Names and IDs"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript IDs > Permission Names and IDs"
parent: "chapter_1494647249"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3236764.html"
anchors: []
sha256: "096e7bda218cade0f90e6ffc38260ee118099dbf6ad0641b627a7b29afb487c9"
---

The following table provides permission names and IDs associated with each NetSuite feature. You can use the permission ID to return the permission levels that have been specified in your account by calling [User.getPermission(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296668393.html) in the [N/runtime Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4296359529.html).

The following link provides access to a Microsoft Excel worksheet listing the usage of most NetSuite permissions: [NetSuitePermissionsUsage.xls](https://system.netsuite.com/core/media/media.nl?id=359816354&c=NLCORP&h=ARV6JlFsVUmTraKk02jPw8s85QSxEDenjWXwbgch473UhWZL&_xt=.xls). You can use this list to understand the implications of assigning a specific permission, or to find the permission required to provide access to a specific task or page. For more information, see [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html).

| Permission ID | Permission Name | Feature | Valid Levels |
| --- | --- | --- | --- |
| ADMI\_ACCOUNTING | Accounting Management | Accounting | None, Full |
| ADMI\_ACCOUNTINGBOOK | Accounting Book | Accounting | None, View, Create, Edit, Full |
| ADMI\_ACCOUNTINGLIST | Accounting Lists | Accounting | None, View, Create, Edit, Full |
| ADMI\_ACCTPERIODS | Manage Accounting Periods | Accounting Periods | None, View, Full |
| ADMI\_ACCTSETUP | Set Up Accounting | Accounting | None, Full |
| ADMI\_ACCTSETUP | Accounting Preferences | Accounting | None, Full |
| ADMI\_ADVANCED\_ORDER\_MANAGEMENT | Advanced Order Management | Advanced Order Management | None, Full |
| ADMI\_ADVANCED\_TEMPLATES | Advanced PDF/HTML Templates | Advanced Printing | None, Full |
| ADMI\_ALLOW\_JS\_HTML\_UPLOAD | Allow JS / HTML Uploads | Documents | None, Full |
| ADMI\_ALLOWNONGLCHANGES | Allow Non G/L Changes | Accounting Periods | None, Full |
| ADMI\_ANALYTICS | Analytics Administrator | \- | None, Full |
| ADMI\_APP\_DEPLOYMENT | SuiteApp Deployment | SuiteApp | None, Full |
| ADMI\_APPDEFPKG | App Definitions and Packages | \- | None, Full |
| ADMI\_APPPUBLISHER | Application Publishers | SSP Applications | None, Full |
| ADMI\_AUDITLOGIN | View Login Audit Trail | Login Audit Trail | None, Full |
| ADMI\_BACKUPEXPORT | Backup Your Data | CSV Export | None, Full |
| ADMI\_BALANCE\_TRX\_BY\_SEGMENTS | Balance Transactions by Segments | Balancing Segments | None, View, Create |
| ADMI\_BANK\_CONNECTIVITY\_CONFIG | Bank Connectivity Plug-In Configuration | \- | None, Full |
| ADMI\_BILLINGINFO | Billing Information | Allow Multiple Users | None, Full |
| ADMI\_BLCGA | Balance Location Costing Group Accounts | Group Average Costing | None, Full |
| ADMI\_BUNDLER | SuiteBundler | SuiteBundler | None, Full |
| ADMI\_BUNDLER | SuiteApp Marketplace | SuiteBundler | None, Full |
| ADMI\_BUNDLERAUDITTRAIL | SuiteBundler Audit Trail | SuiteBundler | None, Full |
| ADMI\_BUNDLERMANUP | SuiteBundler Upgrade Install Base | SuiteBundler | None, Full |
| ADMI\_CAMPAIGNEMAIL | Set Up Campaign Email Addresses | Marketing Automation | None, Full |
| ADMI\_CAMPAIGNSETUP | Setup Campaigns | Marketing Automation | None, Full |
| ADMI\_CASEALERT | Case Alerts | Customer Support and Service | None, View, Full |
| ADMI\_CASEFORM | Online Case Form | Customer Support and Service | None, Full |
| ADMI\_CASEISSUE | Support Case Issue | Customer Support and Service | None, Full |
| ADMI\_CASEORIGIN | Support Case Origin | Customer Support and Service | None, Full |
| ADMI\_CASEPRIORITY | Support Case Priority | Customer Support and Service | None, Full |
| ADMI\_CASERULE | Support Case Territory Rule | Customer Support and Service | None, View, Create, Edit, Full |
| ADMI\_CASESTATUS | Support Case Status | Customer Support and Service | None, Full |
| ADMI\_CASETERRITORY | Support Case Territory | Customer Support and Service | None, View, Create, Edit, Full |
| ADMI\_CASETYPE | Support Case Type | Customer Support and Service | None, Full |
| ADMI\_CENTERLINK | Custom Center Link | Custom Centers | None, Full |
| ADMI\_CERTIFICATES | Certificate Management | \- | None, View, Create, Edit, Full |
| ADMI\_CLASSESTOLOCS | Convert Classes to Locations | Locations | None, Full |
| ADMI\_CLASSSEGMENTMAPPING | Class Segment Mapping | Classes | None, Full |
| ADMI\_CLASSSEGMENTMAPPING | Class Mapping | Multi Book Version 2 | \- |
| ADMI\_CLOSEPERIOD | Lock Transactions | Accounting Periods | None, Full |
| ADMI\_COMMERCECATEGORY | Commerce Categories | \- | None, Full |
| ADMI\_COMMISSIONSETUP | Commission Feature Setup | Commissions | None, Full |
| ADMI\_COMPANY | Company Information | Company Setup | None, Full |
| ADMI\_CONVERTCLASSES | Convert Classes to Departments | Departments | None, Full |
| ADMI\_CONVERTLEAD | Lead Conversion Mapping | Sales Force Automation | None, Full |
| ADMI\_COPYPROJECTTASK | Copy Project Tasks | Project Management | None, Full |
| ADMI\_CREATEJOBSFROMSALESTRANS | Create Jobs from Sales Transactions | Project Management | None, Full |
| ADMI\_CREDITCARD | Credit Card Processing | Credit Card Payments | None, Full |
| ADMI\_CRMLIST | CRM Lists | Opportunities | None, View, Create, Edit, Full |
| ADMI\_CROSSCHARGE | Manage Cross Charge Automation | Intercompany Framework | View, None, Full |
| ADMI\_CSVIMPORTPREF | Set Up CSV Preferences | Accounting | None, Full |
| ADMI\_CUSTADDRESSFORM | Custom Address Form | Custom Forms | None, View, Create, Edit, Full |
| ADMI\_CUSTBODYFIELD | Custom Body Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTCATEGORY | Custom Center Categories | Custom Centers | None, View, Create, Edit, Full |
| ADMI\_CUSTCENTER | Custom Centers | Custom Centers | None, View, Create, Edit, Full |
| ADMI\_CUSTCOLUMNFIELD | Custom Column Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTEMAILLAYOUT | Custom HTML Layouts | Custom PDF/HTML Templates | None, View, Create, Edit, Full |
| ADMI\_CUSTENTITYFIELD | Custom Entity Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTENTRYFORM | Custom Entry Forms | Custom Forms | None, View, Create, Edit, Full |
| ADMI\_CUSTEVENTFIELD | Custom Event Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTFIELD | Custom Fields | SuiteFlow Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTFIELDTAB | Custom Subtabs | Custom Subtabs | None, View, Create, Edit, Full |
| ADMI\_CUSTFORM | Custom Transaction Forms | Custom Forms | None, View, Create, Edit, Full |
| ADMI\_CUSTITEMFIELD | Custom Item Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTITEMNUMBERFIELD | Custom Item Number Fields | Inventory | None, View, Create, Edit, Full |
| ADMI\_CUSTLAYOUT | Custom PDF Layouts | Custom PDF/HTML Templates | None, View, Create, Edit, Full |
| ADMI\_CUSTLIST | Custom Lists | Custom Lists | None, View, Create, Edit, Full |
| ADMI\_CUSTOMERFORM | Online Customer Form | Sales Force Automation | None, View, Create, Edit, Full |
| ADMI\_CUSTOMERRULE | Sales Territory Rule | Sales Force Automation | None, View, Create, Edit, Full |
| ADMI\_CUSTOMER\_SEGMENTS | Customer Segments Manager | \- | None, Full |
| ADMI\_CUSTOMIZEDFIELDLEVELHELP | Customize Field Level Help | SuiteBuilder Customized Field Level Help | None, View, Create, Edit, Full |
| ADMI\_CUSTOMSCRIPT | SuiteScript | Client SuiteScript | None, View, Create, Edit, Full |
| ADMI\_CUSTOMSUBLIST | Custom Sublists | Custom Sublists | None, View, Create, Edit, Full |
| ADMI\_CUSTOTHERFIELD | Other Custom Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTRECORD | Custom Record Types | Custom Records | None, View, Create, Edit, Full |
| ADMI\_CUSTRECORDFORM | Online Custom Record Form | Custom Forms | None, View, Create, Edit, Full |
| ADMI\_CUSTSECTION | Custom Center Tabs | Custom Records | None, View, Create, Edit, Full |
| ADMI\_CUSTTASKS | Custom Center Links | Custom Records | None, View, Create, Edit, Full |
| ADMI\_CUSTTRANFIELD | Custom Transaction Fields | Custom Fields | None, View, Create, Edit, Full |
| ADMI\_CUSTTRANSACTION | Custom Transaction Types | Custom Transactions | None, View, Create, Edit, Full |
| ADMI\_DELETEDRECORD | Deleted Records | Search for Deleted Records | None, Full |
| ADMI\_DEPTSEGMENTMAPPING | Department Segment Mapping | Departments | None, Full |
| ADMI\_DEPTSEGMENTMAPPING | Department Mapping | Multi Book Version 2 | None, Full |
| ADMI\_DEVICE\_ID | Device ID Management | Suite Commerce InStore | None, Full |
| ADMI\_DIRECTINVOICEPAYMENTSETUP | Direct Invoice Payment Setup | \- | None, View, Create, Edit, Full |
| ADMI\_DOMAINS | Set Up Domains | SuiteCommerce | None, Full |
| ADMI\_DUPLICATESETUP | Duplicate Detection Setup | Duplicate Detection & Merge | None, Full |
| ADMI\_EMPLCATEGORY | Publish Employee List | SuiteCommerce | None, Full |
| ADMI\_EMPLOYEE\_EXPENSE\_SOURCE | Employee Expense Sources | Expense Reports | None, View, Create, Edit, Full |
| ADMI\_EMPLOYEECENTERPUBLISHING | Employee Center Publishing | \- | None, Full |
| ADMI\_EMPLOYEELIST | Other Lists | Accounting | None, View, Create, Edit, Full |
| ADMI\_ENABLEFEATURES | Enable Features | Enable Company Features | None, Full |
| ADMI\_ENTITYACCOUNTMAPPING | Entity Account Mapping | Accounting | None, Full |
| ADMI\_ENTITYSTATUS | Customer Status | Customer Relationship Management | None, Full |
| ADMI\_ESCALATIONRULE | Escalation Assignment Rule | Customer Support and Service | None, View, Create, Edit, Full |
| ADMI\_ESCALATIONTERRITORY | Escalation Assignment | Customer Support and Service | None, View, Create, Edit, Full |
| ADMI\_EXPENSEREPORTPOLICY | Expense Report Policies | Expense Reports | None, View, Full |
| ADMI\_EXPORTIIF | Export as IIF | Accounting | None, Full |
| ADMI\_FFTEXCEPTIONREASON | Fulfillment Exception Reason | \- | None, View, Create, Edit, Full |
| ADMI\_FINANCIALINSTITUTION | Financial Institution Records | \- | None, Full |
| ADMI\_FINCHARGEPREF | Finance Charge Preferences | A/R | None, Full |
| ADMI\_GAINLOSSACCTMAPPING | Foreign Currency Variance Mapping | Accounting | None, Full |
| ADMI\_GLOBALACCOUNTMAPPING | Global Account Mapping | Accounting | None, Full |
| ADMI\_HTMLFORMULA | Create HTML Formulas in Search | \- | None, View, Create, Edit, Full |
| ADMI\_IMPORTCSVFILE | Import CSV File | CSV Import | None, Full |
| ADMI\_IMPORTOVERRIDESSTRIG | Control SuiteScript and Workflow Triggers per CSV Import |  | None, Full |
| ADMI\_IMPORTXML | Set Up ADP Payroll | Import ADP Payroll | None, Full |
| ADMI\_INTEGRAPP | Integration Application | Integration | None, Full |
| ADMI\_ISSUESETUP | Issue Setup | Issue Management | None, Full |
| ADMI\_ISSUESHOWSTOPPER | Mark Issue As Showstopper | Issue Management | None, Full |
| ADMI\_ITEMACCOUNTMAPPING | Item Account Mapping | Accounting | None, Full |
| ADMI\_KERNEL | Core Administration Permissions | Core Administration Permissions | None, Full |
| ADMI\_KEYS | Key management | \- | None, View, Create, Edit, Full |
| ADMI\_KNOWLEDGEBASE | Publish Knowledge Base | Knowledge Base | None, View, Create, Edit, Full |
| ADMI\_KPIREPORT | KPI Scorecards | KPI Scorecards | None, Full |
| ADMI\_LOCATIONCOSTINGGROUP | Location Costing Group | Item Record Management | None, Full |
| ADMI\_LOCSEGMENTMAPPING | Location Segment Mapping | Custom Segments | None, Full |
| ADMI\_LOCSEGMENTMAPPING | Location Mapping | Multi Book Version 2 | None, Full |
| ADMI\_LOGIN\_OAUTH | Log in using Access Tokens | TBA | None, Full |
| ADMI\_LOGIN\_OAUTH2 | Log in using OAuth 2.0 Access Tokens | OAuth 2.0 | None, Full |
| ADMI\_MANAGECUSTOMSEGMENTS | Custom Segments | Custom Segments | None, View, Create, Edit, Full |
| ADMI\_MANAGE\_OAUTH2 | OAuth 2.0 Authorized Applications Management | OAuth 2.0 | None, Full |
| ADMI\_MANAGE\_OAUTH\_TOKENS | Access Token Management | Token-based Authentication | None, Full |
| ADMI\_MANAGE\_OWN\_OAUTH\_TOKENS | User Access Tokens | Token-based Authentication | None, Full |
| ADMI\_MANAGE\_RESTRICTIONS | Manage Custom Restrictions | Advanced Employee Permissions | None, View, Edit, Full, Create |
| ADMI\_MANAGEPERMISSIONS | Manage Custom Permissions | Allow Multiple Users | None, Full |
| ADMI\_MANAGEROLES | Bulk Manage Roles | Show Role Differences | None, Full |
| ADMI\_MANAGEUSERS | Manage Users | Managing Users | None, Full |
| ADMI\_MANUFACTURING | Manufacturing Preferences | Assembly Items | None, Full |
| ADMI\_MHLEVEL | Merchandise Hierarchy Level | \- | None, Full |
| ADMI\_MHNODE | Merchandise Hierarchy Node | \- | None, Full |
| ADMI\_MHVERSION | Merchandise Hierarchy Version | \- | None, Full |
| ADMI\_MIGRATEREVARRNGANDPLAN | Migrate Revenue Arrangements and Plans | Advanced Revenue Management | None, Full |
| ADMI\_MOBILE\_ACCESS | Mobile Device Access | \- | None, Full |
| ADMI\_MCP\_SERVER | MCP Server Connection | \- | None, Full |
| ADMI\_NSASOIDCPROVIDER | OIDC Provider Setup |  | None, Full |
| ADMI\_NUMBERING | Auto-Generated Numbers |  | None, View, Edit, Full |
| ADMI\_OIDC | OpenID Connect (OIDC) Single Sign-On | \- | None, Full |
| ADMI\_OIDCSETUP | Set Up OpenID Connect (OIDC) Single Sign-On | \- | None, Full |
| ADMI\_OPENIDSSO | OpenID Single Sign-on | \- | None, Full |
| ADMI\_OPENIDSSOSETUP | Set Up OpenID Single Sign-on | \- | None, Full |
| ADMI\_ORDERALLOCATIONSTRATEGY | Order Allocation Strategy | \- | None, View, Create, Edit, Full |
| ADMI\_ORDERPROMISING | Order Promising | \- | None, View, Full |
| ADMI\_OUTLOOKINTEGRATION | Outlook Integration 2.0 | Outlook Integration | None, Full |
| ADMI\_OUTLOOKINTEGRATION\_V3 | Outlook Integration 3.0 | Outlook Integration | None, Full |
| ADMI\_PARTNERCONTRIBUTION | Partner Contribution | \- | None, Full |
| ADMI\_PAYMENT\_LINK\_SETUP | Set Up Payment Link |  | None, Full |
| ADMI\_PAYROLL | Set Up Payroll | Payroll | None, Full |
| ADMI\_PENDINGBOOKJOURNAL | Allow Pending Book Journal Entry | \- | None, Full |
| ADMI\_PERIODCLOSING | Period Closing Management | \- | None, Full |
| ADMI\_PERIODOVERRIDE | Override Period Restrictions | \- | None, Full |
| ADMI\_PI\_REMOVAL\_CREATE | Remove Personal Information Create | \- | None, Full |
| ADMI\_PI\_REMOVAL\_RUN | Remove Personal Information Run | \- | None, Full |
| ADMI\_PROJECT\_ACCOUNTING\_SETUP | Project Profitability Setup | Project Management | None, Full |
| ADMI\_PROJECT\_ACCOUNTING\_SETUP | Project Profitability | Advanced Project Profitability | None, Full |
| ADMI\_PROMPTS | Prompts | AI | None, View, Create, Edit, Full |
| ADMI\_PROVISION | Provisioning | NLCORP feature | None, View, Full |
| ADMI\_RAG | Knowledge Base for Retrieval Augmented Generation | Artificial Intelligence | None, Full |
| ADMI\_RECSYS | Intelligent Recommendations | Artificial Intelligence | None, View |
| ADMI\_REPOGROUPS | Financial Statement Sections | Accounting | None, Full |
| ADMI\_REPOLAYOUTS | Financial Statement Layouts | Accounting | None, Full |
| ADMI\_RESTWEBSERVICES | REST Web Services | REST Web Services | None, Full |
| ADMI\_REVIEW\_CUSTOM\_GL\_RUNS | Review Custom GL plug-in executions | Custom GL Lines Plug-in | None, Full |
| ADMI\_SALESCHANNEL | Sales Channel | \- | None, View, Edit, Full, Create |
| ADMI\_SALESTERRITORY | Sales Territory | Sales Force Automation | None, View, Create, Edit, Full |
| ADMI\_SAMLSSO | SAML Single Sign-on | SAML Single Sign-on | None, Full |
| ADMI\_SAMLSSOSETUP | Set Up SAML Single Sign-on | SAML Single Sign-on | None, Full |
| ADMI\_SAVEDASHBOARD | Publish Dashboards | Publishing Dashboards | None, Full |
| ADMI\_SETUPCOMPANY | Set Up Company | Company Preferences | None, View, Full |
| ADMI\_SETUPIMAGERESIZE | Set Up Image Resizing | SuiteCommerce Advanced | None, Full |
| ADMI\_SETUPYEARSTATUS | Set Up Year Status | Accounting | None, Full |
| ADMI\_SFASETUP | Sales Force Automation Setup | Sales Force Automation | None, Full |
| ADMI\_SITEMANAGEMENT | Web Site Management | Web Site | None, Full |
| ADMI\_STATETAXIMPORT | Import State Sales Tax | Accounting | None, Full |
| ADMI\_STORESEARCH | Site Search | \- | None, Full |
| ADMI\_STORESETUP | Set Up Web Site | Web Site | None, Full |
| ADMI\_SUBLIST | Custom Sublist | Allow Multiple Users | None, View, Create, Edit, Full |
| ADMI\_SUBSIDIARYHIERARCHYMOD | Subsidiary Hierarchy Modification | \- | None, View, Edit |
| ADMI\_SUBSIDIARYSETTINGSMANAGER | Subsidiary Settings Manager | \- | None, View, Edit |
| ADMI\_SUITE\_OAX\_CONNECTOR | NSAW Connector Administrator |  | None, Full |
| ADMI\_SUITEANALYTICSCONNECT | SuiteAnalytics Connect | SuiteAnalytics Connect | None, Full |
| ADMI\_SUITEAPP\_MANAGEMENT | SuiteApp Management | SuiteApp Control Center | None, Full |
| ADMI\_SUITECOMMERCEANALYTICS | SuiteCommerce Analytics |  | None, View, Full |
| ADMI\_SUITESIGNON | SuiteSignOn | Outbound Single Sign-on | None, Full |
| ADMI\_SUITE\_OAX\_CONNECTOR | OAX Connector Administrator | NetSuite Analytics Warehouse | None, Full |
| ADMI\_SUPPLYALLOCATIONSETUP | Supply Allocation Setup | \- | None, View, Create, Edit, Full |
| ADMI\_SUPPORTSETUP | Support Setup | Customer Support and Service | None, Full |
| ADMI\_SWAPPRICES | Swap Prices Between Price Levels | Multiple Prices | None, Full |
| ADMI\_TAXMIGRATION | SuiteTax Migration | \- | None, Full |
| ADMI\_TIMEMODIFICATION | Bulk Time Entry Modification | \- | None, Full |
| ADMI\_TAXPERIODS | Manage Tax Reporting Periods | Accounting | None, Full |
| ADMI\_TEAMSELLINGCONTRIBUTION | Team Selling Contribution | Team Selling | None, Full |
| ADMI\_TELEPHONY\_SETUP | Telephony Integration | Telephony | None, Full |
| ADMI\_TRAN\_ACCOUNTING\_RULES | Transaction Accounting Rules | \- | None, Full |
| ADMI\_TRANSITEMTXT | Translation | Multi-Language | None, Full |
| ADMI\_TRANSLATION | Manage Translation | Multi-Language | None, Full |
| ADMI\_TSTDRV\_MASTER | Testdrive Masters | NLCORP feature | None, Full |
| ADMI\_TWOFACTORAUTH | Two-Factor Authentication | Two-Factor Authentication | None, Full |
| ADMI\_TWOFACTORAUTHBASE | Two-Factor Authentication base | Two-Factor Authentication | None, Full |
| ADMI\_UNCATSITEITEMS | Uncategorized Presentation Items | Web Store | None, Full |
| ADMI\_UPDATEPRICES | Update Prices | Item Record Management | None, Full |
| ADMI\_UPSELLSETUP | Upsell Setup | Upsell Manager | None, Full |
| ADMI\_WEBSERVICES | SOAP Web Services | SuiteTalk | None, Full |
| ADMI\_WEBSERVICES | Web Services | Internal Web Services | None, Full |
| ADMI\_WEBSERVICESLOG | View SOAP Web Services Logs | SuiteTalk | None, Full |
| ADMI\_WEBSERVICESLOG | View Web Services Logs | Internal Web Services | None, Full |
| ADMI\_WEBSERVICESSETUP | Set Up SOAP Web Services | SuiteTalk | None, Full |
| ADMI\_WEBSERVICESSETUP | Set Up Web Services | Internal Web Services | None, Full |
| ADMI\_WORKFLOW | Workflow | SuiteFlow | None, Full |
| LIST\_ACCOUNT | Accounts | Accounting | None, View, Create, Edit, Full |
| LIST\_ACH | Automated Clearing House | Payment Instruments | None, View, Create, Edit, Full |
| LIST\_ALLGOVERNMENTISSUEDIDS | Advanced Government-Issued IDs | Advanced Government-Issued ID Tracking | None, View, Create, Edit, Full |
| LIST\_ALLOCSCHEDULE | Allocation Schedules | Expense Allocation | None, View, Create, Edit, Full |
| LIST\_AMORTIZATION | Amortization Schedules | Amortization | None, View, Create, Edit, Full |
| LIST\_BASICGOVERNMENTISSUEDIDS | Basic Government-Issued IDs | Basic Government-Issued ID Tracking | None, View, Create, Edit, Full |
| LIST\_BIG\_SEARCH | Persist Search | Search | None, Create |
| LIST\_BILLINBOUNDSHIPMENT | Bill Inbound Shipment | Inbound Shipment Management | None, View, Create, Edit, Full |
| LIST\_BILLINGSCHEDULE | Billing Schedules | SuiteBilling | None, View, Create, Edit, Full |
| LIST\_BILLOFDISTRIBUTION | Bill Of Distribution | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_BILLOFMATERIALSINQUIRY | Bill Of Materials Inquiry | Assembly Items | None, View, Create, Edit, Full |
| LIST\_BOM | Bill of Materials | Assembly Items | None, View, Create, Edit, Full |
| LIST\_BILLCAPTURE | Scanned Vendor Bills | \- | None, View, Create, Edit, Full |
| LIST\_BIN | Bins | Accounting | None, View, Create, Edit, Full |
| LIST\_BONUS | Bonus | \- | View, None, Create, Full, Edit |
| LIST\_BONUSTYPE | Bonus Types | \- | View, None, Create, Full, Edit |
| LIST\_CALENDAR | Calendar | Calendar Preferences | None, View, Create, Edit, Full |
| LIST\_CALL | Phone Calls | Phone Calls | None, View, Create, Edit, Full |
| LIST\_CAMPAIGN | Marketing Campaigns | Marketing Automation | None, View, Create, Edit, Full |
| LIST\_CAMPAIGNHISTORY | Campaign History | Marketing Automation | None, View, Create, Edit, Full |
| LIST\_CARDHOLDERAUTHENTICATION | Cardholder Authentications | Credit Card Payments | None, View, Edit, Full, Create |
| LIST\_CARDHOLDERAUTHEVENT | Cardholder Authentication Events | Credit Card Payments | None, View, Edit, Full, Create |
| LIST\_CASE | Cases | Customer Support and Service | None, View, Create, Edit, Full |
| LIST\_CASE\_DUPLICATES | Duplicate Case Management |  | None, Full |
| LIST\_CATEGORY | Expense Categories | Expense Reports | None, View, Create, Edit, Full |
| LIST\_CERTIFICATES | Certificate Access | \- | None, View, Create, Edit, Full |
| LIST\_CHECKITEMAVAILABILITY | Check Item Availability | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_CLASS | Classes | Classes | None, View, Create, Edit, Full |
| LIST\_COLORTHEME | Color Themes | SuiteCommerce | None, View, Create, Edit, Full |
| LIST\_COMMISSIONRULES | Employee Commission Schedules/Plans | Employee Commissions | None, View, Create, Edit, Full |
| LIST\_COMPANY | Companies | Customer Relationship Management | None, View, Create, Edit, Full |
| LIST\_COMPETITOR | Competitors | Sales Force Automation | None, View, Create, Edit, Full |
| LIST\_COMPONENTWHEREUSEDINQUIRY | Component Where Used | Assembly Items | None, View, Create, Edit, Full |
| LIST\_CONTACT | Contacts | Contacts | None, View, Create, Edit, Full |
| LIST\_CONTACTROLE | Contact Roles | Sales Force Automation | None, View, Create, Edit, Full |
| LIST\_CONTACTSUBSIDIARYRELATION | Contact-Subsidiary Relationship | \- | None, View |
| LIST\_CONVERTLEAD | Lead Conversion | \- | View, None, Create, Full, Edit |
| LIST\_COSTEDBOMINQUIRY | Costed Bill Of Materials Inquiry | Assembly Items | None, View, Create, Edit, Full |
| LIST\_CRMGROUP | CRM Groups | Customer Relationship Management | None, View, Create, Edit, Full |
| LIST\_CRMMESSAGE | Track Messages | Customer Relationship Management | None, View, Create, Edit, Full |
| LIST\_CRMTEMPLATE | Marketing Template | Marketing Automation | None, View, Create, Edit, Full |
| LIST\_CURRENCY | Currency | Multiple Currencies | None, View, Create, Edit, Full |
| LIST\_CUSTJOB | Customers | Prospects and Contacts | None, View, Create, Edit, Full |
| LIST\_CUSTPROFILE | Customer Profile | Customer Profile | None, View, Create, Edit, Full |
| LIST\_CUSTRECORDENTRY | Custom Record Entries | Custom Records | None, View, Create, Edit, Full |
| LIST\_DEPARTMENT | Departments | Departments | None, View, Create, Edit, Full |
| LIST\_DISTRIBUTIONNETWORK | Distribution Network | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_EARLIEST\_AVAILABILITY | Earliest Availability | Supply Allocation | None, View, Create, Edit, Full |
| LIST\_EMAILTEMPLATE | Email Template | Email Template | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE | Employees | Employees | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE\_ACCESS | Employee Access Tab | Advanced Employee Permissions | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE\_ADMINISTRATION | Employee Administration | Advanced Employee Permissions | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE\_CONFIDENTIAL | Employee Confidential | Advanced Employee Permissions | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE\_PUBLIC | Employee Public | Advanced Employee Permissions | None, View, Create, Edit, Full |
| LIST\_EMPLOYEE\_RECORD | Employee Record | \- | View, Create, Edit, Full |
| LIST\_EMPLOYEE\_SELF | Employee Self | Advanced Employee Permissions | View, Create, Edit, Full |
| LIST\_EMPLOYEECHANGETYPE | Employee Change Request Type | \- | None, View, Create, Edit, Full |
| LIST\_EMPLOYEECHANGEREASON | Employee Change Reason | Effective Dating | None, View, Create, Edit, Full |
| LIST\_EMPLOYEECHANGEREQUEST | Employee Change Request | Employee Change Requests | None, View, Create, Edit, Full |
| LIST\_EMPLOYEECHANGETYPE | Employee Change Request Type | Employee Change Requests | None, View, Create, Edit, Full |
| LIST\_EMPLOYEEEFFECTIVEDATING | Employee Effective Dating | Effective Dating | None, View, Create, Edit, Full |
| LIST\_EMPLOYEESEPARATION | Termination Reasons | Termination Reason Tracking | None, View, Create, Edit, Full |
| LIST\_EMPLOYEESSN | Employee Social Security Numbers | Employees | None, View, Full |
| LIST\_ENTITY\_DUPLICATES | Duplicate Entity Management | Duplicate Detection & Merge | None, View, Full |
| LIST\_EVENT | Events | Events | None, View, Create, Edit, Full |
| LIST\_EXPENSEAMORTIZATIONRULE | Expense Amortization Rule | \- | None, View, Create, Edit, Full |
| LIST\_EXPENSEPLAN | Expense Amortization Plan | \- | None, View, Create, Edit, Full |
| LIST\_EXPORT | Export Lists | Search Result Export | None, Create |
| LIST\_FAIRVALUEDIMENSION | Fair Value Dimension | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_FAIRVALUEFORMULA | Fair Value Formula | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_FAIRVALUEPRICE | Fair Value Price | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_FAXMESSAGE | Fax Messages | Communications | None, View, Create, Edit, Full |
| LIST\_FAXTEMPLATE | Fax Template | Mail Merge | None, View, Create, Edit, Full |
| LIST\_FILECABINET | Documents and Files | File Cabinet | None, View, Create, Edit, Full |
| LIST\_FIND | Perform Search | Order Management | None, View, Full |
| LIST\_FINHISTORY | Financial History |  | None, View, Create, Edit, Full |
| LIST\_FISCALCALENDAR | Fiscal Calendars | Accounting | None, View, Create, Edit, Full |
| LIST\_GENERAL\_TOKEN | General Token | Payment Instruments | None, View, Create, Edit, Full |
| LIST\_GENERICRESOURCE | Generic Resources | Project Management | None, View, Create, Edit, Full |
| LIST\_GIFT\_CERTIFICATE | Gift Certificate | \- | None, View, Create, Edit, Full |
| LIST\_GLLINESAUDITLOG | Custom GL Lines Plug-in Audit Log | Custom GL Lines Plug-in | None, View, Create, Edit, Full |
| LIST\_GLLINESAUDITLOGSEG | Custom GL Lines Plug-in Audit Log (Segments) | Custom GL Lines Plug-in | None, View, Create, Edit, Full |
| LIST\_GLOBALINVTRELATIONSHIP | Global Inventory Relationship | \- | None, View, Create, Edit, Full |
| LIST\_GOVERNMENTISSUEDIDTYPE | Government-Issued ID Types | Advanced Government-Issued ID Tracking | None, View, Create, Edit, Full |
| LIST\_HCMJOB | HCMJob Management | \- | None, View, Create, Edit, Full |
| LIST\_HCMPOSITION | Positions | \- | None, View, Create, Edit, Full |
| LIST\_HISTORY | Notes Tab | Communications | None, View, Create, Edit, Full |
| LIST\_IMPORTED\_EMPLOYEE\_EXPENSE | Imported Employee Expenses | Expense Reports | View, None |
| LIST\_INBOUNDSHIPMENT | Inbound Shipment | Inbound Shipment Management | None, View, Create, Edit, Full |
| LIST\_INFOCATEGORY | Store Content Categories | Web Store | None, View, Create, Edit, Full |
| LIST\_INFOITEM | Store Content Items | SuiteCommerce | None, View, Create, Edit, Full |
| LIST\_INFOITEMFORM | Publish Forms | SuiteCommerce | None, View, Create, Edit, Full |
| LIST\_INTEGRAPP | Integration Applications | SuiteTalk | None, View, Create, Edit, Full |
| LIST\_INTERNALPUBLISH | Internal Publisher |  | None, View, Create, Edit, Full |
| LIST\_INVCOSTTEMPLATE | Inventory Cost Template | Multi-Book Accounting | None, View, Create, Edit, Full |
| LIST\_INVENTORYSTATUS | Inventory Status | Inventory Management | None, View, Create, Edit, Full |
| LIST\_ISSUE | Issues | Issue Management | None, View, Create, Edit, Full |
| LIST\_ITEM | Items | Item Record Management | None, View, Create, Edit, Full |
| LIST\_ITEM\_COLLECTION | Item Collection | \- | None, View, Create, Edit, Full |
| LIST\_ITEMDEMANDPLAN | Item Demand Plan | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_ITEMREVENUECATEGORY | Item Revenue Category | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_ITEMPROCESSFAMILY | Item Process Family | Warehouse Management | None, View, Create, Edit, Full |
| LIST\_ITEMPROCESSGROUP | Item Process Group | Warehouse Management | None, View, Create, Edit, Full |
| LIST\_ITEM\_REVISION | Item Revisions | Item Record Management | None, View, Create, Edit, Full |
| LIST\_ITEMSUPPLYPLAN | Item Supply Plan | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_ITEMTEMPLATE | Item Templates |  | None, View, Create, Edit, Full |
| LIST\_JOB | Jobs | Projects | None, View, Create, Edit, Full |
| LIST\_JOBREQUISITION | HCMJob Requisitions | Job Requisitions | None, View, Create, Edit, Full |
| LIST\_KEYS | Key access | \- | None, View, Create, Edit, Full |
| LIST\_KUDOS | Kudos | Kudos | None, View, Create, Edit, Full |
| LIST\_KNOWLEDGEBASE | Knowledge Base | Knowledge Base | None, View, Create, Edit, Full |
| LIST\_LABORCOSTING | Labor Costing | Labor Costing | View, None, Full, Create, Edit |
| LIST\_LICENSEPLATE | License Plate | \- | View, None, Full, Create, Edit |
| LIST\_LOCATION | Locations | Locations | None, View, Create, Edit, Full |
| LIST\_MAILMERGE | Mail Merge | Mail Merge | None, View, Create, Edit, Full |
| LIST\_MAILMESSAGE | Letter Messages | Communications | None, View, Create, Edit, Full |
| LIST\_MAILTEMPLATE | Letter Template | Mail Merge | None, View, Create, Edit, Full |
| LIST\_MASSUPDATES | Mass Updates | Mass Update | None, View, Create, Edit, Full |
| LIST\_MATERIALREQUIREMENTSPLAN | Material Requirements Planning | Material Requirements Planning | View, None, Full, Create, Edit |
| LIST\_MEDIAITEMFOLDER | Media Folders | File Cabinet | None, View, Create, Edit, Full |
| LIST\_MEMDOC | Memorized Transactions | Transactions | None, View, Create, Edit, Full |
| LIST\_MESSAGE\_UNRESTRICTED | Messages for Analytics and REST | Email | None, View |
| LIST\_MFGCOSTTEMPLATE | Manufacturing Cost Template | Inventory Management | None, View, Create, Edit, Full |
| LIST\_MFGROUTING | Manufacturing Routing | Inventory Management | None, View, Create, Edit, Full |
| LIST\_NEWSITEM | News Items | \- | None, View, Create, Edit, Full |
| LIST\_NOTIFICATION | Notifications | \- | None, View, Create, Edit, Full |
| LIST\_ORDER\_REALLOCATION | Commit Orders | Advanced Inventory Management | None, View, Create, Edit, Full |
| LIST\_ORDERMANAGEDASHBOARD | Order Management Dashboard | Sales Channel Allocation | None, View, Create, Edit, Full |
| LIST\_ORGANIZATIONVALUE | Organizational Value | Kudos | None, View, Create, Edit, Full |
| LIST\_OTHERNAME | Other Names | Sales Force Automation | None, View, Create, Edit, Full |
| LIST\_OUTBOUNDREQUEST | Outbound Request | \- | None, View, Create, Edit, Full |
| LIST\_OVERTIMEPOLICY | Overtime Policies |  | None, View, Create, Edit, Full |
| LIST\_PA\_RECORDS | Product Analytics Records | \- | None, View, Create, Edit, Full |
| LIST\_PARTNER | Partners | Partner Relationship Management | None, View, Create, Edit, Full |
| LIST\_PARTNERCOMMISSNRULES | Partner Commission Schedules/Plans | Partner Commissions/Royalties | None, View, Create, Edit, Full |
| LIST\_PAYCHECK | Paychecks | Payroll | None, View, Create, Edit, Full |
| LIST\_PAYMENT\_CARD | Payment Card | Payment Instruments | None, View, Create, Edit, Full |
| LIST\_PAYMENT\_CARD\_TOKEN | Payment Card Token | Payment Instruments | None, View, Create, Edit, Full |
| LIST\_PAYMENT\_INSTRUMENTS | Payment Instruments | Payment Instruments | None, View, Create, Edit, Full |
| LIST\_PAYMETH | Payment Methods | Order Management | None, View, Create, Edit, Full |
| LIST\_PAYROLLITEM | Payroll Items | Payroll | None, View, Create, Edit, Full |
| LIST\_PDFMESSAGE | PDF Messages | Communications | None, View, Create, Edit, Full |
| LIST\_PDFTEMPLATE | PDF Template | Mail Merge | None, View, Create, Edit, Full |
| LIST\_PHASEDPROCESS | Phased Processes |  | None, View, Create, Edit, Full |
| LIST\_PICKDECOMPOSITION | Units for Pick Decomposition | \- | None, View, Create, Edit, Full |
| LIST\_PICKSTRATEGY | Pick Strategy | Warehouse Management | None, View, Create, Edit, Full |
| LIST\_PICKTASK | Pick Task | Warehouse Management | None, View, Create, Edit, Full |
| LIST\_PLANNEDREVENUE | Planned Revenue | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_PLANNEDSTANDARDCOST | Planned Standard Cost | Item Record Management | None, View, Create, Edit, Full |
| LIST\_PRESCATEGORY | Presentation Categories | SuiteCommerce | None, View, Create, Edit, Full |
| LIST\_PRICEBOOK | Price Books | \- | None, View, Create, Edit, Full |
| LIST\_PRICEPLAN | Price Plans | \- | None, View, Create, Edit, Full |
| LIST\_PRICINGRECORDS | Pricing Records | \- | None, View, Create, Edit, Full |
| LIST\_PROJECT\_BUDGET | Project Budget | Advanced Project Budgets | None, View, Create, Edit, Full |
| LIST\_PROJECTREVENUERULE | Project Revenue Rules | Project Management | None, View, Create, Edit, Full |
| LIST\_PROJECTTASK | Project Tasks | Project Management | None, View, Create, Edit, Full |
| LIST\_PROJECTTEMPLATE | Project Templates | Project Management | None, View, Create, Edit, Full |
| LIST\_PROMOTIONCODE | Promotion | Sales Force Automation | None, View, Create, Edit, Full |
| LIST\_PUBLISHSEARCH | Publish Search | Publishing Search Results | None, View, Create, Edit, Full |
| LIST\_QUANTITYPRICINGSCHEDULE | Quantity pricing Schedules | Quantity Pricing | None, View, Create, Edit, Full |
| LIST\_REALLOCATE\_ORDER\_ITEM | Reallocate Order Item | Supply Allocation | View, None, Full, Create, Edit |
| LIST\_RECOGNITIONEVENTTYPE | Custom Recognition Event Type | Advanced Revenue Recognition Or Advanced Expense Management | None, View, Create, Edit, Full |
| LIST\_RECORDCUSTFIELD | Record Custom Field |  | None, View, Create, Edit, Full |
| LIST\_RELATEDITEMS | Related Items | Web Site | None, View, Create, Edit, Full |
| LIST\_RESOURCE | Resource | Project Management | None, View, Create, Edit, Full |
| LIST\_RESOURCEGROUP | Resource Groups | Project Management | None, View, Create, Edit, Full |
| LIST\_REVENUEELEMENT | Revenue Element | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_REVENUEPLAN | Revenue Recognition Plan | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_REVENUERECOGNITIONRULE | Revenue Recognition Rule | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_REVRECSCHEDULE | Revenue Recognition Schedules | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_REVRECTREATMENT | Recognition Treatment | \- | None, View, Create, Edit, Full |
| LIST\_REVRECTREATMENTRULE | Recognition Treatment Rule | \- | None, View, Create, Edit, Full |
| LIST\_REVRECFIELDMAPPING | Revenue Recognition Field Mapping | Revenue Recognition | None, View, Create, Edit, Full |
| LIST\_REVRECVSOE | Revenue Management VSOE | VSOE | None, View, Create, Edit, Full |
| LIST\_RSRCALLOCATION | Resource Allocations | Project Management | None, View, Create, Edit, Full |
| LIST\_RSRCALLOCATIONAPPRV | Resource Allocation Approval | Project Management | None, View, Create, Edit, Full |
| LIST\_RSSFEED | Publish RSS Feeds | \- | None, View, Create, Edit, Full |
| LIST\_SAASMETRIC | SaaS Metric | \- | None, View, Create, Edit, Full |
| LIST\_SALESCAMPAIGN | Sales Campaigns | Sales Campaigns | None, View, Create, Edit, Full |
| LIST\_SALESROLE | Sales Roles | Team Selling | None, View, Create, Edit, Full |
| LIST\_SCHEDULEMASSUPDATES | Schedule Mass Updates | \- | None, View, Create, Edit, Full |
| LIST\_SCSNAPSHOT | Supply Chain Snapshot List | \- | None, View, Create, Edit, Full |
| LIST\_SENTEMAIL | Sent Email | Sent Email List | None, View, Create, Edit, Full |
| LIST\_SHIPITEM | Shipping Items | Accounting | None, View, Create, Edit, Full |
| LIST\_SHIPPARTPACKAGE | Shipping Partner Package | Order Management | None, View, Create, Edit, Full |
| LIST\_SHIPPARTREGISTRATION | Shipping Partner Registration | Order Management | None, View, Create, Edit, Full |
| LIST\_SHIPPARTSHIPMENT | Shipping Partner Shipment | Order Management | None, View, Create, Edit, Full |
| LIST\_SHORTCUT | Shortcuts | \- | None, View, Create, Edit, Full |
| LIST\_SITEEMAILTEMPLATE | Web Store Email Template | SuiteCommerce | None, View, Create, Edit, Full |
| LIST\_STANDARDCOSTVERSION | Standard Cost Version | Item Record Management | None, View, Create, Edit, Full |
| LIST\_STORECATEGORY | Store Categories | Web Store | None, View, Create, Edit, Full |
| LIST\_STOREITEMLISTLA | Item/Category Layouts | Web Store | None, View, Create, Edit, Full |
| LIST\_STORETAB | Store Tabs | Web Store | None, View, Create, Edit, Full |
| LIST\_SUBSCRIPTION | Subscriptions | Advanced Subscription Billing | None, View, Create, Edit, Full |
| LIST\_SUBSCRIPTIONCHANGEORDER | Subscription Change Orders | Advanced Subscription Billing | None, View, Create, Edit, Full |
| LIST\_SUBSCRIPTIONPLAN | Subscription Plan | Advanced Subscription Billing | None, View, Create, Edit, Full |
| LIST\_SUBSIDIARY | Subsidiaries | Subsidiaries | None, View, Create, Edit, Full |
| LIST\_SUPPLY\_REALLOCATION | Allocate Orders | \- | None, View, Create, Edit, Full |
| LIST\_SYSTEMNOTES | System Notes for Analytics and REST | System Notes | None, View |
| LIST\_SYSTEMEMAILTEMPLATE | System Email Template | Customer Relationship Management | None, View, Create, Edit, Full |
| LIST\_TALENT\_ADMINISTRATION | Talent Administration | \- | View, Full |
| LIST\_TALENT\_EMPLOYEE | Talent Employee | \- | None, Full |
| LIST\_TASK | Tasks | Customer Relationship Management | None, View, Create, Edit, Full |
| LIST\_TAXDETAILSTAB | Tax Details Tab | Tax Overhauling | None, View, Edit, Full |
| LIST\_TAXENGINESELECTION | Subsidiary Tax Registrations Tab | Tax Overhauling | None, View, Edit, Full |
| LIST\_TAXITEM | Tax Records | Accounting | None, View, Create, Edit, Full |
| LIST\_TAXSCHEDULE | Tax Schedules | Advanced Taxes | None, View, Create, Edit, Full |
| LIST\_TEGATAACCOUNT | Tegata Accounts | Accounting | None, View, Create, Edit, Full |
| LIST\_TEMPLATE\_CATEGORY | Template Categories | Email Marketing Campaigns | None, View, Create, Edit, Full |
| LIST\_TIMECODE | Time Codes | Overtime | None, View, Create, Edit, Full |
| LIST\_TIMEOFF | Time-Off | Time-Off Management | None, View, Create, Edit, Full |
| LIST\_TIMEOFFADMIN | Time-Off Administration | Time-Off Management | None, View, Create, Edit, Full |
| LIST\_TRANNUMBERAUDITLOG | Access to transaction numbering audit log | Transactions | None, View, Create, Edit, Full |
| LIST\_UNDELIVEREDEMAIL | Undelivered Emails | \- | None, View |
| LIST\_UNIT | Units | Accounting | None, View, Create, Edit, Full |
| LIST\_UPSELL | Upsell Assistant | Upsell Manager | None, View, Create, Edit, Full |
| LIST\_UPSELLWIZARD | Upsell Wizard | Upsell Manager | None, View, Create, Edit, Full |
| LIST\_USAGE | Usage | Advanced Subscription Billing | None, View, Create, Edit, Full |
| LIST\_VENDOR | Vendors | Accounting | None, View, Create, Edit, Full |
| LIST\_VENDOR\_ACH | Vendor Automated Clearing House | \- | None, View, Create, Edit, Full |
| LIST\_WBS | Work Breakdown Structure | Advanced Project Budgets | None, View, Create, Edit, Full |
| LIST\_WEBSITE | Website (External) publisher | Web Site | None, View, Create, Edit, Full |
| LIST\_WORKASSIGNMENT | Work Assignments | \- | View, None, Full, Create, Edit |
| LIST\_WORKCALENDAR | Work Calendar | Project Management | None, View, Create, Edit, Full |
| LIST\_WORKPLACE | Workplaces | Payroll | None, View, Create, Edit, Full |
| LIST\_ZONE | Zone | Warehouse Management | None, View, Create, Edit, Full |
| REGT\_ACCTPAY | Accounts Payable Register | A/P | None, View, Create, Edit, Full |
| REGT\_ACCTREC | Accounts Receivable Register | A/R | None, View, Create, Edit, Full |
| REGT\_BANK | Bank Account Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_COGS | Cost of Goods Sold Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_CREDCARD | Credit Card Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_DEFEREXPENSE | Deferred Expense Registers | Amortization | None, View, Create, Edit, Full |
| REGT\_DEFERREVENUE | Deferred Revenue Registers | Revenue Recognition | None, View, Create, Edit, Full |
| REGT\_EQUITY | Equity Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_EXPENSE | Expense Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_FIXEDASSET | Fixed Asset Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_INCOME | Income Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_LONGTERMLIAB | Long Term Liability Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_NONPOSTING | Non Posting Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_OTHASSET | Other Asset Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_OTHCURRASSET | Other Current Asset Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_OTHCURRLIAB | Other Current Liability Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_OTHEXPENSE | Other Expense Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_OTHINCOME | Other Income Registers | Accounting | None, View, Create, Edit, Full |
| REGT\_PAYROLL | Run Payroll | Payroll | None, View, Create, Edit, Full |
| REGT\_STAT | Statistical Account Registers | Statistical Accounting | None, View, Create, Edit, Full |
| REGT\_UNBILLEDREC | Unbilled Receivable Registers | Revenue Commitments | None, View, Create, Edit, Full |
| REPO\_1099 | Form 1099 - Federal Miscellaneous Income | A/P | None, View, Create, Edit, Full |
| REPO\_940 | Form 940 - Employer's Annual Federal Unemployment Tax Return | Payroll | None, View |
| REPO\_941 | Form 941 - Employer's Quarterly Federal Tax Return | Payroll | None, View |
| REPO\_ACCOUNTDETAIL | Account Detail | Accounting | None, View |
| REPO\_AMORTIZATION | Amortization Reports | Amortization | None, View |
| REPO\_ANALYTICS | SuiteAnalytics Workbook | SuiteAnalytics Workbook | None, Edit |
| REPO\_AP | Accounts Payable | A/P | None, View |
| REPO\_AR | Accounts Receivable | A/R | None, View |
| REPO\_AUTHPARTNERCOMMISSION | Partner Authorized Commission Reports | Partner Commissions/Royalties | None, View |
| REPO\_BALANCESHEET | Balance Sheet | Accounting | None, View |
| REPO\_BOOKINGS | Sales Order Reports | Sales Force Automation | None, View |
| REPO\_BUDGET | Budget | Accounting | None, View |
| REPO\_CASHFLOW | Cash Flow Statement | Accounting | None, View |
| REPO\_COMMISSION | Commission Reports | Employee Commissions | None, View |
| REPO\_CONSOLIDATED\_REPORTING | Consolidated Reporting | \- | None, View |
| REPO\_CUSTOMIZATION | Report Customization | Report Customization | None, View |
| REPO\_DEFERREDEXPENSE | Deferred Expense Reports | \- | None, View |
| REPO\_FINANCIALS | Financial Statements | Accounting | None, View |
| REPO\_GL | General Ledger | Accounting | None, View |
| REPO\_GRANT\_ACCESS | Granting access to Reports |  | None, View, Create, Edit, Full |
| REPO\_GSTSUMMARY | GST Summary Report |  | None, View |
| REPO\_INTEGRATION | Integration | SuiteTalk | None, View |
| REPO\_INVENTORY | Inventory | Inventory | None, View |
| REPO\_ISSUE | Issue Reports | Issue Management | None, View |
| REPO\_MARKETING | Marketing Campaign Reports | Marketing Automation | None, View |
| REPO\_NONPOSTING | Sales Order Transaction Report | Order Management | None, View |
| REPO\_PANDL | Income Statement | Accounting | None, View |
| REPO\_PARTNERCOMMISSION | Partner Commission Reports | Partner Commissions/Royalties | None, View |
| REPO\_PAYCHECKDETAIL | Payroll Check Register | Payroll | None, View |
| REPO\_PAYROLL | Payroll Summary & Detail Reports | Payroll | None, View |
| REPO\_PAYROLLHIDEFINEMPINFO | Hide Employee Information on Financial Reports | Payroll | None, View |
| REPO\_PAYROLLHOURSEARNING | Payroll Hours & Earnings | Payroll | None, View |
| REPO\_PAYROLLJOURNAL | Payroll Journal Report | Payroll | None, View |
| REPO\_PAYROLLLIAB | Payroll Liability Report | Payroll | None, View |
| REPO\_PAYROLLSTATEWITHHOLD | Payroll State Withholding | Payroll | None, View |
| REPO\_PAYROLLW2 | Form W-2 - Wage and Tax Statement | Payroll | None, View, Create, Edit, Full |
| REPO\_PERIODENDFINANCIALS | Period End Financial Statements | \- | None, View |
| REPO\_PROJECT\_ACCOUNTING | Project Accounting | Accounting | None, View |
| REPO\_PSTSUMMARY | PST Summary Report |  | None, View |
| REPO\_PURCHASEORDER | Purchase Order Reports | Purchase Orders | None, View |
| REPO\_PURCHASES | Purchases | Accounting | None, View |
| REPO\_QUOTA | Quota Reports | Sales Force Automation | None, View |
| REPO\_RECONCILE | Reconcile Reporting | Accounting | None, View |
| REPO\_REMINDEREMPLOYEE | Employee Reminders | Employees | None, View |
| REPO\_RETURNAUTH | Return Authorization Reports | Return Authorizations | None, View |
| REPO\_REVREC | Revenue Recognition Reports | Revenue Recognition | None, View |
| REPO\_RSRCALLOCATION | Resource Allocation Reports | Project Management | None, View |
| REPO\_SALES | Sales | Sales Force Automation | None, View |
| REPO\_SALESORDER | Sales Order Fulfillment Reports | Sales Orders | None, View |
| REPO\_SALES\_PARTNER | Sales By Partner | Partner Relationship Management | None, View |
| REPO\_SALES\_PROMO | Sales By Promotion Code | Sales Force Automation | None, View |
| REPO\_SALES\_PROMO | Sales By Promotion | Sales Force Automation | None, View |
| REPO\_SCHEDULE | Report Scheduling | Reports | None, Full |
| REPO\_SNAPSHOTCASE | Support Case Snapshot/Reminders | Support | None, View |
| REPO\_SNAPSHOTLEAD | Lead Snapshot/Reminders | Business | None, View |
| REPO\_SFA | Sales Force Automation | Customer Relationship Management | None, View |
| REPO\_SUPPORT | Support | Customer Support and Service | None, View |
| REPO\_TAX | Tax | Accounting | None, View |
| REPO\_TAXREPORTS | Tax Reports | Accounting | None, View |
| REPO\_TIME | Time Tracking | Time Tracking | None, View |
| REPO\_TRAN | Transaction Detail | Transactions | None, View |
| REPO\_TRIALBALANCE | Trial Balance | Accounting | None, View |
| REPO\_UNBILLED | Accounts Receivable Un-Billed | Accounting | None, View |
| REPO\_W4 | Form W4 - Employee's Withholding Allowance Certificate | Payroll | None, View |
| REPO\_WEBSITE | Web Site Report | Web Site | None, View |
| REPO\_WEBSTORE | Web Store Report | Web Store | None, View |
| REPO\_WORKFORCEANALYTICS | Workforce Analytics | Workforce Analytics | View |
| TRAN\_ADJUSTMENTJOURNAL | Currency Adjustment Journal | Accounting | None, View, Create, Edit, Full |
| TRAN\_ALLOCSCHEDULE | Create Allocation Schedules | Expense Allocation | None, View, Create, Edit, Full |
| TRAN\_AMENDW4 | Amend W-4 | Employees | None, View, Create, Edit, Full |
| TRAN\_APPROVECOMMISSN | Employee Commission Transaction Approval | Employee Commissions | None, View, Create, Edit, Full |
| TRAN\_APPROVEDD | Approve Direct Deposit | Direct Deposit | None, View, Create, Edit, Full |
| TRAN\_APPROVEPARTNERCOMM | Partner Commission Transaction Approval | Partner Commissions/Royalties | None, View, Create, Edit, Full |
| TRAN\_AUDIT | Audit Trail | Transactions | None, View, Create, Edit, Full |
| TRAN\_AUTO\_CASH | Automated Cash Application | Accounting | None, Full |
| TRAN\_BALANCEOVERVIEW | Balance Overview | Intercompany Framework | None, View |
| TRAN\_BALJRNAL | Balancing Journals | \- | None, View, Create, Full |
| TRAN\_BINTRNFR | Bin Transfer | Bin Management | None, View, Create, Edit, Full |
| TRAN\_BINWKSHT | Bin Putaway Worksheet | Bin Management | None, View, Create, Edit, Full |
| TRAN\_BLANKORD | Blanket Purchase Order | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_BLANKORDAPPRV | Blanket Purchase Order Approval | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_BUDGET | Set Up Budgets | Accounting | None, View, Create, Edit, Full |
| TRAN\_BUILD | Build Assemblies | Assembly Items | None, View, Create, Edit, Full |
| TRAN\_CARDCHRG | Credit Card | Accounting | None, View, Create, Edit, Full |
| TRAN\_CARDHOLDERAUTHENTICATION | Cardholder Authentication | Credit Card Payments | None, View, Edit, Full, Create |
| TRAN\_CARDHOLDERAUTHEVENT | Cardholder Authentication Event | Credit Card Payments | None, View, Edit, Full, Create |
| TRAN\_CARDRFND | Credit Card Refund | Accounting | None, View, Create, Edit, Full |
| TRAN\_CASHRFND | Cash Sale Refund | Accounting | None, View, Create, Edit, Full |
| TRAN\_CASHSALE | Cash Sale | Accounting | None, View, Create, Edit, Full |
| TRAN\_CHARGE | Charge | Project Management | None, View, Create, Edit, Full |
| TRAN\_CHARGERULE | Charge Rule | Project Management | None, View, Create, Edit, Full |
| TRAN\_CHECK | Check | Accounting | None, View, Create, Edit, Full |
| TRAN\_CLEARHOLD | Override Payment Hold | Order Management | None, View, Create, Edit, Full |
| TRAN\_COMMISSN | Employee Commission Transaction | Employee Commissions | None, View, Create, Edit, Full |
| TRAN\_COMMITPAYROLL | Commit Payroll | Payroll | None, View, Create, Edit, Full |
| TRAN\_COPY\_BUDGET | Copy Budgets | Accounting | None, View, Create, Edit, Full |
| TRAN\_CREATEINVCOUNT | Create Inventory Counts | Inventory Count | None, View, Create, Edit, Full |
| TRAN\_CUSTAUTH | Customer Payment Authorization | Customer Payment Authorizations | None, View, Create, Edit, Full |
| TRAN\_CUSTCHRG | Statement Charge | A/R | None, View, Create, Edit, Full |
| TRAN\_CUSTCRED | Credit Memo | A/R | None, View, Create, Edit, Full |
| TRAN\_CUSTDEP | Customer Deposit | A/R | None, View, Create, Edit, Full |
| TRAN\_CUSTINVC | Invoice | A/R | None, View, Create, Edit, Full |
| TRAN\_CUSTINVCAPPRV | Invoice Approval | Order Management | None, View, Create, Edit, Full |
| TRAN\_CUSTPYMT | Customer Payment | A/R | None, View, Create, Edit, Full |
| TRAN\_CUSTRFND | Customer Refund | A/R | None, View, Create, Edit, Full |
| TRAN\_DEPAPPL | Deposit Application | A/R | None, View, Create, Edit, Full |
| TRAN\_DEPOSIT | Deposit | Accounting | None, View, Create, Edit, Full |
| TRAN\_DLTD\_TXNS\_SUMMARY\_SBMSN | Archive and Purge Submissions | \- | None, Full |
| TRAN\_EDITBANKINGINFO | Personal Banking Information | \- | None, View, Full |
| TRAN\_EDITPROFILE | Edit Profile | Employees | None, View, Create, Edit, Full |
| TRAN\_ESTIMATE | Estimate | Estimates | None, View, Create, Edit, Full |
| TRAN\_ESTIMATEDCOSTOVERRIDE | Override Estimated Cost on Transactions |  | None, Full |
| TRAN\_EXPREPT | Expense Report | Expense Reports | None, View, Create, Edit, Full |
| TRAN\_FFTREQ | Fulfillment Request | Order Management | None, View, Create, Edit, Full |
| TRAN\_FINCHRG | Finance Charge | A/R | None, View, Create, Edit, Full |
| TRAN\_FIND | Find Transaction | Transactions | None, View, Create, Edit, Full |
| TRAN\_FORECAST | Edit Forecast | Sales Force Automation | None, View, Create, Edit, Full |
| TRAN\_FXREVAL | Currency Revaluation | Multiple Currencies | None, View, Create, Edit, Full |
| TRAN\_GST\_REFUND | Process GST Refund | Accounting | None, View, Create, Edit, Full |
| TRAN\_IMPORTOLBFILE | Import Online Banking (QIF) File | Accounting | None, View, Create, Edit, Full |
| TRAN\_INTERCOADJ | Intercompany Adjustments | Accounting | None, View, Create, Edit, Full |
| TRAN\_INVADJST | Adjust Inventory | Inventory | None, View, Create, Edit, Full |
| TRAN\_INVCOUNT | Count Inventory | Advanced Inventory Management | None, View, Create, Edit, Full |
| TRAN\_INVDISTR | Distribute Inventory | Multi-Location Inventory | None, View, Create, Edit, Full |
| TRAN\_INVREVAL | Revalue Inventory Cost | Inventory | None, View, Create, Edit, Full |
| TRAN\_INVTRNFR | Transfer Inventory | Multi-Location Inventory | None, View, Create, Edit, Full |
| TRAN\_INVWKSHT | Adjust Inventory Worksheet | Inventory | None, View, Create, Edit, Full |
| TRAN\_ITEMRCPT | Item Receipt | Advanced Receiving | None, View, Create, Edit, Full |
| TRAN\_ITEMSHIP | Item Fulfillment | Advanced Shipping | None, View, Create, Edit, Full |
| TRAN\_JOURNAL | Make Journal Entry | Accounting | None, View, Create, Edit, Full |
| TRAN\_JOURNALAPPRV | Journal Approval | Accounting | None, View, Create, Edit, Full |
| TRAN\_LIABPYMT | Payroll Liability Payments | Payroll | None, View, Create, Edit, Full |
| TRAN\_MANAGEPAYROLL | Manage Payroll | Payroll | None, View, Create, Edit, Full |
| TRAN\_MATCHING\_RULES | Matching Rules for Online Banking | Accounting | None, View, Create, Edit, Full |
| TRAN\_MGRFORECAST | Edit Manager Forecast | Sales Force Automation | None, View, Create, Edit, Full |
| TRAN\_NETTINGSETTLEMENTAPPRV | Netting Settlement Approval | Intercompany Framework | None, Edit |
| TRAN\_NETTSTLM | Netting Settlement | Intercompany Framework | None, View, Create, Edit, Full |
| TRAN\_OPENBAL | Enter Opening Balances | Accounting | None, View, Create, Edit, Full |
| TRAN\_OPPRTNTY | Opportunity | Opportunities | None, View, Create, Edit, Full |
| TRAN\_ORDERRESERVATION | Order Reservation | \- | None, View, Edit, Full, Create |
| TRAN\_ORDRESVAPPRV | Approve Order Reservation |  | None, View, Create, Edit, Full |
| TRAN\_OWNTRNSF | Ownership Transfer | \- | None, View, Create, Edit, Full |
| TRAN\_PARTNERCOMMISSN | Partner Commission Transaction | Partner Commissions/Royalties | None, View, Create, Edit, Full |
| TRAN\_PAYCHECK | Individual Paycheck | Payroll | None, View, Create, Edit, Full |
| TRAN\_PAYMENTAUDIT | Access Payment Audit Log | Order Management | None, View, Create, Edit, Full |
| TRAN\_PAYMENTEVENT | View Payment Events | Credit Card Payments | None, View, Create, Edit, Full |
| TRAN\_PAYMENTRESULTPREVIEW | View Payment Result Previews | Credit Card Payments | None, View, Edit, Full, Create |
| TRAN\_PAYROLLRUN | Process Payroll | Payroll | None, View, Create, Edit, Full |
| TRAN\_PCHKJRNL | Paycheck Journal | Employees | None, View, Create, Edit, Full |
| TRAN\_PEJRNL | Period End Journals | \- | None, View, Create, Edit, Full |
| TRAN\_POSTPERIODS | Posting Period on Transactions | Accounting | None, View, Create, Edit, Full |
| TRAN\_POSTVENDORBILLVARIANCE | Post Vendor Bill Variances | Vendors | None, View, Create, Edit, Full |
| TRAN\_PRICELIST | Generate Price Lists | Item Record Management | None, View, Create, Edit, Full |
| TRAN\_PRINTSHIPMENTDOCS | Print Shipment Documents | Shipping Partners | None, View, Create, Edit, Full |
| TRAN\_PROJECT\_IC\_CHARGE\_REQUEST | Project Intercompany Cross Charge Request | Project Intercompany Cross Charge Request | None, View, Create, Edit, Full |
| TRAN\_PURCHCON | Purchase Contract | Vendors | None, View, Create, Edit, Full |
| TRAN\_PURCHCONAPPRV | Purchase Contract Approval | Vendors | None, View, Create, Edit, Full |
| TRAN\_PURCHORD | Purchase Order | Purchase Orders | None, View, Create, Edit, Full |
| TRAN\_PURCHORDBILL | Bill Purchase Orders | Advanced Receiving | None, View, Create, Edit, Full |
| TRAN\_PURCHORDRECEIVE | Receive Order | Purchase Orders | None, View, Create, Edit, Full |
| TRAN\_PURCHREQ | Requisition | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_PURCHREQAPPRV | Requisition Approval | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_QUOTA | Establish Quotas | Sales Force Automation | None, View, Create, Edit, Full |
| TRAN\_RECOG\_GIFTCERT\_INCOME | Recognize Gift Certificate Income | Accounting | None, View, Create, Edit, Full |
| TRAN\_RECONCILE | Reconcile | Accounting | None, View, Create, Edit, Full |
| TRAN\_REVARRNG | Revenue Arrangement | Revenue Recognition | None, View, Create, Edit, Full |
| TRAN\_REVARRNGAPPRV | Revenue Arrangement Approval | Revenue Recognition | None, View, Create, Edit, Full |
| TRAN\_REVCOMM | Revenue Commitment | Revenue Commitments | None, View, Create, Edit, Full |
| TRAN\_REVCOMRV | Revenue Commitment Reversal | Revenue Commitments | None, View, Create, Edit, Full |
| TRAN\_REVCONTR | Revenue Contracts | Revenue Recognition | None, View, Create, Edit, Full |
| TRAN\_RFQ | Request For Quote | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_RTNAUTH | Return Authorization | Return Authorizations | None, View, Create, Edit, Full |
| TRAN\_RTNAUTHAPPRV | Return Auth. Approval | Return Authorizations | None, View, Create, Edit, Full |
| TRAN\_RTNAUTHCREDIT | Refund Returns | Order Management | None, View, Create, Edit, Full |
| TRAN\_RTNAUTHRECEIVE | Receive Returns | Order Management | None, View, Create, Edit, Full |
| TRAN\_RTNAUTHREVERSEREVCOMMIT | Generate Revenue Commitment Reversals | Revenue Commitments | None, View, Create, Edit, Full |
| TRAN\_SALESORD | Sales Order | Sales Orders | None, View, Create, Edit, Full |
| TRAN\_SALESORDAPPRV | Sales Order Approval | Sales Orders | None, View, Create, Edit, Full |
| TRAN\_SALESORDCOMMITREVENUE | Generate Revenue Commitment | Revenue Commitments | None, View, Create, Edit, Full |
| TRAN\_SALESORDFULFILL | Fulfill Orders | Order Management | None, View, Create, Edit, Full |
| TRAN\_SALESORDINVOICE | Invoice Sales Orders | Advanced Shipping | None, View, Create, Edit, Full |
| TRAN\_SALESORDREVENUECONTRACT | Generate Single Order Revenue Contracts | Revenue Recognition | None, View, Create, Edit, Full |
| TRAN\_STATEMENT | Generate Statements | A/R | None, View, Create, Edit, Full |
| TRAN\_STATCHNG | Inventory Status Change | Inventory Status | None, View, Create, Edit, Full |
| TRAN\_STATUSDD | Direct Deposit Status | Direct Deposit | None, View, Create, Edit, Full |
| TRAN\_STPICKUP | Store Pickup Fulfillment | SuiteCommerce InStore | None, View, Create, Edit, Full |
| TRAN\_SYSJRNL | System Journal | Accounting | None, View, Create, Edit, Full |
| TRAN\_TAXLIAB | Tax Liability Payment | Accounting | None, View, Create, Edit, Full |
| TRAN\_TAXPYMT | Pay Sales Tax | Accounting | None, View, Create, Edit, Full |
| TRAN\_TEGPYBL | Tegata Payable | Accounting | None, View, Create, Edit, Full |
| TRAN\_TEGRCVBL | Tegata Receivable | Accounting | None, View, Create, Edit, Full |
| TRAN\_TIMEBILL | Track Time | Time Tracking | None, View, Create, Edit, Full |
| TRAN\_TIMECALC | Calculate Time | Time Tracking | None, View, Create, Edit, Full |
| TRAN\_TIMEPOST | Post Time | Project Management | None, View, Create, Edit, Full |
| TRAN\_TIMER | Timer | Time Tracking | None, View, Create, Edit, Full |
| TRAN\_TRANSFER | Transfer Funds | Accounting | None, View, Create, Edit, Full |
| TRAN\_TRNFRORD | Transfer Order | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_TRNFRORDAPPRV | Transfer Order Approval | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_UNBUILD | Unbuild Assemblies | Assembly Items | None, View, Create, Edit, Full |
| TRAN\_VENDAUTH | Vendor Return Authorization | Vendor Return Authorizations | None, View, Create, Edit, Full |
| TRAN\_VENDAUTHAPPRV | Vendor Return Auth. Approval | Vendor Return Authorizations | None, View, Create, Edit, Full |
| TRAN\_VENDAUTHCREDIT | Credit Returns | Vendor Returns | None, View, Create, Edit, Full |
| TRAN\_VENDAUTHRETURN | Vendor Returns | Vendor Return Authorizations | None, View, Create, Edit, Full |
| TRAN\_VENDBILL | Bills | A/P | None, View, Create, Edit, Full |
| TRAN\_VENDBILLAPPRV | Vendor Bill Approval | Vendor Bills | None, View, Create, Edit, Full |
| TRAN\_VENDCRED | Enter Vendor Credits | A/P | None, View, Create, Edit, Full |
| TRAN\_VENDPYMT | Pay Bills | A/P | None, View, Create, Edit, Full |
| TRAN\_VENDPYMTAPPRV | Vendor Payment Approval | Vendor Bills | None, View, Create, Edit, Full |
| TRAN\_VENDRFQ | Vendor Request For Quote | Purchasing and Receiving | None, View, Create, Edit, Full |
| TRAN\_VPREPAPP | Vendor Prepayment Application | \- | None, View, Create, Edit, Full |
| TRAN\_VPREP | Vendor Prepayment | \- | None, View, Create, Edit, Full |
| TRAN\_WAVE | Wave | \- | None, View, Create, Edit, Full |
| TRAN\_WOCLOSE | Work Order Close | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WOCOMPL | Work Order Completion | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WOISSUE | Work Order Issue | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORD | Work Order | Work Orders | None, View, Create, Edit, Full |
| TRAN\_WORKORDBUILD | Build Work Orders | Work Orders | None, View, Create, Edit, Full |
| TRAN\_WORKORDCLOSE | Close Work Orders | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORDCOMPLETE | Enter Completions | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORDISSUE | Issue Components | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORDMARKBUILT | Mark Work Orders Built | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORDMARKFIRMED | Mark Work Orders Firmed | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_WORKORDMARKRELEASED | Mark Work Orders Released | Inventory Management | None, View, Create, Edit, Full |
| TRAN\_XCHGJRNL | Cross Charge Journal | Intercompany Framework | None, View |
| TRAN\_YTDADJST | Enter Year-To-Date Payroll Adjustments | Payroll | None, View, Create, Edit, Full |

### Related Topics

-   [SuiteScript IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494647249.html)
-   [Feature Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3247851.html)
-   [Preference Names and IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3251359.html)
-   [Task IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3269064.html)
-   [Button IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3265696.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
