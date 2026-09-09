---
id: "section_N3741914"
type: "section"
title: "Currency Rate"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Currency Rate"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3741914.html"
anchors: ["bridgehead_N3742027", "bridgehead_N3742168", "bridgehead_N3742212", "bridgehead_3820213802", "bridgehead_N28821561", "bridgehead_N28821441", "bridgehead_N28821501"]
sha256: "0e21eacc67af17936510d443facae59c84ec2246e29f4334cdce8f6f84748fd3"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Currency Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0715014257.html).

The currency rate record is defined in the [listAcct (accounting) XSD](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd).

The currency rate record is the same record that appears as the **Exchange Rate** record in the UI. In the UI, access this record by going to _Lists > Accounting > Currency Exchange Rates > New_.

Note:

The Multiple Currencies feature must be enabled in your account before using this record. For information about enabling this feature, see [Enabling the Multiple Currencies Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395677.html).

In SOAP web services, you can add new currency rate records, but you cannot update them. That is, after added the record, you cannot use any of the update operations to update the record. Update operations include update, updateList, upsert, and upsertList.

After adding a currency rate record, your data will appear in the Currency Exchange Rates table.

In SOAP web services you must use the getCurrencyRate operation to get the exchange rate between two currencies based on a certain date. (See [getCurrencyRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3492280.html) for more information about using this operation.)

Note that in both the UI and in SOAP web services, the Exchange Rate (exchangeRate) field is a create-time-only field that is used to specify the initial exchange rate with respect to the base currency. After the initial exchange rate value is set, this value does not get updated to reflect real-time exchange rates. Therefore, if you were to attempt to get today's current exchange rate, the value returned could be inaccurate.

Note:

The Previous Effective Date and the Previous Exchange Rate fields are not currently available in SOAP web services.

## Supported Operations {#bridgehead_N3742027}

The following operations can be used with the currency rate record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getCurrencyRate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3492280.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3742168}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [currency](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/currency.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3742212}

The follow sample shows how to add a currency rate record through SOAP web services.

## Code Sample {#bridgehead_3820213802}

## Java {#bridgehead_N28821561}

          `// USD -> GBP, from tomorrow, with rate 1.4488    public void addCurrencyRate() throws Exception    {       this.login();         RecordRef usd = new RecordRef();       usd.setInternalId("1");       usd.setType(RecordType.currency);         RecordRef gbp = new RecordRef();       gbp.setInternalId("2");       gbp.setType(RecordType.currency);         com.netsuite.devtools.lists.accounting.CurrencyRate crs = new com.netsuite.devtools.lists.accounting.CurrencyRate();       crs.setBaseCurrency(usd);       crs.setTransactionCurrency(gbp);       crs.setExchangeRate(1.4488D);         Calendar cal = Calendar.getInstance();       cal.add(Calendar.DAY_OF_YEAR, +1);   //tomorrow       crs.setEffectiveDate(cal);         _port.add(crs);    }` 
        

## SOAP Request {#bridgehead_N28821441}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <ns1:passport soapenv:mustUnderstand="0" soapenv:actor="http://schemas.xmlsoap.org/soap/actor/next" xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">             <ns2:email xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com">email@netsuite.com</ns2:email>             <ns3:password xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com">*******</ns3:password>             <ns4:account xmlns:ns4="urn:core_2017_1.platform.webservices.netsuite.com">1234567</ns4:account>             <ns5:role internalId="37" xmlns:ns5="urn:core_2017_1.platform.webservices.netsuite.com"/>         </ns1:passport>     </soapenv:Header>     <soapenv:Body>         <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <record xsi:type="ns6:CurrencyRate" xmlns:ns6="urn:accounting_2017_1.lists.webservices.netsuite.com">                 <ns6:baseCurrency xsi:type="ns7:RecordRef" type="currency" internalId="1" xmlns:ns7="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:transactionCurrency xsi:type="ns8:RecordRef" type="currency" internalId="2" xmlns:ns8="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <ns6:exchangeRate xsi:type="xsd:double">1.4488</ns6:exchangeRate>                 <ns6:effectiveDate xsi:type="xsd:dateTime">2012-08-11T06:50:09.038Z</ns6:effectiveDate>             </record>         </add>     </soapenv:Body> </soapenv:Envelope>` 
        

## SOAP Response {#bridgehead_N28821501}

          `<soapenv:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">     <soapenv:Header>         <platformMsgs:documentInfo xmlns:platformMsgs="urn:messages_2017_1.platform.webservices.netsuite.com">             <platformMsgs:nsId>WEBSERVICES_1326288_080920122566427461899365710_9bfa26bd40b8</platformMsgs:nsId>         </platformMsgs:documentInfo>     </soapenv:Header>     <soapenv:Body>         <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">             <writeResponse>                 <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>                 <baseRef xsi:type="platformCore:RecordRef" type="currencyRate" internalId="58" xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com"/>             </writeResponse>         </addResponse>     </soapenv:Body> </soapenv:Envelope>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
