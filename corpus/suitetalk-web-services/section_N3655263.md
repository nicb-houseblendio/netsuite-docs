---
id: "section_N3655263"
type: "section"
title: "Note"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Communications > Note"
parent: "chapter_N3655132"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3655263.html"
anchors: ["bridgehead_N3655283", "bridgehead_N3655524", "bridgehead_N3655562", "bridgehead_N3655574", "bridgehead_N28268141", "bridgehead_N28268201", "bridgehead_N28268261"]
sha256: "3c6a39c52eb9f5087f6ae96f08b5c35495efc55be8173e8b74f4990620184e00"
---

Notes are used to attach information to another record. Use the notes record to create new notes and attach them to a specific record.

The note record is defined in the [generalComm (communication)](https://webservices.netsuite.com/xsd/general/v2025_2_0/communication.xsd) XSD.

## Supported Operations {#bridgehead_N3655283}

The following operations can be used to modify the note record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3655524}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [note](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/note.html) reference page.

Note:

For information on using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3655562}

A note must be associated with one and only one of these records. If values for more than one of these fields is submitted, an error is thrown.

## Sample Code {#bridgehead_N3655574}

The following SOAP and C# samples show how to add a note.

## SOAP Request {#bridgehead_N28268141}

          `<soap:Envelope     xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"     xmlns:xsd="http://www.w3.org/2001/XMLSchema">    <soap:Header>       <preferences xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <warningAsError>false</warningAsError>          <useConditionalDefaultsOnAdd>false</useConditionalDefaultsOnAdd>       </preferences>    </soap:Header>    <soap:Body>       <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <record xsi:type="q1:Note" xmlns:q1="urn:communication_2017_1.general.webservices.netsuite.com">             <q1:title>-- note title goes here --</q1:title>             <q1:noteType internalId="7" type="noteType" />             <q1:direction>_outgoing</q1:direction>             <q1:noteDate>2008-04-09T00:00:00</q1:noteDate>             <q1:note>-- memo goes here --</q1:note>             <q1:activity internalId="39" type="calendarEvent" />             <q1:author internalId="-5" type="employee" />          </record>       </add>    </soap:Body> </soap:Envelope>` 
        

## SOAP Response {#bridgehead_N28268201}

          `<soapenv:Envelope     xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"     xmlns:xsd="http://www.w3.org/2001/XMLSchema"     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">    <soapenv:Header>       <ns1:documentInfo xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com">          <ns1:nsId>WEBSERVICES_721410_040920088803062742117685935_252c2fccbf8a0</ns1:nsId>       </ns1:documentInfo>    </soapenv:Header>    <soapenv:Body>       <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com">          <writeResponse>             <ns2:status isSuccess="true" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com" />             <baseRef internalId="27" type="note" xsi:type="ns3:RecordRef"               xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com" />          </writeResponse>       </addResponse>    </soapenv:Body> </soapenv:Envelope>` 
        

## C# {#bridgehead_N28268261}

          `private void addNotes()         {             this.login(true);               Note note = new Note();               RecordRef activityref = new RecordRef();             activityref.internalId = "39";             activityref.type = RecordType.calendarEvent;             activityref.typeSpecified = true;             note.activity = activityref;                          RecordRef authorref = new RecordRef();             authorref.internalId = "-5";             authorref.type = RecordType.employee;             authorref.typeSpecified = true;             note.author = authorref;               note.direction = NoteDirection._outgoing;             note.directionSpecified = true;               RecordRef notetyperef = new RecordRef();             notetyperef.internalId = "7";             notetyperef.type = RecordType.noteType;             notetyperef.typeSpecified = true;             note.noteType = notetyperef;               DateTime searchDate = new DateTime();             searchDate = DateTime.Now;             searchDate = DateTime.Parse(searchDate.ToString("dd/MM/yyyy"));             note.noteDate = searchDate;             note.noteDateSpecified = true;               note.title = "-- note title goes here --";             note.note = "-- memo goes here --";               WriteResponse writeRes = _service.add(note);             if (writeRes.status.isSuccess)             {                 _out.writeLn("\nThe note " + note.internalId + " has been added successfully");             }             else             {                 _out.error(getStatusDetails(writeRes.status));             }         }` 
        

### Related Topics

-   [Communications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3655132.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
