---
id: "section_N3781656"
type: "section"
title: "Coupon Code"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Marketing Records > Coupon Code"
parent: "chapter_N3775421"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3781656.html"
anchors: ["bridgehead_N3781673", "bridgehead_N3781898", "bridgehead_3820241837", "bridgehead_N29040911", "bridgehead_N29040971", "bridgehead_N29041031"]
sha256: "04d66b1a567d9b90f2944cba75d251ee84e61c93b38b98d7743eb9afc3628a23"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Coupon Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_19112846600.html).

Promotions allow you to track the source of revenue and to offer discounts in the form of coupons. Each promotion has a promotion code that can be applied to transactions and campaigns.

The coupon code record is defined in the [listMkt (marketing)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/marketing.xsd) XSD.

For information about working with coupon codes in the UI, see [Coupon Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1519291829.html).

## Supported Operations {#bridgehead_N3781673}

The following operations can be used with coupon code records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3781898}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [coupon code](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/couponcode.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Code Sample {#bridgehead_3820241837}

The following sample shows how to add a coupon code through SOAP web services. Note that to work with coupon codes, you must have a promotion with 'single use' coupon codes (Promotion record > Codes subtab > Number of Uses > Single Use). Then you can start adding coupon codes.

## Java {#bridgehead_N29040911}

          `public void addCouponCode() throws Exception    {       this.login();         CouponCode cc = new CouponCode();       RecordRef promoRef = new RecordRef();       promoRef.setInternalId("3");       cc.setPromotion(promoRef);    // the promotion the coupon code is bound to         cc.setExternalId("exCC12345");       cc.setCode("CouponCode2012");         RecordRef recRef = new RecordRef();       recRef.setInternalId("15");       cc.setRecipient(recRef);       cc.setDateSent(Calendar.getInstance());       _port.add(cc);    }` 
        

## SOAP Request {#bridgehead_N29040971}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <ns1:passport soapenv:mustUnderstand="0" soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">email@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">*******</ns3:password>             <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">1234567</ns4:account>             <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>         </ns1:passport>     </soapenv:Header>     <soapenv:Body>         <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns6:CouponCode" externalId="exCC12345" xmlns:ns6="urn:marketing_2017_1.lists.webservices.netsuite.com">                 <ns6:promotion xsi:type="ns7:RecordRef" internalId="3" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:code xsi:type="xsd:string">CouponCode2012</ns6:code>                 <ns6:recipient xsi:type="ns8:RecordRef" internalId="15" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:dateSent xsi:type="xsd:dateTime">2012-08-10T08:13:27.370Z</ns6:dateSent>             </record>         </add>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N29041031}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1326288_08102012261640432423581449_323eee69f5203</platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                 <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <baseRef xsi:type="platformCore:RecordRef" type="couponCode" externalId="exCC12345" internalId="3" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>         </addResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

### Related Topics

-   [Marketing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3775421.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
