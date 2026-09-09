---
id: "section_N3667711"
type: "section"
title: "Customer Payment"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Customer Payment"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3667711.html"
anchors: ["bridgehead_N3667752", "bridgehead_N3668021", "bridgehead_N3668058", "bridgehead_3946317766", "bridgehead_N3668067", "bridgehead_N3668107", "bridgehead_N3668159"]
sha256: "f3094a32997f1b312be213b0be303ebf88809d8c90e6a88a6a60e1a8ca483cc3"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Customer Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0224093711.html).

A customer payment transaction records a customer payment and applies it to the appropriate invoice or cash sale, decreasing the amount due and tracking income.

For details about this type of transaction, see [Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html).

The customer payment record is defined in the [tranCust (customers)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/customers.xsd) XSD.

## Supported Operations {#bridgehead_N3667752}

The following operations can be used with customer payment records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3668021}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [customer payment](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customerpayment.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3668058}

## Working with Credit Card Data {#bridgehead_3946317766}

When working with credit card data, be aware of the following security features:

-   When adding a transaction that uses a credit card number, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## Initializing Customer Payments {#bridgehead_N3668067}

You can initialize a customer payment from a [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html) or an [Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3678746.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Working with AutoApply {#bridgehead_N3668107}

If you specify the 'total amount of the original payment' as the payment value in a customer payment, autoApply through SOAP web services fails when there has already been an amount applied previously on the payment. This process fails when autoApply is set to true, and an invoice with apply = true already exists in the customer payment.

To work around this, you must set apply=false for the invoice. The following is the preferred workflow:

GET: (get the existing customer payment)

          `<get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <baseRef internalId="2262" type="customerPayment" xsi:type="ns1:RecordRef" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/> </get>` 
        

RESPONSE: (the response will return all the invoices that were already applied)

          `<ns3:applyList> <ns3:apply> <ns3:apply>true</ns3:apply> <ns3:doc>1929</ns3:doc> <ns3:total>27.92</ns3:total> <ns3:due>27.92</ns3:due> <ns3:amount>27.92</ns3:amount> </ns3:apply> <ns3:apply> <ns3:apply>true</ns3:apply> <ns3:doc>1930</ns3:doc> <ns3:total>27.92</ns3:total> <ns3:due>27.92</ns3:due> <ns3:amount>27.92</ns3:amount> </ns3:apply> </ns3:applyList>` 
        

UPDATE: (update the customer payment - set paymentAmount to the original amount, set autoApply = true, \*\*AND\*\* set apply = false on all the invoices that have been already applied)

          `<update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record internalId="2262" xsi:type="ns1:CustomerPayment" xmlns:ns1="urn:customers_2017_1.transactions.webservices.netsuite.com"> <ns1:customer internalId="176" xsi:type="ns2:RecordRef" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com"/> <ns1:payment xsi:type="xsd:double">80.0</ns1:payment> <ns1:autoApply xsi:type="xsd:boolean">true</ns1:autoApply> <ns1:applyList replaceAll="false" xsi:type="ns1:CustomerPaymentApplyList"> <ns1:apply xsi:type="ns1:CustomerPaymentApply"> <ns1:apply xsi:type="xsd:boolean">false</ns1:apply> <ns1:doc xsi:type="xsd:long">1929</ns1:doc> </ns1:apply> <ns1:apply xsi:type="ns1:CustomerPaymentApply"> <ns1:apply xsi:type="xsd:boolean">false</ns1:apply> <ns1:doc xsi:type="xsd:long">1930</ns1:doc> </ns1:apply> </ns1:applyList> </record> </update>` 
        

GET: (perform a get to verify that it worked)

          `<get xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <baseRef internalId="2262" type="customerPayment" xsi:type="ns1:RecordRef" xmlns:ns1="urn:core_2017_1.platform.webservices.netsuite.com"/> </get>` 
        

RESPONSE: (this response shows that the update worked. The invoices that were applied before are still applied, and the rest of the Payment Amount was applied to new invoices)

          `<ns3:applyList> <ns3:apply> <ns3:apply>true</ns3:apply> <ns3:doc>1933</ns3:doc> <ns3:total>27.92</ns3:total> <ns3:due>27.92</ns3:due> <ns3:amount>24.16</ns3:amount> </ns3:apply> <ns3:apply> <ns3:apply>true</ns3:apply> <ns3:doc>1929</ns3:doc> <ns3:total>27.92</ns3:total> <ns3:due>27.92</ns3:due> <ns3:amount>27.92</ns3:amount> </ns3:apply> <ns3:apply> <ns3:apply>true</ns3:apply> <ns3:doc>1930</ns3:doc> <ns3:total>27.92</ns3:total> &lt...` 
        

## Setting Accounts on Customer Payments {#bridgehead_N3668159}

The 2013.1 endpoint changed the precedence for setting the account on customer payments from earlier endpoints. For the 2013.1 and later endpoints, if Undep. Funds is set to True, this value overrides Payment Method, and if Undep. Funds is set to False, Account overrides Payment Method.

In the 2012.2 and earlier endpoints, the account for a customer payment can only be set to Undep. Funds if the Payment Method and Account fields do not have values set, and there are also further complexities. Review the following table for details about setting the account on a customer payment in these earlier endpoints:

| Payment Method Group with Undep. Funds or Deposit to Account? | Is Payment Method Field Value Set? | What Is Undep. Funds Field Value? | Is Account Field Value Set? | What is Result? |
| --- | --- | --- | --- | --- |
| Deposit to Account | Yes | False | Yes | account = value set for Account Field |
| Deposit to Account | Yes | True | No | account = account associated with selected payment meethod |
| Group with Undep. Funds | No | False | Yes | FAIL |
| Group with Undep. Funds | No | True | No | account = Undeposited Funds account |
| Group with Undep. Funds | No | True | Yes | FAIL |
| Deposit to Account | Yes | True | Yes | account = value set for Account Field |

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
