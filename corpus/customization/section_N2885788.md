---
id: "section_N2885788"
type: "section"
title: "Parent-Child Record Relationships"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Parent-Child Record Relationships"
parent: "chapter_N2875173"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885788.html"
anchors: ["kaltura_player_279"]
sha256: "570c333f7a17300cafd6752142d5cd12aaa299e09cb8fa5d22cc032eb5db563a"
---

A child record type is a record that's referenced from another record in NetSuite. The information in the child record is associated with another record at a higher level, which is the parent record. You can use a child record to track multiple fields of specific information that are related to the parent record. Child records are always of the List/Record type. For more information, see [Using Child Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886136.html).

For example, a typical customer record may include sublists, represented as tables in subtabs on a form, for notes and messages record instances. In this case the customer record is a parent of the note and message child records. Therefore the notes and messages are child record instances of the customer record. The child record sublist name on the parent record are the plural forms of the child record types.

**Parent Record** - Customer

**Child Records** - Note, Message

**Child Record Sublists on the Parent Record** - Notes, Messages

You can also create custom parent-child relationships. For example, you can create a custom record type called Service Note and associate it with an Equipment custom record type. In this example, the Service Note record is associated as the child of the parent Equipment record type. On the Service Note record type definition, you can create custom fields for service person, price of service, whether the service was covered under warranty, and the equipment's next date of service. With this parent-child relationship established, defined as a custom field, employees can then view these service notes when working on the parent Equipment records.

Parent-child relationships can exist between:

-   Two standard records
    
-   Two custom records
    
-   One standard record and one custom record
    

The following diagram demonstrates the parent-child record relationship. In this example both the parent and child records are custom records.

![Parent-child record relationship diagram.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/ParentChild5.png)

To add a child record to a parent record, the parent record must already have been created and saved. When you reopen the parent record in edit mode, you can then add existing child records or create new ones. You can't add child records at the time when you're creating a new parent record.

Note:

A child record may not be available on a form for a parent record that was created through transformation from another record type. For example, if you define a custom record as a child record of sales order, this custom child record isn't available on forms for sales orders transformed from quotes

For more information, see the following topics:

-   [Establishing a Parent-Child Relationship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2885814.html)
    
-   [Creating a Parent-Child Relationship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158229389859.html)
    
-   [Types of Parent-Child Relationships](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158229565989.html)
    
-   [Using Child Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886136.html)
    

Watch the following video for an overview of parent-child record relationships.

<a id="kaltura_player_279"></a>

Also, see:

-   [Overview of Parent-Child Record Relationships (video 1 of 5)](https://videohub.oracle.com/media/Overview+of+Parent-Child+Record+Relationships+%28video+1+of+5%29/1_l91g63ws)
    
-   [Example of Creating a Parent-Child Relationship Between a Standard Record and a Custom Record (video 3 of 5)](https://videohub.oracle.com/media/Example+of+Creating+a+Parent-Child+Relationship+Between+a+Standard+Record+and+a+Custom+Record+%28video+3+of+5%29/1_1aoesf59)
    
-   [Example of Creating a Parent-Child Relationship Between Custom Records (video 4 of 5)](https://videohub.oracle.com/media/Example+of+Creating+a+Parent-Child+Relationship+Between+Custom+Records+%28video+4+of+5%29/1_jgi95zro)
    
-   [Types of Relationships Between Parent-Child Instances (video 5 of 5)](https://videohub.oracle.com/media/Types+of+Relationships+Between+Parent-Child+Instances+%28video+5+of+5%29/1_j95w4h4w)
    

### Related Topics

-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Creating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2876492.html)
-   [Sourcing with Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2886428.html)
-   [Updating Custom Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1501860753.html)
-   [Using Custom Record Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2888872.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
