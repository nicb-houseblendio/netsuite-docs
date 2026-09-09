---
id: "section_N3413913"
type: "section"
title: "NetSuite WSDL and XSD Structure"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > NetSuite WSDL and XSD Structure"
parent: "chapter_N3412777"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413913.html"
anchors: ["bridgehead_N3414015", "bridgehead_N3414193", "bridgehead_N3417653", "bridgehead_N3418061", "svg_1", "svg_1Background", "svg_1Layer_1", "svg_1Oval", "svg_1Oval_1_", "svg_1Swoopy_3", "svg_1Swoopy_2", "svg_1Swoopy_3_1_", "svg_1Swoopy_3_00000137114115186815859350000015997709724293470640_", "bridgehead_161598870606", "bridgehead_161598883228", "bridgehead_161598949069", "bridgehead_161599081573"]
sha256: "90915286370c1a52bc9ed22582f41ae4784300de020d65d8ed75b90687b097d3"
---

Important:

Oracle NetSuite has scheduled the gradual removal of SOAP web services from the product as part of ongoing efforts to provide modern integration channels.

The 2025.2 SOAP endpoint is the last planned SOAP endpoint and any later SOAP endpoints would be released only as necessary to meet business, technical, or other significant requirements.

The support period of older endpoints is also affected and with the 2027.1 release, only the 2025.2 endpoint will be supported. With the 2028.2 release, SOAP will no longer be available in NetSuite and existing SOAP integrations with NetSuite will stop working.

For more details, see the [SOAP Removal Plans FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2104046421.html). For a list of the currently supported endpoints, see [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html).

Also, see [Removal of SOAP Web Services](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1021357/kw/1021357).

**SuiteTalk REST web services** is the technology intended to replace SOAP. All newly built integrations should use REST web services with OAuth 2.0 for authentication.

-   For any custom integration applications, that you have developed using SOAP, you should start planning the migration of your solution to REST as soon as possible. For a detailed guide for the migration, see [SOAP Web Services To Rest Web Services Upgrade Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_8110600984.html).
    
-   If you use a partner SOAP application to integrate with NetSuite, consult with your partner to provide you with a REST-based application instead.
    
-   If you use an Oracle NetSuite integration application, a REST-based application will be provided by Oracle NetSuite.
    

SOAP web services use single WSDL file that describes all supported operations and messages. You can access that file at the following link:

[https://webservices.netsuite.com/wsdl/v2025\_2\_0/netsuite.wsdl](https://webservices.netsuite.com/wsdl/v2025_2_0/netsuite.wsdl)

You can also download a .zip version of the file at the following link:

[https://content.netsuite.com/download/WSDL\_v2025\_2\_0.zip](https://content.netsuite.com/download/WSDL_v2025_2_0.zip)

In these links, v2025\_2\_0 reflects the WSDL version.

NetSuite defines WSDL versioning, the location of schemas, namespaces, and the endpoint as follows:

          `WSDL: https://webservices.netsuite.com/wsdl/v2025_2_0/netsuite.wsdl     <xsd:import namespace="urn:core_2023_2_0.platform.webservices.netsuite.com"     schemaLocation="https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd"/>  <port name="NetSuitePort" binding="tns:NetSuiteBinding">    <soap:address location="https://webservices.netsuite.com/services/NetSuitePort_2023_2_0" />  </port>` 
        

Note:

For more information about WSDL versioning, upgrading, and testing, see [NetSuite WSDL Versioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418174.html). For information about WSDLs that pre-date 2025.2, see [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html).

The WSDL includes various NetSuite-specific types defined in related XSD files. Each XSD file has a corresponding alias that serves as a shortcut to its URL. The following tables show the organization of the XSD files.

Important:

NetSuite hosts customer accounts in multiple data centers. For that reason, the correct URL for SOAP web services access varies depending on the data center hosting the account.

For more details, see [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html).

Your integration **must** incorporate logic that dynamically determines the correct URL. You should use the [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) operation and the [The DataCenterUrls REST Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157011836591.html) to dynamically discover the correct domain URLs.

## Messaging XSD Files {#bridgehead_N3414015}

These files provide descriptions for the base SOAP web services functions used by all operations. For API documentation on each operation, see [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html).

| URL | Schema Alias | Notes |
| --- | --- | --- |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/common.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/common.xsd) | platformCommon | This file also includes descriptions for the following subrecords:
-   Address
-   InventoryDetail
-   LandedCost

 |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/core.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd) | platformCore | Among other elements, this file includes descriptions for the following complex types, which are used for authentication:

