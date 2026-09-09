---
id: "section_N3655720"
type: "section"
title: "Message"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Communications > Message"
parent: "chapter_N3655132"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3655720.html"
anchors: ["bridgehead_N3655763", "bridgehead_N3656000", "bridgehead_N3656037", "bridgehead_4771613580", "bridgehead_4771614213", "bridgehead_4771613898", "bridgehead_4785520390", "bridgehead_N3656070", "bridgehead_N3656099", "bridgehead_N3656145", "bridgehead_N3657590", "bridgehead_N28272391", "bridgehead_N28272451", "bridgehead_N3657623"]
sha256: "791a6d32644536cd3c428ed6a5bdb6f990fd9057e92ac015013b1c79e692787a"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Message](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161038358813.html).

A message is used to record correspondence you have with a specific business. Use the message record to add an email message to an existing customer, contact, or opportunity record. After an email message has been added to a record, any related emails are automatically attached to the same record as well as to any recipients of the original email.

The message record is defined in the [generalComm (communication)](https://webservices.netsuite.com/xsd/general/v2025_2_0/communication.xsd) XSD.

For information about adding an email message to a record in the NetSuite user interface, see [Sending Email from Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512629.html).

Note:

Adding letters, PDFs, or faxes through SOAP web services is not supported.

## Supported Operations {#bridgehead_N3655763}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) |

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3656000}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [message](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/message.html) reference page.

Note:

For information on using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3656037}

## Message RecordRef Fields {#bridgehead_4771613580}

Message recordref fields cannot be referred to by externalId.

## Email Fields May Be Required {#bridgehead_4771614213}

The following Email fields are required if the From or Attach to entity records do not have an email address specified. If you attempt to create a message without both of these fields specified, the request fails with a message about missing mandatory fields.

| **Field** | **Label in UI** | **Description** |
| --- | --- | --- |
| `authorEmail` | (From) Email Address | A string that includes the email address of the person writing the email. This email address is displayed as the From address in the email message that is sent to the recipient. |
| `recipientEmail` | (To) Email Address | A string that includes the email address of the person receiving the email. This email address is the address to which the email message is sent.. |

## Using the BCC and CC Fields on the Message Record {#bridgehead_4771613898}

The bcc and cc fields represent the list of secondary email addresses associated with the message. These are string fields that accept a space deliminated list of email addresses. For endpoints prior to 2009.2, invalid email addresses in the bcc and cc fields do not result in errors. For the 2009.2 and later endpoints, invalid email addresses in the bcc and cc fields return Invalid Field Value errors.

## Using the dateTime Field on the Message Record {#bridgehead_4785520390}

The dateTime field is only included in 2009.2 and earlier endpoints. It contains the same value as the messageDate field, but in a different date format. If you use an endpoint later than 2009.2, use messageDate rather than the obsolete dateTime field.

## Working with Attachments {#bridgehead_N3656070}

You cannot update an attachment in the context of a message, but you can do so through an update operation on the file record. File records represent files that are stored in the NetSuite File Cabinet. Use the file record to define email attachments sent or received via the messages record. For additional usage notes on working with the file record, see [File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3784054.html).

