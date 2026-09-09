---
id: "section_N3458179"
type: "section"
title: "Custom Field Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Types > Custom Field Types"
parent: "chapter_N3452524"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html"
anchors: ["bridgehead_N3458594", "bridgehead_N3458748", "bridgehead_N3458947", "bridgehead_N3459146", "bridgehead_N3459345", "bridgehead_N3459544", "bridgehead_N3459822", "bridgehead_N3460021", "bridgehead_N3460220", "bridgehead_N3460361"]
sha256: "b02f12c84264b9868f577a3716d76dc5e95a856b0eade775656a06537aced11c"
---

Custom fields are represented by the type [CustomFieldRef](#bridgehead_N3458594), which is an abstract type. The table below contains a list of concrete custom field types that extend the CustomFieldRef type. Each type is followed by its corresponding type in the UI.

| XML Schema Type | Custom Field Type in UI |
| --- | --- |
| [LongCustomFieldRef](#bridgehead_N3458748) | Integer |
| [DoubleCustomFieldRef](#bridgehead_N3458947) | Decimal Number |
| [BooleanCustomFieldRef](#bridgehead_N3459146) | Check Box |
| [StringCustomFieldRef](#bridgehead_N3459345) | 
Free-Form Text

Text Area

Phone Number

E-mail Address

Hyperlink

Rich Text



 |
| [DateCustomFieldRef](#bridgehead_N3459544) | 

Date

Time of Day

or Date/Time (both in one field) |
| [SelectCustomFieldRef](#bridgehead_N3459822) | 

List/Record

Document



 |
| [MultiSelectCustomFieldRef](#bridgehead_N3460021) | Multiple Select |

## CustomFieldRef {#bridgehead_N3458594}

The CustomFieldRef type is an abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

To locate the internal ID for a specific custom field in the UI, go to Customization > Lists, Records, & Fields > _\[Custom Field\]_ (where _\[Custom Field\]_ is the type of custom field such as CRM). The internal IDs for each custom field that has been created is listed in the ID column in the UI.

## LongCustomFieldRef {#bridgehead_N3458748}

The LongCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | xsd:int | Y |  |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## DoubleCustomFieldRef {#bridgehead_N3458947}

The DoubleCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | xsd:double | Y |  |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## BooleanCustomFieldRef {#bridgehead_N3459146}

The BooleanCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | xsd:boolean | Y |  |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## StringCustomFieldRef {#bridgehead_N3459345}

The StringCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | xsd:string | Y |  |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## DateCustomFieldRef {#bridgehead_N3459544}

The DateCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | xsd:datetime | Y |  |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## SelectCustomFieldRef {#bridgehead_N3459822}

The SelectCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type. This references a single ListOrRecordRef and also requires an InternalId attribute to indicate the field name.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | ListorRecordRef | Y | A single ListOrRecordRef. |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## MultiSelectCustomFieldRef {#bridgehead_N3460021}

The MultiSelectCustomFieldRef type extends the [CustomFieldRef](#bridgehead_N3458594) abstract type. This references an array of ListOrRecordRef's and also requires an internalId attribute to indicate the field name.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | ListorRecordRef\[\] | Y | An array of type RecordRef |
| internalId | xsd:string (attribute) | Y | References a unique instance of a custom field type. |

## CustomFieldList {#bridgehead_N3460220}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| value | customFieldRef \[\] | Y | An array of type customFieldRef. The actual entries in the array will be of a concrete type that extends customFieldRef. |

The following is an XML excerpt from a SOAP body that illustrates a custom field list that contains all the available custom field types.

## SOAP Sample {#bridgehead_N3460361}

          `<listRel:customFieldList xmlns:platformCore="urn:core_2017_1.platform.webservices.netsuite.com">  <platformCore:customField internalId="526" scriptId="custentity_exchange_rate" xsi:type="platformCore:DoubleCustomFieldRef">    <platformCore:value>2.35</platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="524" scriptId="custentity_soft_skills" xsi:type="platformCore:MultiSelectCustomFieldRef">    <platformCore:value internalId="1">       <platformCore:name>Communication</platformCore:name>    </platformCore:value>    <platformCore:value internalId="5">       <platformCore:name>Teamwork</platformCore:name>    </platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="146" scriptId="custentity_checkbox" xsi:type="platformCore:BooleanCustomFieldRef">    <platformCore:value>false</platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="525" scriptId="custentity_first_contact" xsi:type="platformCore:DateCustomFieldRef">    <platformCore:value>2017-03-16T00:00:00.000-07:00</platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="324" scriptId="custentity_proficiency_level" xsi:type="platformCore:SelectCustomFieldRef">    <platformCore:value internalId="2">       <platformCore:name>Medium</platformCore:name>    </platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="72" scriptId="custentity_franchiseeabn_on_customerrec" xsi:type="platformCore:StringCustomFieldRef">    <platformCore:value>{partner.vatregnumber}</platformCore:value>  </platformCore:customField>  <platformCore:customField internalId="424" scriptId="custentity_test_score" xsi:type="platformCore:LongCustomFieldRef">    <platformCore:value>25</platformCore:value>  </platformCore:customField> </listRel:customFieldList>` 
        

### Related Topics

-   [Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html)
-   [Built-in Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452691.html)
-   [Complex Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html)
-   [Search Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html)
-   [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