-   Passport
-   SsoPassport
-   TokenPassport

 |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/faults.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/faults.xsd) | platformFaults | \- |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/messages.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/messages.xsd) | platformMsgs | \- |

## Record Type Definitions {#bridgehead_N3414193}

The following XSD files provide descriptions for each record type in NetSuite. For field reference information about each record, see [SuiteTalk SOAP Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3634785.html). For general information about working with records in SOAP web services, see [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html).

| URL | Schema Alias | Record Types |
| --- | --- | --- |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/scheduling.xsd](https://webservices.netsuite.com/xsd/activities/v2025_2_0/scheduling.xsd) | actSched | 
ContactCategory

CustomerCategory

SalesRole

PriceLevel

WinLossReason

Term

NoteType

PaymentMethod

CalendarEvent

CalendarEventSearch

CalendarEventSearchAdvanced

Task

TaskSearch

TaskSearchAdvanced

PhoneCall

PhoneCallSearch

PhoneCallSearchAdvanced

ProjectTask

Resource Allocation



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/demandPlanning.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/demandPlanning.xsd) | demandPlanning | 

ItemDemandPlan

ItemSupplyPlan



 |
| [https://webservices.netsuite.com/xsd/documents/v2025\_2\_0/fileCabinet.xsd](https://webservices.netsuite.com/xsd/documents/v2025_2_0/fileCabinet.xsd) | docfileCab | 

File

FileSearch

FileSearchAdvanced

Folder

FolderSearch

FolderSearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/general/v2025\_2\_0/communication.xsd](https://webservices.netsuite.com/xsd/general/v2025_2_0/communication.xsd) | generalComm | 

Note

NoteSearch

NoteSearchAdvanced

Message

MessageSearch

MessageSearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/accounting.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) | listAcct | 

Billing Schedule

Bill of Materials (BOM)

BOM Revision

ContactCategory

CustomerCategory

SalesRole

PriceLevel

WinLossReason

Term

NoteType

PaymentMethod

LeadSource

Assembly Item (BOM Item)

DescriptionItem

DiscountItem

Download Item

GeneralToken

GiftCertificateItem

InventoryItem

ItemSearch

ItemSearchAdvanced

Kit/Package Item

Lot Numbered Assembly Item

Lot Numbered Inventory Item

MerchandiseHierarchyNode

MarkupItem

NonInventoryPurchaseItem

NonInventoryResaleItem

NonInventorySaleItem

OtherChargePurchaseItem

OtherChargeResaleItem

OtherChargeSaleItem

PaymentCard

PaymentCardToken

PaymentItem

SerializedAssemblyItem

Serialized Inventory Item

ServicePurchaseItem

ServiceResaleItem

ServiceSaleItem

SubtotalItem

Currency

ExpenseCategory

Account

AccountSearch

AccountSearchAdvanced

AccountingPeriod

Bin

BinSearch

BinSearchAdvanced

Classification

ClassificationSearch

ClassificationSearchAdvanced

Department

DepartmentSearch

DepartmentSearchAdvanced

Expense Category

Gift Certificate

FairValuePrice



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/accounting.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) | listAcct | 

GiftCertificateSearch

GiftCertificateSearchAdvanced

GlobalAccountMapping

Inventory Number

ItemAccountMapping

Location

LocationSearch

LocationSearchAdvanced

Nexus

Revenue Recognition Schedule

Revenue Recognition Template

Sales Tax ItemItemSearchAdvanced

ContactRole

Bin

SalesTaxItem

TaxAcct

TaxGroup

TaxType

Subsidiary

SubsidiarySearch

SubsidiarySearchAdvanced

UnitsType

PartnerCategory

VendorCategory



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/employees.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/employees.xsd) | listEmp | 

Employee

EmployeeSearch

EmployeeSearchAdvanced

HCM Job



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/marketing.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/marketing.xsd) | listMkt | 

Campaign

CampaignSearch

CampaignSearchAdvanced

CampaignCategory

CampaignAudience

CampaignFamily

CampaignSearchEngine

CampaignChannel

