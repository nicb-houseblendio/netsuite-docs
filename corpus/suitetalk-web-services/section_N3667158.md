---
id: "section_N3667158"
type: "section"
title: "Customer Deposit"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Customer Deposit"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3667158.html"
anchors: ["bridgehead_N3667195", "bridgehead_N3667461", "bridgehead_N3667498", "bridgehead_3946333175", "bridgehead_N3667506", "bridgehead_N3667522", "bridgehead_N3667534"]
sha256: "7bd6226e9dc7a0a694fe5fafbc86c227b706b2b7e69dd9a58ae7c0b6fccf6cb4"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0830072110.html).

A customer deposit transaction records the funds received when a customer makes an advance payment for an order. This payment is recorded in the general ledger as a liability until the goods or services are delivered, and does not affect the customer's accounts receivable balance. After the order is filled, the deposit is applied against the invoice.

For more details about this type of transaction, see [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html).

The customer deposit record is defined in the [tranCust (customers)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/customers.xsd) XSD.

## Supported Operations {#bridgehead_N3667195}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3667461}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [customer deposit](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customerdeposit.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3667498}

## Working with Credit Card Data {#bridgehead_3946333175}

When working with credit card data, be aware of the following security features:

-   When adding a transaction that uses a credit card number, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## Creating a Customer Deposit based on a Sales Order {#bridgehead_N3667506}

As of the 2012.1 endpoint, the salesOrder field is exposed for customer deposit transactions, so that customer deposits can be based on other types of sales orders in addition to cash sales, typically from invoices. Note that only sales orders with the same customer as in the customer deposit can be used.

The following example shows the creation of a customer deposit based on a sales order:

## HTTP Request {#bridgehead_N3667522}

          `<platformMsgs:add           xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/"           xmlns:xs="http://www.w3.org/2001/XMLSchema"           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"           xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com"           xmlns:s0="urn:customers_2017_1.transactions.webservices.netsuite.com"           xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">          <platformMsgs:record xsi:type="s0:CustomerDeposit">             <s0:customer internalId="199" />             <s0:salesOrder internalId="7818" />             <s0:payment>214.0</s0:payment>          </platformMsgs:record>       </platformMsgs:add>` 
        

## HTTP Response {#bridgehead_N3667534}

          `<addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <writeResponse>             <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com" />             <baseRef internalId="7828" type="customerDeposit" xsi:type="platformCore:RecordRef"               xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com" />          </writeResponse>       </addResponse>` 
        

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
