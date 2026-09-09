---
id: "section_N3744289"
type: "section"
title: "Gift Certificate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Gift Certificate"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744289.html"
anchors: ["bridgehead_N3744322", "bridgehead_N3744564", "bridgehead_3820215343", "bridgehead_N28829041", "bridgehead_N28828921", "bridgehead_N28828981"]
sha256: "2f655e2a2ba8a0386eb38f45496b11aeb85e9661f6b69d1dc0ddbffb1076b2f3"
---

A gift certificate record is created when a customer purchases a gift certificate item. For example, you might create a gift certificate item and make it available for purchase. A customer can then buy this gift certificate item. When the customer buys the gift certificate item and names a recipient, the system creates a gift certificate, which can be redeemed for goods and services sold by your business. The gift certificate includes properties such as an expiration date, a remaining value, and the email address of the gift certificate's recipient.

The gift certificate record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD, where it is called giftCertificate.

To view existing gift certificate instances in the UI, go to _Lists > Accounting > Gift Certificates_.

For details about working with gift certificate items in the UI, see [Viewing and Editing Gift Certificate Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2246379.html). For full details about the gift certificate feature, see [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html).

The gift certificate item record is also supported in SOAP web services. For details, see [Gift Certificate Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3717097.html).

## Supported Operations {#bridgehead_N3744322}

The following operations can be used with the gift certificate record:

[get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

Note that when using the **update** operation, only the following fields can be updated:

-   email
    
-   expirationDate
    
-   message
    
-   name
    
-   sender
    

## Gift Certificate Field Definitions {#bridgehead_N3744564}

This record does not support external ID.

For full details on all body fields, sublist fields, search filters, and search joins available to this record, see the SOAP Schema Browser's [gift certificate reference page](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/giftcertificate.html).

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#bridgehead_3820215343}

The following example show how to update a gift certificate instance's with new values for the recipient, name, message, and expirationDate fields.

## C# {#bridgehead_N28829041}

          `private void updateGiftCertificate() {    GiftCertificate myGiftCertificate = new GiftCertificate();    myGiftCertificate.internalId = "13";    myGiftCertificate.email = "john@smith.com";    myGiftCertificate.name = "John";    myGiftCertificate.message = "Happy Birthday!";               DateTime nextYear = new DateTime(2016, 1, 1);    myGiftCertificate.expirationDate = nextYear;    myGiftCertificate.expirationDateSpecified = true;             _service.update(myGiftCertificate);  }` 
        

## SOAP Request {#bridgehead_N28828921}

          `<soap:Body>    <update xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <record internalId="13" xsi:type="q1:GiftCertificate" xmlns:q1="urn:accounting_2017_1.lists.webservices.netsuite.com">          <q1:name>John</q1:name>          <q1:email>john@smith.com</q1:email>          <q1:message>Happy Birthday!</q1:message>          <q1:expirationDate>2016-01-01T00:00:00</q1:expirationDate>       </record>    </update> </soap:Body>` 
        

## SOAP Response: {#bridgehead_N28828981}

          `<soapenv:Body>    <updateResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">       <writeResponse>          <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>          <baseRef xsi:type="platformCore:RecordRef" type="giftCertificate" internalId="13" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>       </writeResponse>    </updateResponse> </soapenv:Body>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