CampaignOffer

CampaignResponse

CampaignVertical

CampaignSubscription

PromotionCode

PromotionCodeSearch

PromotionCodeSearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/relationships.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationships.xsd) | listRel | 

Billing Account

Contact

ContactSearch

ContactSearchAdvanced

Customer

CustomerSearch

CustomerSearchAdvanced

CustomerStatus

CustomerSubsidiaryRelationship

Partner

PartnerSearch

PartnerSearchAdvanced

Vendor

VendorSearch

VendorSearchAdvanced

VendorSubsidiaryRelationship

EntityGroup

EntityGroupSearch

EntityGroupSearchAdvanced

Job

JobSearch

JobSearchAdvanced

JobType

JobStatus



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/supplyChain.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/supplyChain.xsd) | listScm | 

ManufacturingCostTemplate

ManufacturingOperationTask

ManufacturingRouting



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/website.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/website.xsd) | listSite | 

SiteCategory

SiteCategorySearch

SiteCategorySearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/support.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/support.xsd) | listSupport | 

SupportCase

SupportCaseSearch

SupportCaseSearchAdvanced

SupportCaseStatus

SupportCaseType

SupportCaseOrigin

SupportCaseIssue

SupportCasePriority

Solution

SolutionSearch

SolutionSearchAdvanced

Topic

TopicSearch

TopicSearchAdvanced

Issue

IssueSearch

IssueSearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/setup/v2025\_2\_0/customization.xsd](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customization.xsd) | setupCustom | 

CustomRecord

CustomRecordSearch

CustomRecordSearchAdvanced

CustomList

CustomRecordType

EntityCustomField

CrmCustomField

OtherCustomField

ItemCustomField

TransactionBodyCustomField

TransactionColumnCustomField

ItemOptionCustomField

CustomRecordCustomField

CustomTransaction

CustomSegment



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/bank.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/bank.xsd) | tranBank | 

Check

Deposit



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/customers.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/customers.xsd) | tranCust | 

CashRefund

Charge

CustomerPayment

ReturnAuthorization

CreditMemo

CustomerRefund

CustomerDeposit

DepositApplication



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/inventory.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) | tranInvt | 

InventoryAdjustment

InventoryCostRevaluation

AssemblyBuild

AssemblyUnbuild

WorkOrder

WorkOrderClose

WorkOrderIssue

WorkOrderCompletionOperation



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/employees.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/employees.xsd) | tranEmp | 

TimeBill

TimeBillSearch

TimeBillSearchAdvanced

ExpenseReport

TimeEntry

Timesheet

Paycheck



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/financial.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/financial.xsd) | tranFin | 

Budget

BudgetSearch

BudgetSearchAdvanced



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/general.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/general.xsd) | tranGeneral | 

JournalEntry

InterCompanyJournalEntry

StatisticalJournalEntry

AdvIntercompanyJournalEntry



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/purchases.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/purchases.xsd) | tranPurch | 

VendorBill

PurchaseOrder

ItemReceipt

VendorPayment

VendorCredit

Purchase/Requisition

InboundShipment



 |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/sales.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) | tranSales | 

AccountingTransactionSearch

AccountingTransactionSearchAdvanced

Opportunity

OpportunitySearch

OpportunitySearchAdvanced

SalesOrder

TransactionSearch

TransactionSearchAdvanced

ItemFulfillment

Invoice

CashSale

Estimate



 |

## System Constants XSD Files {#bridgehead_N3417653}

These files provide constant values for the corresponding types in the business records XSD files.

