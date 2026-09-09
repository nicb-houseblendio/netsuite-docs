---
id: "section_N3672681"
type: "section"
title: "Deposit Application"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Deposit Application"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3672681.html"
anchors: ["bridgehead_N3672718", "bridgehead_N3672968", "bridgehead_N3673005", "bridgehead_N3673013", "bridgehead_4770778682", "bridgehead_4770781362", "bridgehead_4770781779", "bridgehead_4785550584"]
sha256: "ef50807c3674836eed3f1f82dfc7b3e6b2d8d400d7b04848e79a200d55815117"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Deposit Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0830101547.html).

A deposit application transaction applies a customer deposit against an invoice after the order is complete.

For details about this type of transaction, see [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html).

The deposit application record is defined in [tranCust (customers)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/customers.xsd) XSD.

## Supported Operations {#bridgehead_N3672718}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3672968}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [deposit application](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/depositapplication.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3673005}

## Initializing Deposit Applications {#bridgehead_N3673013}

You can initialize a Deposit Application from a [Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3667158.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Initializing Deposit Applications from Customer Deposits {#bridgehead_4770778682}

For NetSuite accounts with multiple A/R accounts, the InitializeAuxRefType arAccount parameter can be used to specify an A/R account a deposit application record is initialized from a customer deposit record. The returned record contains lines that correspond to the specified A/R account.

The arAccount parameter is defined in InitializeAuxRefType in the [coreTypes](https://webservices.netsuite.com/xsd/platform/v2025_2_0/coreTypes.xsd) XSD.

For information about working with the customer deposit record in the UI, see [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html). For information about working with customer deposit records in SOAP web services, see [Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3667158.html).

The following example shows the initialization of a deposit application from a customer deposit:

## Java {#bridgehead_4770781362}

          `DepositApplication da = (DepositApplication)c.initialize(new InitializeRef(null, InitializeRefType.customerDeposit, '1506', null), InitializeType.depositApplication, new InitializeAuxRef(null, InitializeAuxRefType.arAccount, '9', null));  System.out.println(da.getArAcct());  da.getApplyList().getApply(0).setApply(true);  c.addRecord(da);` 
        

## SOAP Request {#bridgehead_4770781779}

          `<soapenv:Body>         <initialize xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <initializeRecord>                 <ns9:type xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">depositApplication</ns9:type>                 <ns10:reference type="customerDeposit" internalId="1506" xmlns:ns10="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns11:auxReference type="arAccount" internalId="9" xmlns:ns11="urn:core_2017_1.platform.webservices.netsuite.com"/>             </initializeRecord>         </initialize>     </soapenv:Body>` 
        

## SOAP Response {#bridgehead_4785550584}

          `<soapenv:Body>         <initializeResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <readResponse>                 <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <record xsi:type="tranCust:DepositApplication" xmlns:tranCust="urn:customers_2017_1.transactions.webservices.netsuite.com">                     <tranCust:createdDate>2016-11-07T09:35:00.000-08:00</tranCust:createdDate>                     <tranCust:lastModifiedDate>2016-11-07T09:35:00.000-08:00</tranCust:lastModifiedDate>                     <tranCust:arAcct internalId="9" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                         <platformCore:name>11200 Delinquent Accounts</platformCore:name>                     </tranCust:arAcct>                     <tranCust:status>Not Deposited</tranCust:status>                     <tranCust:customer internalId="87" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                         <platformCore:name>Abe Simpson</platformCore:name>                     </tranCust:customer>                     <tranCust:tranDate>2016-11-07T00:00:00.000-08:00</tranCust:tranDate>                     <tranCust:postingPeriod internalId="288" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                         <platformCore:name>Nov 2016</platformCore:name>                     </tranCust:postingPeriod>                     <tranCust:deposit internalId="1506" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                         <platformCore:name>Customer Deposit #1</platformCore:name>                     </tranCust:deposit>                     <tranCust:total>222.0</tranCust:total>                     <tranCust:applied>0.0</tranCust:applied>                     <tranCust:unapplied>222.0</tranCust:unapplied>                     <tranCust:tranId>To Be Generated</tranCust:tranId>                 </record>             </readResponse>         </initializeResponse>     </soapenv:Body>` 
        

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
