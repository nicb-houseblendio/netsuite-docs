---
id: "section_N2868543"
type: "section"
title: "Generating Custom Bar Codes in Advanced Templates"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced PDF/HTML Templates > Advanced Templates Customization in the Template Editor > Source Code Editing in the Template Editor > Adding Bar Codes in Advanced Templates > Generating Custom Bar Codes in Advanced Templates"
parent: "section_3950986185"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2868543.html"
anchors: []
sha256: "416e863f27630fcbac9d2908da25ce158bd84c257e9fc14dded3b67db1964f1e"
---

You can edit the HTML markup source of your advanced template to add a custom bar code or QR code for any custom transaction you need. For example, you can add a custom bar code to a warehouse picking ticket. With a bar code scanner, a warehouse employee can retrieve relevant inventory information needed to complete the order.

In the Advanced Template Editor, edit the HTML markup source and use the BFO tag `<barcode />` to create a custom bar code. For more information about editing the source code, see [Source Code Editing in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454200103.html).

Warning:

Don't modify markup source directly unless you have sufficient CSS and HTML knowledge. NetSuite doesn't provide support or training in CSS or HTML.

Be aware that the template editor may not function properly if you switch back to WYSIWYG mode after you have made edits in markup source mode. Some template content may not be represented correctly, may not be accessible for editing, or may not be displayed at all.

If these issues occur, you can preserve template content by not saving the template in WYSIWYG mode and switching back to markup source mode.

To add a custom bar code to an advanced template:

1.  Open the advanced template in the template editor and click the **Source Code** switch.
    
2.  Scroll down to the portion of the HTML markup source where you want to create a bar code. Add the following code to the template and specify the `codetype`, `showtext`, and `value` parameters as required.
    
                  `<barcode codetype="qrcode" showtext="false" height="150" width="150" value="http://www.example.com/" />` 
                
    

Note:

Your custom bar code won't be visible in the Advanced Template Editor. You must generate a report using your template to see the bar code.

| Parameter | Type | Required/Optional | Description |
| --- | --- | --- | --- |
| `codetype` | string | required | Choose the bar code algorithm used to generate the bar code. For a list of supported bar code algorithms, see the following table. |
| `showtext` | boolean `true` | `false` | required | If set to `true`, a readable version of the value is printed below the bar code. If set to `false`, no readable information is displayed. **Note:** The following bar code types don't display the printed values below the bar code: `aztec`, `deutchepostmatrix`, `intelligentmail`, `maxicode`, `pdf417`, `postnet`, `qrcode`, and `rm4scc`. |
| `value` | string | required | Enter the information you want to encode using the bar code algorithm. Use the following table to decide which bar code type matches your needs - each type has its own length and character requirements. For example, you can encode a URL in an `aztec` , `maxicode`, or `qrcode` by setting the value to "http://www.example.com". Alternatively, you can encode a serial number in a `upca`, `postnet` , or `code25` bar code by setting the value to "0123456789". **Note:** If value contains characters that the bar code algorithm doesn't support, your template can generate an error. Confirm that the bar code algorithm supports the requirements of the value string. |
| `height` | number | optional | Set the height of the bar code in pixels. Some bar code algorithms might ignore this parameter. **Note:** The height parameter is required for the `qrcode`. |
| `width` | number | optional | Set the width of the bar code in pixels. Some bar code algorithms might ignore this parameter. **Note:** The width parameter is required for the `qrcode`. |

The following bar code algorithms are supported by advanced templates and the BFO report generator. For more information about each bar code type, see [http://bfo.com/products/report/docs/userguide.pdf](http://bfo.com/products/report/docs/userguide.pdf).

| `codetype` | Type | Supported Characters | Length | Example (with `showtext = true`) |
| --- | --- | --- | --- | --- |
| `aztec` | 2D matrix | 
-   Full ASCII
-   FNC1 and ESI control codes

 | 12 - 3832 | ![Sample aztec barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-aztec.png) |
| `codabar` | Linear | 

-   Numbers 0-9
-   Symbols : - . $ / +

 | Variable **Note:** Requires a Start and Stop character Use one of the following characters for the Start and Stop character: A, B, C, D, E, \*, N, T | ![Sample codabar barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-codabar.png) |
| `code25` | Linear | 

-   Numbers 0-9

 | Variable | ![Sample code25 barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-code25.png) |
| `code25checksum/code25deutschenpost` | Linear | 

-   Numbers 0-9

 | Variable | ![Sample code25checksum barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-code25checksum.png) |
| `code39` | Linear | 

-   Uppercase letters A-Z
-   Number 0-9
-   Symbols - . $ / + % Space

 | Variable | ![Sample code39 barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-code39.png) |
| `code39checksum` | Linear | 

-   Uppercase letters A-Z
-   Number 0-9
-   Symbols - . $ / + % Space

 | Variable | ![Sample code39checksum barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-code39checksum.png) |
| `code128` | Linear | 

-   Full ASCII
-   Control Codes

 | Variable | ![Sample code128 barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-code128.png) |
| `databar` | Linear | 

-   Number 0-9

 | 14 Maximum | ![Sample databar barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-databar.png) |
| `datamatrix` | 2D matrix | 

-   Full ASCII

 | 2335 Maximum | ![Sample datamatrix barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-datamatrix.png) |
| `deutchepostmatrix` | 2D matrix | 

-   Full ASCII

 | 2335 Maximum | ![Sample deutchepostmatrix barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-deutschepostmatrix.png) |
| `ean8` | Linear | 

-   Numbers 0-9

 | 7 + checkdigit | ![Sample ean8 barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-ean8.png) |
| `ean13/upca` | Linear | 

-   Numbers 0-9

 | 13+ checkdigit | ![Sample ean13/upca barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-ean13-upac.png) |
| `intelligentmail` | 2D height | 

-   Numbers 0-9

 | 20, 25, 29, or 31 digits | ![Sample intelligentmail barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-intelligentmail.png) |
| `maxicode` | 2D matrix | 

-   Full ASCII

 | Maximum 92 ASCII characters | ![Sample maxicode barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-maxicode.png) |
| `pdf417` | 2D stacked | 

-   Full ASCII

 | Maximum 1850 ASCII characters or 2725 numeric characters | ![Sample pdf417 barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-pdf417.png) |
| `postnet` | Linear | 

-   Numbers 0-9

 | 5, 9, or 11 + check digits | ![Sample postnet barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-postnet.png) |
| `qrcode` | 2D matrix | 

-   Full ASCII

 | Maximum 1520 ASCII characters or 2509 numeric characters | ![Sample qrcode barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-qrcode.png) |
| `rm4scc` | 2D height | 

-   Uppercase letters A-Z
-   Number 0-9

 | Variable | ![Sample rm4scc barcode](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/barcode-rm4scc.png) |

### Related Topics

-   [Source Code Editing in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454200103.html)
-   [Source Code Editing to Customize Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454208098.html)
-   [Syntax for Advanced Template Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864199.html)
-   [Setting a Template to Use a Font Unavailable in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4549515329.html)
-   [Languages for Printed Forms that Use Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3963046048.html)
-   [Adding Striping to Line Items in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2866065.html)
-   [Adding Page Breaks to Tables](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4418819945.html)
-   [Printing Subsidiary Logo on Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4407559296.html)
-   [Adding Apply Sublist to Check Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4824042035.html)
-   [Using FreeMarker to Work with Hidden Fields Used in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156752233995.html)
-   [Adding Bar Codes in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950986185.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
