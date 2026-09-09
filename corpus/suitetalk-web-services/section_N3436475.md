---
id: "section_N3436475"
type: "section"
title: "Fields in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Fields in SOAP Web Services"
parent: "chapter_N3428523"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html"
anchors: []
sha256: "e6e399a618508814320cee2965fd77867db96eab0247c89e3e80262230053c68"
---

NetSuite records contain standard body fields and custom fields. Standard fields are those that are default in all NetSuite accounts. In SOAP web services, a record's standard body fields are its attributes, for example: `Customer.email, SalesOrder.salesRep`. Standard fields must be of one of the following logical types.

| Type | Description |
| --- | --- |
| String | Corresponds to the xsd:string type in the XML Schema |
| Int | Corresponds to the xsd:int type in the XML Schema |
| Double | Corresponds to the xsd:double in the XML Schema |
| Boolean | Corresponds to the xsd:boolean type in the XML Schema and has valid values of true or false. If not explicitly set to either true or false, then set as false. |
| Datetime | Corresponds to the xsd:dateTime type in the XML Schema which conforms to the ISO 8601 standard. |
| RecordRef | Corresponds to the RecordRef type in the XML Schema. References an nsKey value for any other record in the system including system defined constants that are controlled by the system. |
| Enum | Corresponds to a specific type defined as an enum in the XSD that represents system constants that are also available in the UI. |
| WsEnum | Corresponds to a specific type defined as an enum in the XSD that represents system constants that are NOT available in the UI. |
| List | A List references a type that is a list and should be explicitly defined in the in the XML Schema as a type. A list can either be null (if it is an optional field), or it must contain at least one entry unless otherwise noted. |

Custom fields are those that have been created by NetSuite users to customize their accounts. Custom fields can be added to an account using point-and-click customization tools. They can also be added through the SOAP web services [add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) operation. Custom fields must be one of the types defined in [Custom Field Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3458179.html).

On records, custom fields are contained in the customFieldList property. For more details, see [CustomFieldList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438152.html).

Note:

If you are getting unusual results in your SOAP web services queries, it may be that a standard field has been customized.

Consider the following general guidelines when working with both standard and custom fields.

-   If a **standard** field is set as mandatory in a custom form, the 'requiredness' of the field is honored in SOAP web services. If you do not provide value in your SOAP web services request for a field that is set as mandatory in a custom form, an error message is returned. For more information about NetSuite form types, see [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html).
    
-   Customizations made to **standard** fields are honored in SOAP web services. For example, if a standard field is set as disabled, it is not settable through SOAP web services, either. If you try to set such a field through SOAP web services, an error message is returned.
    
-   If a **standard** field is set to NOT show in the UI, it is not settable through SOAP web services, either. If you try to set such a field through SOAP web services, an error message is returned.
    
-   **Custom** display only (inline) and disabled fields are not settable through SOAP web services because these are NOT settable through the UI. If you provide a value in your SOAP web services request for such a field, an error message is returned. For information about field display types, see [Setting Display Options for Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2830238.html).
    
-   The get operation does not return the value of **custom** hidden fields.
    
-   Hidden fields are not readable in SOAP web services, but this does **not** apply to:
    
    -   Special SOAP web services fields, that are only listed in the data base.
        
    -   Time stamp fields like `lastModifiedDate, createdDate, created, lastModified`.
        
    -   The `externalID` field.
        
-   Defaulted fields that are set to blank on a SOAP web services update will stay blank on update.
    
-   The bodyFieldsOnly request-level preference affects the way formulas on forms are processed. Consequently, if the values of custom fields are calculated using formulas, the search might return incorrect results. If the calculated values of formulas are incorrect, set the bodyFieldsOnly preference to false to make sure the correct values are returned. For more information, see [Request-Level Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html).
    

Note:

If you are unfamiliar with NetSuite custom fields, you should see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html). This section describes the purpose and general characteristics of each custom field type, which will help you when working with the SOAP customization API (described in [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3768661.html)).

### Related Topics

-   [Field Lengths](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438979.html)
-   [Field Level Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439078.html)
-   [Required Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439180.html)
-   [Fields and Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439314.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
