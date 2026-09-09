---
id: "section_N3460474"
type: "section"
title: "Search Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Types > Search Types"
parent: "chapter_N3452524"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3460474.html"
anchors: ["bridgehead_N3460570", "bridgehead_N3460583", "bridgehead_N3460836", "bridgehead_N3461018", "bridgehead_N3461474", "bridgehead_N3461684", "bridgehead_N3461822", "bridgehead_N3462646", "bridgehead_N3462885", "bridgehead_N3463126", "bridgehead_N3463443", "bridgehead_N3463650", "bridgehead_N3463849", "bridgehead_N3463862", "bridgehead_N3464002", "bridgehead_N3464245", "bridgehead_N3464431", "bridgehead_N3465812", "bridgehead_N3466100", "bridgehead_N3466433", "bridgehead_N3466677", "bridgehead_N3466920", "bridgehead_N3467057", "bridgehead_N3467069", "bridgehead_N3467210", "bridgehead_N3467350", "bridgehead_N3467490", "bridgehead_N3467631", "bridgehead_N3467771", "bridgehead_N3467912", "bridgehead_N3468052", "bridgehead_N3468193", "bridgehead_N3468333", "bridgehead_N3468346", "bridgehead_N3468487", "bridgehead_N3468673", "bridgehead_N3468859", "bridgehead_N3469045", "bridgehead_N3469231", "bridgehead_N3469417", "bridgehead_N3469603", "bridgehead_N3469789", "bridgehead_N3469975", "bridgehead_N3471212", "bridgehead_3705183312"]
sha256: "b1046720a53799b8df70f7daf94f17bf12354d98b225e2b9f2a6df5d7b7c0573"
---

Every NetSuite record that supports search has corresponding search and advanced search objects. For example, the SOAP listRel XSD contains a Customer object, as well as its corresponding CustomerSearch, CustomerSearchAdvanced, and CustomerSearchRow search objects.

