---
id: "section_N2873464"
type: "section"
title: "Transaction Form HTML Layouts"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Basic Printing Layouts > Transaction Form HTML Layouts"
parent: "chapter_4453552264"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873464.html"
anchors: ["subsect_163733107381", "procedure_N2873565"]
sha256: "185127aa5a6d4f41b865f672874c25d8a86395fa1d2af71a377f178c4f4264c3"
---

Transaction form HTML layouts define the arrangement of fields on HTML transaction documents in NetSuite. Standard and Classic HTML layouts exist for all the standard form types other than shipping label and item label - these are assumed to be printed using PDF. For more information, see [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html). You can use HTML layouts to generate customized email versions of transactions forms.

Important:

Basic layouts will be deprecated in a future release. We encourage you to use Advanced PDF/HTML Templates instead because new features are added exclusively to advanced printing. For information, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

You can customize transaction form HTML layouts by editing the templates on which they are based. The templates for each layout consist of two blocks of HTML:

-   **Style Block** : this block begins with `<style>` and ends with `</style>`. The style block defines the styles used by the layout.
    
-   **Body Block** : this block begins with `<table>` and ends with `</table>`. The body block defines the content of the HTML page.
    

When you print using the Classic HTML Transaction Layout template, the header information, including the logo, is printed on every page of the HTML printout. To print the logo and other header information only on the first page, use the Standard HTML Transaction Layout template. You can also customize the classic template and remove the `<thead>` and `</thead>` tags.

Totaling works the same way as it does for Transaction Form PDF Layouts. For more information, see [Totals Transaction Form Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873768.html).

Note:

Advanced PDF/HTML templates provide an alternative model for customizing printed and emailed records. They support more customization capabilities than transaction form layouts. For details, see [Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453550706.html).

## Creating Custom Transaction Form HTML Layouts {#subsect_163733107381}

You can customize transaction form HTML layouts.

#### To customize a transaction form HTML layout: {#procedure_N2873565}

1.  Go to _Customization > Forms > Transaction Form HTML Layouts_.
    
2.  Click **Customize** next to the layout you want to customize.
    
3.  In the **Label** field, enter the name of your customized layout.
    
4.  Check the **Layout is Inactive** box to remove this layout as an option in dropdown lists. You can always clear this box later and the layout is available again.
    
5.  Check the **Layout is Preferred** box to make this layout your preferred layout for this type of transaction.
    
6.  On the **Templates** subtab, edit the **Style** and **Body** blocks as needed.
    
    Embedded in the body block are NetSuite tags that correspond to individual content elements. The content elements correspond closely to the layout elements in the existing PDF layouts. Basic customization consists of editing the body or style templates but leaving all of the NetSuite tags in the body block.
    
    For example, to create a collection layout you could add a block of text at the top of the body layout.
    
7.  If needed, click **Elements** and customize the HTML that corresponds to each element.
    
    On the **Elements** subtab, each element is listed with the corresponding element ID, the HTML code that will be used to display the label that corresponds to the element, and the HTML code that will be used to display the data that corresponds to the element.
    
    When editing the HTML for elements, follow these guidelines:
    
    -   Ensure that the HTML used correlates to any formats as defined in the body block. For example, if the element is included in a `<table>` tag in the body block, the element itself must begin with a `<tr>`.
        
    -   Elements always have data and can have a label.
        
    -   The label is represented by the `<nllabel>` tag that must be included in any customization of the label field.
        
    -   The data is represented by the `<nldata>` tag that must be included in any customization of the data field.
        
    -   There is also a `<nlattributes>` tag that is used in the COLUMNS element to indicate where text formatting elements (such as alignment) are inserted.
        
    -   The BODY, COLUMNS, and AGING elements are repeated to produce the HTML of the form.
        

### Related Topics

-   [Basic Printing Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4453552264.html)
-   [Customizing Transaction Form PDF Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2869660.html)
-   [Totals Transaction Form Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873768.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
