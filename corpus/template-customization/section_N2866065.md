---
id: "section_N2866065"
type: "section"
title: "Adding Striping to Line Items in Advanced Templates"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced PDF/HTML Templates > Advanced Templates Customization in the Template Editor > Source Code Editing in the Template Editor > Adding Striping to Line Items in Advanced Templates"
parent: "section_4454200103"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2866065.html"
anchors: ["procedure_N2866098", "procedure_N2867962"]
sha256: "b0c6f3506be2922b8308067c9263d63b6981ebd82995a2891304511e2044fdda"
---

You can edit HTML markup source in the template editor to add striping to the line items table in an advanced template.

The syntax for adding striping to the line items tables relies on BFO (Big Faceless Organization), a set of third party libraries used by NetSuite for generating PDF documents. BFO documentation is available at [http://bfo.com/products/report/docs/userguide.pdf](http://bfo.com/products/report/docs/userguide.pdf).

Note:

If you're having issues with your advanced template, don't contact BFO directly. Always contact NetSuite Customer Support.

Warning:

Don't modify markup source directly unless you know CSS and HTML. NetSuite doesn't offer support or training in CSS or HTML.

Be aware that the template editor may not function properly if you switch back to WYSIWYG mode after you've made edits in markup source mode. Some template content may not display correctly, may not be accessible for editing, or may not display at all.

If these issues occur, you can preserve template content by not saving the template in WYSIWYG mode and switching back to markup source mode.

You can look up hex codes in the HTML color picker available in the template editor.

#### To add striping to a line items table: {#procedure_N2866098}

1.  Open the advanced template in the template editor, and click the **Source Code** switch.
    
2.  Scroll down to the portion of the HTML markup source relating to the rows in the line items table:
    
    ![Advanced PDF/HTML Templates sample code for adding striping to a line items table.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintSourceStriping1.png)
    
    Note:
    
    You should avoid using the `<tbody>` tag. BFO processing issues can result in an inability to save a template that includes this element.
    
3.  Edit the `<tr>` tag relating to rows in the line items table, to specify alternating colors for these rows, like the following example:
    
    `<tr>`
    
    In this example, even rows use the color represented in hexadecimal by `#ffffff` and odd rows use the color represented by `#ccffcc`.
    
    ![Advanced PDF/HTML Templates code example for adding color to even rows of a table.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintSourceStriping2.png)

To get hexadecimal codes for striping colors, you can look up hex codes in the HTML color picker provided in the template editor.

#### To get hexadecimal codes for striping colors: {#procedure_N2867962}

1.  In rich text editing mode, click the text color or background color button.
    
    ![Color buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintingColorOptions.jpg)
2.  Click More Colors.
    
    ![Select color window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintingMoreColorOptions.jpg)
3.  In the Select Color window, click a color to see the hex code.
    
    ![Select color window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintingColorPicker.jpg)

For example, you want your printed purchase orders to include borders and striping.

Edit the template markup source to add the table styles.

![Advanced PDF/HTML Templates example borders and striping code.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPDFHTMLStripingCode.png)

A purchase order that uses the table styles shown will display striping and dotted borders.

![Advanced PDF/HTML Templates sample Purchase Order showing striping and dotted borders.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPDFHTMLStripingExample.png)

### Related Topics

-   [Source Code Editing in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454200103.html)
-   [Source Code Editing to Customize Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454208098.html)
-   [Syntax for Advanced Template Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864199.html)
-   [Setting a Template to Use a Font Unavailable in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4549515329.html)
-   [Adding Files to Advanced PDF Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0414122450.html)
-   [Languages for Printed Forms that Use Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3963046048.html)
-   [Adding Translated Content in Advanced Printouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156623786181.html)
-   [Adding Page Breaks to Tables](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4418819945.html)
-   [Printing Subsidiary Logo on Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4407559296.html)
-   [Adding Apply Sublist to Check Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4824042035.html)
-   [Using FreeMarker to Work with Hidden Fields Used in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156752233995.html)
-   [Adding Bar Codes in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950986185.html)
-   [XML Formatting in Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158204583926.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