-   When using a < _Record_ > **Search** object, all search fields within this search object belong to one of the types decribed in [Search XML Schema Types](#bridgehead_N3460570).
    
-   When searching on custom records or custom fields, all search fields belong to one of the types described in [Search Custom Field XML Schema Types](#bridgehead_N3463849).
    
-   When using either the < _Record_ > **SearchAdvanced** or < _Record_ > **SearchRow** search objects, all search fields within these 'advanced search' objects belong to one of the types described in [Search Column Custom XML Schema Types](#bridgehead_N3468333) or [Search Column Custom XML Schema Types](#bridgehead_N3468333).
    

## Search XML Schema Types {#bridgehead_N3460570}

The following sections define available search types. Every search field within a search object type belongs to one of these search types.

## SearchPreferences {#bridgehead_N3460583}

| Field Name | XML Schema Type | Req |
| --- | --- | --- |
| bodyFieldsOnly | boolean | Y/N |
| pageSize | int | Y/N |
| returnSearchColumns | boolean | Y/N |

## SearchRequest {#bridgehead_N3460836}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| preferences | boolean | Y |  |
| searchRecord | SearchRecord | Y |  |

## SearchResult {#bridgehead_N3461018}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| totalRecords | int | N |  |
| pageSize | int | N |  |
| totalPages | int | N |  |
| pageIndex | int | N |  |
| searchId | string | N |  |
| status |  |  |  |
| recordList | platformCore:RecordList |  |  |
| searchRowList | platformCore:SearchRowList |  |  |

## SearchStringField {#bridgehead_N3461474}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | 
platformCoreTyp:

SearchStringFieldOperator (attribute)



 | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:string | Y |  |

## SearchBooleanField {#bridgehead_N3461684}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | xsd:boolean | Y | The available values are true or false. |

## SearchDoubleField {#bridgehead_N3461822}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchDoubleFieldOperator(attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:double | Y |  |
| searchValue2 | xsd:double | N | If the operator is between or notBetween searchValue2 must be populated. |

## SearchLongField {#bridgehead_N3462646}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchLongFieldOperator(attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:long | Y |  |
| searchValue2 | xsd:long | N | If the operator is between or notBetween searchValue2 must be populated. |

## SearchTextNumberField {#bridgehead_N3462885}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchTextNumberFieldOperator (attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:string | Y |  |
| searchValue2 | xsd:string | N | If the operator is between or notBetween searchValue2 must be populated. |

## SearchDateField {#bridgehead_N3463126}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchDate (attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| predefinedSearchValue | plateformCoreTyp: SearchDate | N | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:dateTime | N | Either predefinedSearchValue or searchValue should be populated. |
| searchValue2 | xsd: dateTime | N | If the operator is between or notBetween searchValue2 must be populated. |

## SearchMultiSelectField {#bridgehead_N3463443}

This search type is used to specify a list of one or more internal IDs that reference other user defined records in the system.

Note:

Note that the maximum number of values that can be specified in a MultiSelectField is 1000.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchMultiSelectFieldOperator (attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | platformCore: RecordRef | Y | An array of type SearchMultiSelectRefValue. |

## SearchEnumMultiSelectField {#bridgehead_N3463650}

This search type is used to specify a list of one or more system defined constants.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| operator | platformCoreTyp: SearchEnumMultiSelectFieldOperator (attribute) | Y | Reference to a value in a system list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:string | Y |  |

## Search Custom Field XML Schema Types {#bridgehead_N3463849}

The following sections define the available search types for custom fields. Every search field within a search object type belongs to one of these search types.

## SearchCustomField {#bridgehead_N3463862}

This is an abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| id | xsd:string (attribute) | Y | References a unique instance of a custom field |

## SearchStringCustomField {#bridgehead_N3464002}

The SearchStringCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchStringFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:string | Y |  |

## SearchBooleanCustomField {#bridgehead_N3464245}

The SearchBooleanCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| searchValue | xsd: boolean | Y | The type is an enumeration type that restricts the value to true or false. |

## SearchLongCustomField {#bridgehead_N3464431}

The SearchLongCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchLongFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:long | Y |  |
| searchValue2 | xsd:long | N |  |

## SearchDoubleCustomField {#bridgehead_N3465812}

The SearchDoubleCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchDoubleFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:double | Y |  |
| searchValue2 | xsd:double | N |  |

## SearchDateCustomField {#bridgehead_N3466100}

The SearchDateCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchDateFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| predefinedSearchValue | platformCoreTyp: SearchDate |  |  |
| searchValue | xsd:dateTime | Y |  |
| searchValue2 | xsd:dateTime | Y |  |

## SearchMultiSelectCustomField {#bridgehead_N3466433}

The SearchMultiSelectCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchMultiSelectFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | ListOrRecordRef | Y |  |

## SearchEnumMultiSelectCustomField {#bridgehead_N3466677}

The SearchEnumMultiSelectCustomField type extends the SearchCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| internalId | xsd:string (attribute) | Y | Inherited from the SearchCustomField. Reference a unique instance of a custom field. |
| operator | platformCoreTyp: SearchEnumMultiSelectFieldOperator (attribute) | Y | The type is an enumeration type that restricts the value to a predefined list. For more information on available values, see [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html). |
| searchValue | xsd:string | Y |  |

## SearchCustomFieldList {#bridgehead_N3466920}

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| customField | platformCore: SearchCustomField \[\] | Y |  |

## Search Column XML Schema Types {#bridgehead_N3467057}

The following search types support advanced search functionality in SOAP web services.

## SearchColumnField {#bridgehead_N3467069}

This is an abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| customLabel | xsd:string |  |  |

## SearchColumnBooleanField {#bridgehead_N3467210}

The SearchColumnBooleanField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:boolean | Y |  |

## SearchColumnStringField {#bridgehead_N3467350}

The SearchColumnStringField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:string | Y |  |

## SearchColumnLongField {#bridgehead_N3467490}

The SearchColumnLongField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:long | Y |  |

## SearchColumnTextNumberField {#bridgehead_N3467631}

The SearchColumnStringField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:string | Y |  |

## SearchColumnDoubleField {#bridgehead_N3467771}

The SearchColumnDoubleField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:double | Y |  |

## SearchColumnDateField {#bridgehead_N3467912}

The SearchColumnDateField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:dateTime | Y |  |

## SearchColumnEnumSelectField {#bridgehead_N3468052}

The SearchColumnEnumSelectField type extends the SearchColumnField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:string | Y |  |

## SearchColumnSelectField {#bridgehead_N3468193}

The SearchColumnSelectField type extends the SearchColumnField abstract type. This references a single ListOrRecordRef and also requires an internalId attribute to indicate the field name.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | RecordRef | Y |  |

## Search Column Custom XML Schema Types {#bridgehead_N3468333}

The following search types support advanced search functionality in SOAP web services.

## SearchColumnCustomField {#bridgehead_N3468346}

This is an abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| customLabel | xsd:string |  |  |

## SearchColumnBooleanCustomField {#bridgehead_N3468487}

The SearchColumnBooleanField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:boolean | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnStringCustomField {#bridgehead_N3468673}

The SearchColumnStringCustomField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:string | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnLongCustomField {#bridgehead_N3468859}

The SearchColumnLongCustomField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:long | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnDoubleCustomField {#bridgehead_N3469045}

The SearchColumnDoubleCustomField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:double | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnDateCustomField {#bridgehead_N3469231}

The SearchColumnDateCustomField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:dateTime | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnEnumMultiSelectCustomField {#bridgehead_N3469417}

The SearchColumnEnumMultiSelectCustomField type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | xsd:string | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnSelectCustomField {#bridgehead_N3469603}

The SearchColumnSelectCustomField type extends the SearchColumnCustomField abstract type. This references a single ListOrRecordRef and also requires an internalId attribute to indicate the field name.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | ListOrRecordRef | Y | A single ListOrRecordRef |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnMultiSelectCustomField {#bridgehead_N3469789}

The SearchColumnMultiSelectCustomField type extends the SearchColumnCustomField abstract type. This references an array of ListOrRecordRefs.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| searchValue | ListOrRecordRef\[\] | Y |  |
| internalId | xsd:string (attribute) | Y |  |

## SearchColumnCustomFieldList {#bridgehead_N3469975}

The SearchColumnCustomFieldList type extends the SearchColumnCustomField abstract type.

| Field Name | XML Schema Type | Req | Notes |
| --- | --- | --- | --- |
| customField | SearchColumnCustomField |  |  |

## Sample Code {#bridgehead_N3471212}

## SOAP Request - Opportunity Search {#bridgehead_3705183312}

Following is an example that contains an excerpt of the SOAP body that illustrates an opportunity search containing several search field types.

          `<opportunitySearch>       <projectedTotal operator="lessThan">          <searchValue>100000</searchValue>       </projectedTotal>       <title operator="contains">          <searchValue>Enterprise</searchValue>       </title>       <createdDateRange operator="between">          <fromValue>2003-10-02</fromValue>          <toValue>2003-10-12</toValue>       </createdDateRange>       <opportunityStatusList operator="anyOf">          <searchValue>inProgress</searchValue>          <searchValue>closedWon</searchValue>       </opportunityStatusList>       <customFieldList>          <customField xsi:type="SearchSelectCustomField" internalId="35" scriptId="cust_SalesEngineer"           operator="equals">             <searchValue>Buddy Williams</searchValue>          </customField>          <customField xsi:type="SearchBooleanCustomField" internalId="165" scriptId="cust_hasSalesEngineer"           operator="true"/>          <customField xsi:type="SearchStringCustomField" internalId="322" scriptId="cust_DemoNotes"           operator="startsWith">             <searchValue>CRM</searchValue>          </customField>          <customField xsi:type="SearchMultiSelectCustomField" internalId="155" scriptId="cust_ProductAreas"           operator="noneOf">             <searchValue>Inventory</searchValue>             <searchValue>Warehousing</searchValue>          </customField><       </customFieldList>  </opportunitySearch>` 
        

### Related Topics

-   [Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html)
-   [Built-in Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452691.html)
-   [Complex Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html)
-   [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html)
-   [Platform Enumerations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3471338.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
