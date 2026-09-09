---
id: "section_N3438152"
type: "section"
title: "CustomFieldList"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services > CustomFieldList"
parent: "section_N3436475"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438152.html"
anchors: ["bridgehead_N3438503", "bridgehead_3819248826", "bridgehead_3819248985"]
sha256: "98743dcfb9496a58c3b05ec92492ecf690d2967ebf9934c2bc0f743a993a1ffc"
---

Most record types that are exposed through SOAP web services can have custom fields. Custom fields are contained in the customFieldList property on each record. The customFieldList property is an array of CustomFieldRef.

Note:

The Disable Mandatory Custom Field Validation preference determines whether a required custom field with no data provided throws an error, or is accepted as a null value. For more information about this preferences, see [Company-Wide Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3422217.html).

| Field Name | Type | Req. | Default | Notes |
| --- | --- | --- | --- | --- |
| customField | varies | Yes |  | Value of the custom field. Points to a type of CustomFieldRef in the XML Schema which is an abstract type. |
| internalID | string | Yes |  | The field instance internal ID |
| recType | string | No |  | The record type id |
| xsi:type | xsi:type | Yes |  | This is a field that is automatically implemented by the XML Schema. The value should represent the concrete custom field type. |

The following is an example that contains an excerpt of the SOAP body for a list of custom fields. It shows that the record associated with the SOAP contains four custom fields, all of which are referenced in the customFieldList property on the record.

          `<listRel:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">    <platformCore:customField internalId="72" scriptId="custentity_franchiseeabn_on_customerrec" xsi:type="platformCore:StringCustomFieldRef">       <platformCore:value>{partner.vatregnumber}</platformCore:value>    </platformCore:customField>    <platformCore:customField internalId="424" scriptId="custentity_score" xsi:type="platformCore:LongCustomFieldRef">       <platformCore:value>25</platformCore:value>    </platformCore:customField>    <platformCore:customField internalId="324" scriptId="custentity_expertise_level" xsi:type="platformCore:SelectCustomFieldRef">      <platformCore:value internalId="2">      <platformCore:name>Medium</platformCore:name>      </platformCore:value>    </platformCore:customField>    <platformCore:customField internalId="57" scriptId="custentity_633637_bsubmit" xsi:type="platformCore:BooleanCustomFieldRef">      <platformCore:value>false</platformCore:value>    </platformCore:customField> </listRel:customFieldList>` 
        

## Setting Custom Fields to NULL {#bridgehead_N3438503}

Custom fields can only be set to NULL by submitting the field in nullFieldList. For example, to set a custom field on a customer record to null, submit the following SOAP request, where custEntity9 is the custom field ID and 373 is the specific instance of the customer record:

          `<soap:Body>    <platformMsgs:update>       <platformMsgs:record internalId="373" xsi:type="listRel:Customer">          <platformCore:nullFieldList xsi:type="platformCore:NullField">             <platformCore:name>custEntity9</platformCore:name>          </platformCore:nullFieldList>       </platformMsgs:record>    </platformMsgs:update> </soap:Body>` 
        

Note:

You cannot set the Custom Form field to NULL. (This field is available on transaction and entry forms to indicate the form that should be used.) Any request to set it this field to NULL with nullFieldList will be ignored.

## Sample .NET Code {#bridgehead_3819248826}

          `Customer cust = new Customer(); cust.internalId = '373'; cust.nullFieldList = new String[]{"custentity9"};  _service.update(cust);` 
        

## Sample Java Code {#bridgehead_3819248985}

          `Customer cust = new Customer(); cust.setInternalId('373'); NullField nfl = new NullField(new String[]{"custentity9"});  cust.setNullFieldList(nfl); port.update(cust);` 
        

### Related Topics

-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