| URL | Schema Alias |
| --- | --- |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/schedulingTypes.xsd](https://webservices.netsuite.com/xsd/activities/v2025_2_0/schedulingTypes.xsd) | actSchedTyp |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/demandPlanning.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/demandPlanning.xsd) | demandPlanningTyp |
| [https://webservices.netsuite.com/xsd/documents/v2025\_2\_0/fileCabinetTypes.xsd](https://webservices.netsuite.com/xsd/documents/v2025_2_0/fileCabinetTypes.xsd) | docFileCabTyp |
| [https://webservices.netsuite.com/xsd/general/v2025\_2\_0/communicationTypes.xsd](https://webservices.netsuite.com/xsd/general/v2025_2_0/communicationTypes.xsd) | generalCommTyp |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/inventoryTypes.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventoryTypes.xsd) | invtTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/accountingTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accountingTypes.xsd) | listAcctTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/employeeTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/employeeTypes.xsd) | listEmpTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/marketingTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/marketingTypes.xsd) | listMktTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/relationshipTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/relationshipTypes.xsd) | listRelTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/supplyChainTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/supplyChainTypes.xsd) | listScmTyp |
| [https://webservices.netsuite.com/xsd/lists/v2025\_2\_0/supportTypes.xsd](https://webservices.netsuite.com/xsd/lists/v2025_2_0/supportTypes.xsd) | listSupportTyp |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/coreTypes.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd) | platformCoreTyp |
| [https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/faultTypes.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/faultTypes.xsd) | platformFaultsTyp |
| [https://webservices.netsuite.com/xsd/setup/v2025\_2\_0/customizationTypes.xsd](https://webservices.netsuite.com/xsd/setup/v2025_2_0/customizationTypes.xsd) | setupCustomTyp |
| [https://webservices.netsuite.com/xsd/transactions/v2025\_2\_0/saleTypes.xsd](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/saleTypes.xsd) | tranSalesTyp |

## Example {#bridgehead_N3418061}

For example, the addRequest message type has three levels of referencing.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                             

In the WSDL file, the **addRequest** message is defined as:

          `<message name="addRequest">    <part name="parameters" element="platformMsgs:add"/> </message>` 
        

The element called **platformMsgs:add** is defined in the platformMsgs XSD file. In this case, the platformMsgs alias refers to the xsd file at:

[https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/messages.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/messages.xsd)

In this file, the addRequest element is defined again as:

          `<complexType name="AddRequest">    <sequence>        <element name="record" type="platformCore:Record" />     </sequence> </complexType>` 
        

Again there is a reference that is not contained in this XSD file called **platformCore:Record**. The platformCore alias refers to the XSD file at:

[https://webservices.netsuite.com/xsd/platform/v2025\_2\_0/core.xsd](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd)

The abstract type Record is defined as:

          `<complexType name="Record" abstract="true">     <sequence>        <element name="nullFieldList" type="platformCore:NullField" minOccurs="0" maxOccurs="1" />     </sequence> </complexType>` 
        

Note:

In SOAP web services, [Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3453509) is the base for all other NetSuite record types.

## XML Samples of Supported Variations of a SOAP Request {#bridgehead_161598870606}

Here you can see 3 variations of a SOAP request that are supported by NetSuite.

## Variation A {#bridgehead_161598883228}

In this variation namespace aliases are always used, as suggested by the official WSDL documentation.

          `<soapenv:Body> <platformMsgs:initialize> <platformMsgs:initializeRecord> <platformCore:type>itemReceipt</platformCore:type> <platformCore:rference type="purchaseOrder" internalId="123"/> </platformMsgs:initializeRecord> </platformMsgs:initialize> </soapenv:Body>` 
        

## Variation B {#bridgehead_161598949069}

In this variation namespace aliases are used only when needed.

          `<soapenv:Body> <platformMsgs:initialize xmlns:platformMsgs="urn:messages_2019_1.platform.webservices.netsuite.com"> <platformMsgs:initializeRecord xmlns:platformCore="urn:core_2019_1.platform.webservices.netsuite.com"> <platformCore:type>itemReceipt</platformCore:type> <platformCore:reference type="purchaseOrder" internalId="123"/> </platformMsgs:initializeRecord> </platformMsgs:initialize> </soapenv:Body>` 
        

## Variation C {#bridgehead_161599081573}

In this variation, the namespace aliases are used again only when necessary.

          `<soapenv:Body> <initialize xmlns="urn:messages_2019_1.platform.webservices.netsuite.com"> <initializeRecord> <urn1:type xmlns:urn1="urn:core_2019_1.platform.webservices.netsuite.com">itemReceipt</urn1:type> <urn2:reference intelId="123" type="purchaseOrder" xmlns:urn2="urn:core_2019_1.platform.webservices.netsuite.com:/> </initializeRecord> </initialize> </soapenv:Body>` 
        

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413869.html)
-   [NetSuite WSDL Versioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418174.html)
-   [SOAP Web Services Performance Optimization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1537861842.html)
-   [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html)
-   [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html)
-   [Glossary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419527.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
