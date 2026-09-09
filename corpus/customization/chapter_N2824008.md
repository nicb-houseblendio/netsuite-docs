---
id: "chapter_N2824008"
type: "chapter"
title: "Customization Overview"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Customization Overview"
parent: "book_N2823893"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2824008.html"
anchors: ["svg_1", "svg_1Layer_3", "svg_1Layer_1", "svg_1Node", "bridgehead_N2824032", "bridgehead_N2824091", "bridgehead_1542222963", "bridgehead_1542223016", "bridgehead_1542223027", "article_159604510519", "section_N2824537"]
sha256: "4f997718a75837acb4a12dd241c607d0985cbe5d89c20543babf8a56cd7b441d"
---

With the customization tools, you can tailor NetSuite to your individual business needs and processes. Customization provides a point-and-click interface for creating various components, such as fields, forms, and record types. Customization also lets you define how information is accessed and entered by each user of your NetSuite account.

<a id="svg_1"></a>

                                                                                                                                                                                       

## Customization Users {#bridgehead_N2824032}

There are three types of Customization users:

-   **Administrators** - Administrators spend time customizing transaction forms, adding custom record types, and setting up custom centers for roles within the company. Some of the customization work is unique to a specific business. Administrators also assign roles to each NetSuite user. Each user's role determines which information they can access in your NetSuite account.
    
-   **IT Staff** - Issues addressed by the IT department often include requests for changes to the NetSuite account. These issues can range from small tasks such as adding a field to a form, to larger work items like creating custom record types. IT staff members can access administrative tools to manage data and schedule batch processing jobs.
    
-   **Developers** - For developers of partner solutions and independent software vendors (ISVs), most of their time with NetSuite is spent coding SuiteScript and SOAP web services. To use these features, developers need to understand how customization objects interact with their code.
    

## Customizing NetSuite Components {#bridgehead_N2824091}

No matter your experience with other software applications, Customization can help you set up NetSuite quickly. Use Customization to customize the components that control how your users interact with NetSuite.

## Access Information {#bridgehead_1542222963}

To define how users interact with NetSuite and what data they have access to, you can configure these components.

| Component | Description | More Information |
| --- | --- | --- |
| Role | Set of permissions that can be assigned to a NetSuite user | [Customizing and Creating Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N286284.html) |
| Center | Configuration of NetSuite created for a specific group of roles with similar tasks. | [Creating and Editing Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890334.html) |
| Center tab | Section of NetSuite that groups similar links and other information. Standard tabs include Home, Reports, Documents, Activities, and Setup. You can also create custom center tabs. | [Creating Center Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2890512.html) |

## Set Up Data {#bridgehead_1542223016}

To define how to get the most out of your NetSuite implementation, use these components to configure your data.

| Componet | Description | More Information |
| --- | --- | --- |
| Record | A single entry of information related to a single business concept. Use custom records to collect information specific to the needs of your business. | [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html) |
| Segment | A single entry of information related to a single business concept. Use custom segments to create custom classification fields similar to class, department, and location. | [Custom Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4313464438.html) |
| Transaction | A single entry of information related to a single business concept. Use custom transactions to create transaction types tailored to your business needs. | [Custom Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4172599049.html) |
| List | List of values that can be selected in a custom field. Use custom lists to set up predefined choices for your employees and customers to select when entering transactions and records. | [Custom Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2852109.html) |
| Template | A single entry of information related to a single business concept. Use advanced templates to customize printed and emailed forms, records, and saved searches. | [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html) |

## Collect and Display Data {#bridgehead_1542223027}

To collect and display data within NetSuite, you must use forms. A form is a page through which you enter records and transactions. Use these components to build your own forms or customize an existing form.

| Component | Description | More Information |
| --- | --- | --- |
| Field | Place on a record or transaction where information is entered. | [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html) |
| Subtab | Section of a record or transaction that groups similar fields. An example of a standard subtab is the Address subtab where the shipping and billing addresses are entered on transactions and records. | [Creating Custom Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2862348.html) |
| Sublist | The results of a saved search displayed on a custom or standard record. Sublists can also be generated through parent-child relationships. | [Custom Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861522.html) |
| Script | SuiteScript JavaScript file that runs against a specific form or record type or that creates a custom portlet. Scripts can also be scheduled to perform periodically. | [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html) |

## Customization Objects in SDF {#article_159604510519}

You can manage custom objects in SuiteCloud Development Framework (SDF). SDF uses XML definitions of custom objects to work with the object attributes, fields, fields structures, field properties, field values, and other details. For more information, see [SuiteCloud Development Framework XML Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml.html).

If the Multi-Languages feature is enabled in your account, you can define translated labels of customization objects, records, or fields to be used for various language settings. For more information, see [Manage Translations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158572305264.html) and [SuiteApp Translatability Support](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158572327037.html).

When working with custom objects that have translatable fields, you can use a translation string from a collection. For more information about translatable fields, see [Translatable Fields on SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156951732735.html) and [Translatable Fields in SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_158572346302.html#subsect_159007422425).

For more information about developing custom objects in SDF, see [SDF Custom Object and File Development in SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4715411907.html).

## Customize Your NetSuite Account {#section_N2824537}

Now that you know what components can be customized, explore the following topics to learn more about customizing your NetSuite account:

-   [Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2824615.html)
    
-   [Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2824771.html)
    
-   [Transaction Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542227073.html)
    
-   [Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542227070.html)
    
-   [Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542227029.html)
    
-   [Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2824967.html)
    

### Related Topics

-   [Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N2823893.html)
-   [Customization Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163039950342.html)
-   [Customizing Field Level Help for Standard Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1530729846.html)
-   [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html)
-   [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html)
-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Custom Transactions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4172599049.html)
-   [Custom Segments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4313464438.html)
-   [Custom Centers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2890160.html)
-   [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