The file record is defined in the [docFileCab (fileCabinet)](https://webservices.netsuite.com/xsd/documents/v2025_2_0/fileCabinet.xsd) XSD.

## Encoding {#bridgehead_N3656099}

The schema has a data type of xsd:base64Binary which is mapped to a byte array in .NET and Axis (Java). On the client side we only need to pass a text or binary file as a byte array with no further base64 encoding. Therefore, do NOT Base64 Encode the file before sending it to Axis or .NET as these layers will do so themselves.

**For example:**

-   Correct
    
                  `--------    fis = new FileInputStream(inFile);    b = new byte[(int)inFile.length()];    fis.read(b);    myMediaItem.setContent(b);    --------` 
                
    
-   Incorrect
    
                  `---------    fis = new FileInputStream(inFile);    b = new byte[(int)inFile.length()];    fis.read(b);    myMediaItem.setContent(new String(Base64.encode(b)));` 
                
    

## Storing Attachments {#bridgehead_N3656145}

To maintain uniqueness for each file attachment, when attachments are stored in NetSuite two levels of sub-folders are automatically created for the Attachments Sent and Attachments Received respectively.

If the incoming field of the message record is set to **false**, the attachment is saved in the Attachments Sent folder. If the incoming filed is set to **true**, the attachment is saved in the Attachments Received folder.

The folder structure being generated is as follows:

-   File Cabinet
    
-   Attachments Sent or Attachments Received
    
-   Entity Name
    
-   Date & Time / Msg ID
    
-   File name
    

**For example:**

A user is using auto email reply capture feature. They send a message to their contact John Smith from within the application. When the contact replies to the message they also attach a file to the message. When the message is created in NetSuite (through the auto reply capture feature) it is saved to a sub-folder that is created when the attachment is saved. The path to the sub-folder is as follows:

file cabinet > attachments received > Attachments Received > John Smith > 20050620\_Message\_525 > File.doc.

Note:

If an attachment is being stored with an extension that does not match the actual file type (for example a .txt file as a .exe file), the file is listed in NetSuite as other text or other binary but this is a label - there is no logical effect on the file.

## Adding Messages {#bridgehead_N3657590}

The following is a basic sample that shows how to add a message record.

## SOAP Request {#bridgehead_N28272391}

          `<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> <soap:Header> <preferences xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <warningAsError>false</warningAsError> <useConditionalDefaultsOnAdd>false</useConditionalDefaultsOnAdd> </preferences> </soap:Header> <soap:Body> <add xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <record xsi:type="q1:Message" xmlns:q1="urn:communication_2017_1.general.webservices.netsuite.com"> <q1:author internalId="-5" type="employee" /> <q1:recipient internalId="-5" type="employee" /> <q1:messageDate>2008-04-09T00:00:00</q1:messageDate> <q1:subject>-- subject goes here --</q1:subject> <q1:message>This is a sample message</q1:message> <q1:activity internalId="39" type="calendarEvent" /> </record> </add> </soap:Body> </soap:Envelope>` 
        

## SOAP Response {#bridgehead_N28272451}

          `<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"> <soapenv:Header> <ns1:documentInfo xmlns:ns1="urn:messages_2017_1.platform.webservices.netsuite.com"> <ns1:nsId>WEBSERVICES_721410_040920088711404551689975949_f1a83e87c1bf0</ns1:nsId> </ns1:documentInfo> </soapenv:Header> <soapenv:Body> <addResponse xmlns="urn:messages_2017_1.platform.webservices.netsuite.com"> <writeResponse> <ns2:status isSuccess="true" xmlns:ns2="urn:core_2017_1.platform.webservices.netsuite.com" /> <baseRef internalId="46" type="message" xsi:type="ns3:RecordRef" xmlns:ns3="urn:core_2017_1.platform.webservices.netsuite.com" /> </writeResponse> </addResponse> </soapenv:Body> </soapenv:Envelope>` 
        

## C# {#bridgehead_N3657623}

          `private void addMessage() { this.login(true);  Message msg = new Message();  RecordRef activityref = new RecordRef(); activityref.internalId = "39"; activityref.type = RecordType.calendarEvent; activityref.typeSpecified = true; msg.activity = activityref;  RecordRef authorref = new RecordRef(); authorref.internalId = "-5"; authorref.type = RecordType.employee; authorref.typeSpecified = true; msg.author = authorref;  RecordRef recipientref = new RecordRef(); recipientref.internalId = "-5"; recipientref.type = RecordType.employee; recipientref.typeSpecified = true; msg.recipient = recipientref;  DateTime searchDate = new DateTime(); searchDate = DateTime.Now; searchDate = DateTime.Parse(searchDate.ToString("dd/MM/yyyy")); msg.messageDate = searchDate; msg.messageDateSpecified = true;  msg.subject = "-- subject goes here --"; msg.message = "This is a sample message"; msg.incoming = true;  WriteResponse writeRes = _service.add(msg); if (writeRes.status.isSuccess) { _out.writeLn("\nThe message " + msg.internalId + " has been added successfully"); } else { _out.error(getStatusDetails(writeRes.status)); } }` 
        

### Related Topics

-   [Communications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3655132.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
