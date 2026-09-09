---
id: "section_N3439676"
type: "section"
title: "Forms in SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > Records, Fields, Forms, and Sublists in SOAP Web Services > Forms in SOAP Web Services"
parent: "chapter_N3428523"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439676.html"
anchors: []
sha256: "27201963ea0af72af8be6cd8d1b12a7dd9d9afd0962245c6cff5c50895c2e41f"
---

If you are building a generic SOAP web services application, to ensure that your applications are account independent, you should create **custom 'Web-services-only' forms**. Use custom forms for SOAP web services requests by specifying the form in the _customForm_ element of a record. This will alleviate problems associated with customer-specific customizations to forms used in the UI that may break your SOAP web services application code.

Note:

If you are unfamiliar with NetSuite custom forms, see [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html). For information about creating custom forms that you can designate as 'web-services-specific,' see [Creating Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html).

For all record types that support custom forms, if a form is specified in the SOAP web services request, that form will be used for validation. Note that it is generally best practice to specify the custom form in all SOAP web services update operations. Also be aware that no record type is needed when specifying a custom form. You only need to specify the internal ID of the custom form.

To get the internal ID of a custom form, in the UI, go to Customization > Forms > \[ _form type_ \], where form type is either an entry or transaction form. The internal ID appears in the Internal ID column if the Show Internal IDs preference is enabled. (For steps on enabling this preference, see [Setting the Show Internal IDs Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3420345.html).)

To specify a form in SOAP web services, see the following C# snippet, which shows how to associate a particular form with a Customer record.

          `// create a customer object  Customer customer = new Customer();  customer.internalId = "555"  // create a custom form object  RecordRef customFormRef = new RecordRef();  // set the internal ID of the custom form. Get the internal ID from the UI  customFormRef.internalId = "-100";  // set the customForm field on the Customer record to reference the form  customer.customForm = customFormRef;` 
        

If a form is NOT specified, then the default preferred form for that record is used. If a custom form is saved with a record in the UI, that form is not used in the SOAP web services request unless it is also the default form for that record type or is explicitly set as the form in the SOAP web services request.

### Related Topics

-   [Records in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3428663.html)
-   [Fields in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3436475.html)
-   [Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3439908.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
