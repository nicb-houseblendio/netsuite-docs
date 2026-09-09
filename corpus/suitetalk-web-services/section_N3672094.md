---
id: "section_N3672094"
type: "section"
title: "Customer Refund"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Customer Refund"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3672094.html"
anchors: ["bridgehead_N3672131", "bridgehead_N3672400", "bridgehead_N3672432", "bridgehead_3946332984", "bridgehead_N3672441", "bridgehead_N3672482", "bridgehead_N28370651", "bridgehead_N3672504"]
sha256: "77acbd6d529f0b23d4860b0ef4c7e1a51cd6bd389180408e7e73f68b7a72c49d"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Customer Refund](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0830082954.html).

A customer refund transaction records the return of funds to a customer who paid for goods or services using cash, a check, or a credit card. The refund is generally made in cash or by check.

For details about this type of transaction, see [Customer Credits and Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1310987.html).

The customer refund record is defined in the [tranCust (customers)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/customers.xsd) XSD.

## Supported Operations {#bridgehead_N3672131}

The following operations can be used to modify customer refund records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3672400}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [customer refund](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customerrefund.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3672432}

## Working with Credit Card Data {#bridgehead_3946332984}

When working with credit card data, be aware of the following security features:

-   When adding a transaction that uses a credit card number, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## Initializing Customer Refunds {#bridgehead_N3672441}

You can initialize a customer refund from a [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html) or a [Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3666537.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Deposits Saved in CustomerRefundApplyList {#bridgehead_N3672482}

If you add a customer refund with deposits in the CustomerRefundDepositList sublist, note that the deposits are saved in the CustomerRefundApplyList sublist. The following sample SOAP code illustrates this case.

## Customer Refund Add Request {#bridgehead_N28370651}

          `<add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record externalId="Pear16027841" xsi:type="ns8:CustomerRefund" xmlns:ns8="urn:customers_2017_1.transactions.webservices.netsuite.com">                <ns8:customer internalId="3023" xsi:type="ns9:RecordRef" xmlns:ns9="urn:core_2017_1.platform.webservices.netsuite.com">                   <ns9:name xsi:type="xsd:string">Strawberry13167584</ns9:name>                </ns8:customer> truncated portion                <ns8:depositList replaceAll="false" xsi:type="ns8:CustomerRefundDepositList">                   <ns8:customerRefundDeposit xsi:type="ns8:CustomerRefundDeposit">                      <ns8:apply xsi:type="xsd:boolean">true</ns8:apply>                      <ns8:doc xsi:type="xsd:long">4354</ns8:doc>                      <ns8:depositDate xsi:type="xsd:dateTime">2012-07-25T07:00:00.000Z</ns8:depositDate>                      <ns8:refNum xsi:type="xsd:string">26</ns8:refNum>                      <ns8:total xsi:type="xsd:double">40.0</ns8:total>                      <ns8:remaining xsi:type="xsd:double">40.0</ns8:remaining>                   </ns8:customerRefundDeposit>                </ns8:depositList>             </record>          </add>` 
        

## Response to Later Get Request {#bridgehead_N3672504}

          `<getResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <readResponse>                <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                <record internalId="4355" externalId="Pear16027841" xsi:type="tranCust:CustomerRefund" xmlns:tranCust="urn:customers_2017_1.transactions.webservices.netsuite.com">                   <tranCust:customer internalId="3023" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">                      <platformCore:name>Strawberry13167584</platformCore:name>                   </tranCust:customer> truncated portion                   <tranCust:applyList>                      <tranCust:apply>                         <tranCust:apply>true</tranCust:apply>                         <tranCust:doc>4356</tranCust:doc>                         <tranCust:line>1</tranCust:line>                         <tranCust:applyDate>2012-07-25T00:00:00.000-07:00</tranCust:applyDate>                         <tranCust:type>Deposit Application</tranCust:type>                         <tranCust:total>40.0</tranCust:total>                         <tranCust:due>40.0</tranCust:due>                         <tranCust:currency>USA</tranCust:currency>                         <tranCust:amount>40.0</tranCust:amount>                      </tranCust:apply>                   </tranCust:applyList>                </record>             </readResponse>          </getResponse>` 
        

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
