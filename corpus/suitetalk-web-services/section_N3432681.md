---
id: "section_N3432681"
type: "section"
title: "Using Internal IDs, External IDs, and References"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Records in SOAP Web Services > Using Internal IDs, External IDs, and References"
parent: "section_N3428663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432681.html"
anchors: ["bridgehead_3740632950", "bridgehead_3740633421", "bridgehead_N3432744"]
sha256: "fc0dff2d1076d17c1eb6d539d95aecc4e443f93df14b86192388224083956d90"
---

Each record in NetSuite can be uniquely identified by its record type in combination with either an external ID or a system-generated NetSuite internal ID.

Important:

To see the internal IDs for all fields, records, lists, and custom forms, enable the Show Internal IDs preference. See [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html). External IDs are not displayed on records by default. However, you can search for external IDs, or you can add a custom field to the record types where you want to the external ID to be displayed in the UI. For information about searching in SOAP web services, see [Basic Searches in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514760.html). For information about working with custom fields, see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html).

Internal and external IDs are NOT unique across all record types. Therefore, to perform an operation on an existing record, you need two pieces of data: the record type and either the internal ID or the external ID.

References are implemented through the RecordRef type, which is defined in the [core](https://webservices.netsuite.com/xsd/platform/v2025_2_0/core.xsd) XSD.

The RecordRef type is described by three attributes - the internal ID, external ID, and the type:

          `<complexType name="RecordRef"> <complexContent>    <extension base="platformCore:BaseRef">       <attribute name="internalId" type="xsd:string"/>       <attribute name="externalId" type="xsd:string"/>       <attribute name="type" type="platformCoreTyp:RecordType"/>    </extension> </complexType>` 
        

Important:

When referencing records in an update operation, you must provide either the internal ID or the external ID, but not both. If both are provided, the internal ID is used to locate the record and the external ID is ignored. Additionally, the external ID attribute is case insensitive.

## Uniqueness of Internal and External IDs {#bridgehead_3740632950}

Internal and external IDs must be unique not only in a specific record type, but also in certain record groups. These groups consist of multiple record types. For details, see [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html).

Internal IDs are not reused in the system. After an internal ID has been assigned, if the associated record is subsequently deleted, the ID is not reused.

Note also that an external ID exists only if you provided it, either at the time of record creation or during an update. For more on external IDs, see [External IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html).

## Internal IDs Do Not Indicate When Record Was Created {#bridgehead_3740633421}

The assignment of internal IDs to new records is sequential. However, the sequence of internal IDs does not indicate when or in which order records were added. This is true even within specific record groups where internal IDs are unique. Therefore, you should not conclude that records with lower internal IDs were added first, whereas those with higher internal IDs were added last.

Consider the following example. All records belonging to the same high-level group share the same ID pool. For example, sales orders and invoices both belong to the group of transaction records. When you create a sales order and it is assigned 1234 as the internal ID, you should not assume that the internal ID of the next sales order will be 1235. If an invoice or another transaction record is created right after sales order 1234, that record might have 1235 as internal ID. Additionally, there can be gaps between internal IDs. Two sales orders created a few minutes' apart might have a significant gap between their internal IDs.

For custom applications that rely on the chronological aspect of when data was entered, you should use the Date Modified or Date Created fields, as they are guaranteed to be chronological. Additionally, for transactions with auto-generated numbers, the sequence number (for example, 'tranid') is guaranteed to be sequential based on the date transactions were entered. The internal ID of a record should never be used to determine when data was entered, and you should not build any functionality based on the sequence of internal IDs.

## Internal IDs for NetSuite Record Types {#bridgehead_N3432744}

Like individual records, each record _type_ also has an internal ID. In certain situations, you must use this ID to specify which type of record you are referencing. By contrast, in some cases, you can use a string to reference the record type (for example, when using RecordRef). But in other cases you must use the internal ID, or typeId (for example, when using [ListOrRecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3455299) or [CustomRecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3454996)). The table below lists the NetSuite record types and their associated typeIds.

Custom fields of the type [MultiSelectCustomFieldRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html#bridgehead_N3460021) on custom records also reference these values, because they contain an array of [ListOrRecordRef](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3455299) types. For details on working with custom records, see [Custom Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3768988.html).

| Record Type | typeId |
| --- | --- |
| ACCOUNT | \-112 |
| ACCOUNTINGPERIOD | \-105 |
| ADDRESS | \-289 |
| ADVINTERCOMPANYJOURNALENTRY | \-30 |
| APPDEFINITION | \-255 |
| APPPACKAGE | \-254 |
| ASSEMBLYBUILD | \-30 |
| ASSEMBLYITEM | \-10 |
| ASSEMBLYUNBUILD | \-30 |
| BILLINGACCOUNT | \-333 |
| BILLINGSCHEDULE | \-141 |
| BIN | \-242 |
| BINTRANSFER | \-30 |
| BINWORKSHEET | \-30 |
| BOM | \-422 |
| BOMREVISION | \-423 |
| BUDGETCATEGORY | \-396 |
| BUDGETIMPORT | \-420 |
| CALENDAREVENT | \-20 |
| CAMPAIGN | \-24 |
| CAMPAIGNAUDIENCE | \-142 |
| CAMPAIGNCATEGORY | \-143 |
| CAMPAIGNCHANNEL | \-144 |
| CAMPAIGNFAMILY | \-145 |
| CAMPAIGNOFFER | \-146 |
| CAMPAIGNRESPONSE | \-130 |
| CAMPAIGNSEARCHENGINE | \-148 |
| CAMPAIGNSUBSCRIPTION | \-149 |
| CAMPAIGNVERTICAL | \-150 |
| CASHREFUND | \-30 |
| CASHSALE | \-30 |
| CHARGE | \-290 |
| CHECK | \-30 |
| CLASSIFICATION | \-101 |
| CONSOLIDATEDEXCHANGERATE | \-322 |
| CONTACT | \-6 |
| CONTACTCATEGORY | \-158 |
| CONTACTROLE | \-157 |
| COSTCATEGORY | \-155 |
| CREDITMEMO | \-30 |
| CRMCUSTOMFIELD | \-124 |
| CURRENCY | \-122 |
| CUSTOMER | \-2 |
| CUSTOMERCATEGORY | \-109 |
| CUSTOMERDEPOSIT | \-30 |
| CUSTOMERMESSAGE | \-161 |
| CUSTOMERPAYMENT | \-30 |
| CUSTOMERREFUND | \-30 |
| CUSTOMERSTATUS | \-104 |
| CUSTOMLIST | \-123 |
| CUSTOMRECORDCUSTOMFIELD | \-124 |
| CUSTOMRECORDTYPE | \-123 |
| CUSTOMTRANSACTION | \-30 |
| CUSTOMTRANSACTION | \-30 |
| CUSTOMTRANSACTION | \-30 |
| CUSTOMTRANSACTION | \-30 |
| DEPARTMENT | \-102 |
| DEPOSIT | \-30 |
| DEPOSITAPPLICATION | \-30 |
| DESCRIPTIONITEM | \-10 |
| DISCOUNTITEM | \-10 |
| DOWNLOADITEM | \-10 |
| EMPLOYEE | \-4 |
| ENTITYCUSTOMFIELD | \-124 |
| ESTIMATE | \-30 |
| EXPENSECATEGORY | \-126 |
| EXPENSEREPORT | \-30 |
| FAIRVALUEPRICE | \-332 |
| GENERALTOKEN | \-540 |
| GIFTCERTIFICATEITEM | \-10 |
| GLOBALACCOUNTMAPPING | \-250 |
| HCMJOB | \-355 |
| INBOUNDSHIPMENT | \-427 |
| INTERCOMPANYJOURNALENTRY | \-30 |
| INTERCOMPANYTRANSFERORDER | \-30 |
| INVENTORYADJUSTMENT | \-30 |
| INVENTORYCOSTREVALUATION | \-30 |
| INVENTORYDETAIL | \-260 |
| INVENTORYITEM | \-10 |
| INVENTORYNUMBER | \-266 |
| INVENTORYTRANSFER | \-30 |
| INVOICE | \-30 |
| ISSUE | \-26 |
| ITEM | \-10 |
| ITEMACCOUNTMAPPING | \-251 |
| ITEMCUSTOMFIELD | \-124 |
| ITEMDEMANDPLAN | \-246 |
| ITEMFULFILLMENT | \-30 |
| ITEMGROUP | \-10 |
| ITEMNUMBERCUSTOMFIELD | \-124 |
| ITEMOPTIONCUSTOMFIELD | \-124 |
| ITEMRECEIPT | \-30 |
| ITEMREVISION | \-269 |
| ITEMSUPPLYPLAN | \-247 |
| JOB | \-7 |
| JOBTYPE | \-177 |
| JOURNALENTRY | \-30 |
| KITITEM | \-10 |
| LOCATION | \-103 |
| LOTNUMBEREDASSEMBLYITEM | \-10 |
| LOTNUMBEREDINVENTORYITEM | \-10 |
| MANUFACTURINGCOSTTEMPLATE | \-294 |
| MANUFACTURINGOPERATIONTASK | \-36 |
| MANUFACTURINGROUTING | \-288 |
| MARKUPITEM | \-10 |
| NEXUS | \-400 |
| NONINVENTORYPURCHASEITEM | \-10 |
| NONINVENTORYRESALEITEM | \-10 |
| NONINVENTORYSALEITEM | \-10 |
| NOTE | \-303 |
| NOTETYPE | \-180 |
| OPPORTUNITY | \-31 |
| OTHERCHARGEPURCHASEITEM | \-10 |
| OTHERCHARGERESALEITEM | \-10 |
| OTHERCHARGESALEITEM | \-10 |
| OTHERCUSTOMFIELD | \-124 |
| OTHERNAMECATEGORY | \-181 |
| PARTNER | \-5 |
| PARTNERCATEGORY | \-182 |
| PAYCHECK | \-30 |
| PAYCHECKJOURNAL | \-30 |
| PAYMENTCARD | \-538 |
| PAYMENTCARDTOKEN | \-539 |
| PAYMENTITEM | \-10 |
| PAYMENTMETHOD | \-183 |
| PAYROLLITEM | \-265 |
| PHONECALL | \-22 |
| PRICELEVEL | \-186 |
| PRICINGGROUP | \-187 |
| PROJECTTASK | \-27 |
| PROMOTIONCODE | \-121 |
| PURCHASEORDER | \-30 |
| PURCHASEREQUISITION | \-30 |
| RESOURCEALLOCATION | \-28 |
| RETURNAUTHORIZATION | \-30 |
| SALESORDER | \-30 |
| SALESROLE | \-191 |
| SALESTAXITEM | \-128 |
| SERIALIZEDASSEMBLYITEM | \-10 |
| SERIALIZEDINVENTORYITEM | \-10 |
| SERVICEPURCHASEITEM | \-10 |
| SERVICERESALEITEM | \-10 |
| SERVICESALEITEM | \-10 |
| SOLUTION | \-25 |
| STATISTICALJOURNALENTRY | \-30 |
| SUBSIDIARY | \-117 |
| SUBTOTALITEM | \-10 |
| SUPPORTCASE | \-23 |
| SUPPORTCASEISSUE | \-151 |
| SUPPORTCASEORIGIN | \-152 |
| SUPPORTCASEPRIORITY | \-153 |
| SUPPORTCASESTATUS | \-132 |
| SUPPORTCASETYPE | \-154 |
| TASK | \-21 |
| TERM | \-199 |
| TIMEBILL | \-256 |
| TIMEENTRY | \-295 |
| TIMESHEET | \-292 |
| TRANSACTION | \-30 |
| TRANSACTIONBODYCUSTOMFIELD | \-124 |
| TRANSACTIONCOLUMNCUSTOMFIELD | \-124 |
| TRANSFERORDER | \-30 |
| UNITSTYPE | \-201 |
| USAGE | \-362 |
| VENDOR | \-3 |
| VENDORBILL | \-30 |
| VENDORCATEGORY | \-110 |
| VENDORCREDIT | \-30 |
| VENDORPAYMENT | \-30 |
| VENDORRETURNAUTHORIZATION | \-30 |
| WINLOSSREASON | \-203 |
| WORKORDER | \-30 |
| WORKORDERCLOSE | \-30 |
| WORKORDERCOMPLETION | \-30 |
| WORKORDERISSUE | \-30 |

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428928.html)
-   [Search Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3429060.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [External IDs Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3433806.html)
-   [Shared Internal and External IDs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436356.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
