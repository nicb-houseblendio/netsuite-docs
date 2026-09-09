---
id: "section_N3191112"
type: "section"
title: "Message"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Communications > Message"
parent: "chapter_N3191061"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3191112.html"
anchors: ["bridgehead_4878697072", "bridgehead_1491851010", "bridgehead_N3191154", "bridgehead_4878703668"]
sha256: "b6e43235d26cc889c671e119b5836496c06db3d7f5310151703e02085235faba"
---

A message is used to record correspondence you have with a specific business. Use the message record to add an email message to an existing customer, contact, or opportunity record. After an email message has been added to a record, any related emails are automatically attached to the same record and to any recipients of the original email.

To work with the message record, sublist of recipients, and to send email, use the [N/email Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4358552361.html).

For help working with this record in the user interface, see [Sending Email from Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512629.html).

The internal ID for this record is `message`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/message.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_4878697072}

The message record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1491851010}

For information about sending email from a record, see [Sending Email from Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512629.html). Note that there are also other types of messages, but those are not supported. In the message that you are creating, you can set all supported fields for email messages before saving. After you save the new message, there are restrictions applied to it. You cannot edit the existing message. It is possible to delete an existing message, if the permissions for the user are set to allow this type of operation. However, you should not delete an existing message because it can cause email communication threads to be displayed incorrectly.

## Usage Notes {#bridgehead_N3191154}

-   Message records can be edited only during the create operation. After they are created and submitted, existing message records cannot be edited.
    
-   Existing message records can be copied and deleted.
    
-   Only beforeLoad and afterSubmit user event scripts will execute on the Message record type when a message is created by an inbound email case capture. Scripts set to execute on a beforeSubmit event will not execute.
    
    For example, if you have a test script like the following deployed to the Message record type:
    
                  `function beforeLoad(type, name) {      log.debug ({         title: 'Before Load',         details: 'In beforeLoad function'     }); }  function beforeSubmit(type, name) {      log.debug ({         title: 'Before Submit',         details: 'In beforeSubmit function'       }); }  function afterSubmit(type, name) {      log.debug ({         title: 'After Submit',         details: 'In afterSubmit function'       }); }` 
                
    
    only the beforeLoad(...) and afterSubmit(...) functions will execute if the message was created to respond to an inbound emailed case.
    
-   When creating a new message, you can use the otherrecipientslist sublist to add an email address to the cc or bcc fields. For an example, see [Code Sample](#bridgehead_4878703668).
    
-   An entity that is defined as the author or recipient for a newly created message must have an associated email in NetSuite. If the NetSuite record for an entity defined as the author of a message does not include an email, the `authoremail` field must be defined on the message record. If the NetSuite record for an entity defined as the recipient of a message does not include an email, the `recipientemail` field must be defined on the message record.
    

## Code Sample {#bridgehead_4878703668}

The following SuiteScript 2.x snippet shows how to add an email address to the cc line of a new message, when working in standard (deferredDynamic) mode.

Note:

Some of the values in this sample are placeholders. Before using this sample, replace all hard-coded values, such as IDs and file paths, with valid values from your NetSuite account. If you run a script with an invalid value, the system may throw an error.

          `/**  * @NApiVersion 2.x  */  require(['N/record'], function(record) {       function makeMessage(){          var messageRec = record.create ({             type: record.Type.MESSAGE,             isDynamic: true       });        messageRec.setValue({          fieldId: 'subject',          value: 'Test Message'       });        messageRec.setValue({          fieldId: 'author',          value: 15 //internal id of author name       });        messageRec.setValue({          fieldId: 'authoremail',          value: 'name@example.com'       });        messageRec.setValue({          fieldId: 'recipient',            value: 164 //internal ID of recipient        });        messageRec.setValue({          fieldId: 'recipientemail',           value: 'name@example.com'       });        messageRec.setValue({          fieldId: 'cc',           value: 'name@example1.com, name@example2.com'        messageRec.setValue({          fieldId: 'bcc',     value: 'name@example3.com'       });        messageRec.setValue({          fieldId: 'message',          value: 'test message'       });        var custMessage = messageRec.save();        log.debug({title: 'message', details: custMessage          });       }       makeMessage();       });    }); ...` 
        

### Related Topics

-   [Sending Email from Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512629.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Communications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191061.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
