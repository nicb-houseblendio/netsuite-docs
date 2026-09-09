---
id: "section_N3740408"
type: "section"
title: "Accounting Period"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Accounting Period"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3740408.html"
anchors: ["bridgehead_N3740442", "bridgehead_N3740542", "bridgehead_N3740580", "procedure_N3740599", "bridgehead_52094223969", "bridgehead_46094423744", "bridgehead_59094519436", "bridgehead_63094618796"]
sha256: "25a603acfa023a58c9f676213ce343bac651fe4f3b860138e301e9e83908c224"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0818065706.html).

In NetSuite, transactions are posted in real time. If you choose to use accounting periods, you must enter a posting period on the transaction and select its posting period from a dropdown list on the transaction page. The posting period can be future or past, depending on the close status of the period.

To access the accounting periods record in the UI, go to _Setup > Accounting > Manage Accounting Periods_. For information about setting up accounting periods, see [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html) in the NetSuite Help Center.

In SOAP web services, the accounting period record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3740442}

The following operations can be used with the accounting period record.

[get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [searchMoreWithId](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3523074.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3740542}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [accounting period](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/accountingperiod.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3740580}

Important:

This record is available as a read-only record. To make changes to this record, you must do so through the UI.

Also note that to use the accounting periods record, a NetSuite administrator must first enable this feature in your account.

#### To enable Accounting Periods: {#procedure_N3740599}

1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
    
2.  Click the **Accounting** subtab.
    
3.  Check the **Accounting Periods** box.
    
4.  Click **Save**.
    

The parent field of the AccountingPeriod record is available only if the Multiple Calendars feature is disabled. If the Multiple Calendars feature is enabled, you should use the parent field of the AccountingPeriodFiscalCalendars record instead.

## Sample Code {#bridgehead_52094223969}

The following sample illustrates what your SOAP web services requests and responses should look like.

## Sample SOAP Web Services Request {#bridgehead_46094423744}

          `</soap:Header>   <soap:Body>     <platformMsgs:get>       <platformMsgs:baseRef xsi:type="platformCore:RecordRef" internalId="3" type="accountingPeriod" />     </platformMsgs:get>   </soap:Body> </soap:Envelope>` 
        

## Sample SOAP Web Services Response with the Multiple Calendars feature Disabled {#bridgehead_59094519436}

          `<soapenv:Body>     <getResponse xmlns="urn:messages_2022_2.platform.webservices.netsuite.com">       <readResponse>         <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2022_2.platform.webservices.netsuite.com"/>           <record internalId="3" xsi:type="listAcct:AccountingPeriod" xmlns:listAcct="urn:accounting_2022_2.lists.webservices.netsuite.com">             <listAcct:periodName>Jan 2014</listAcct:periodName>             <listAcct:parent internalId="2" xmlns:platformCore="urn:core_2022_2.platform.webservices.netsuite.com">               <platformCore:name>Q1 2014</platformCore:name>             </listAcct:parent>             ...           </record>         </readResponse>       </getResponse>     </soapenv:Body>` 
        

## Sample SOAP Web Services Response with the Multiple Calendars feature Enabled {#bridgehead_63094618796}

          `<soapenv:Body>     <getResponse xmlns="urn:messages_2022_2.platform.webservices.netsuite.com">       <readResponse>         <platformCore:status isSuccess="true" xmlns:platformCore="urn:core_2022_2.platform.webservices.netsuite.com"/>           <record internalId="3" xsi:type="listAcct:AccountingPeriod" xmlns:listAcct="urn:accounting_2022_2.lists.webservices.netsuite.com">             <listAcct:periodName>Jan 2014</listAcct:periodName>             ...             <listAcct:fiscalCalendarsList>               <listAcct:accountingPeriodFiscalCalendars>                 <listAcct:fiscalCalendar internalId="1" xmlns:platformCore="urn:core_2022_2.platform.webservices.netsuite.com">                   <platformCore:name>Standard Fiscal Calendar</platformCore:name>                 </listAcct:fiscalCalendar>                 <listAcct:parent internalId="2" xmlns:platformCore="urn:core_2022_2.platform.webservices.netsuite.com">                   <platformCore:name>Q1 2014</platformCore:name>                 </listAcct:parent>               </listAcct:accountingPeriodFiscalCalendars>             </listAcct:fiscalCalendarsList>             ...           </record>         </readResponse>       </getResponse>` 
        

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
