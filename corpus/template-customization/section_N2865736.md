---
id: "section_N2865736"
type: "section"
title: "Adding Tables to Advanced Templates"
branch: "template-customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Template Customization > Advanced PDF/HTML Templates > Advanced Templates Customization in the Template Editor > WYSIWYG Editing in the Template Editor > Adding Tables to Advanced Templates"
parent: "section_4454197641"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2865736.html"
anchors: ["procedure_N2865756"]
sha256: "3f55346a9ea5f48c1c5e541a9c0d33da504caefaa3eeaf9c342efc1044a8652d"
---

The New Element toolbar of the template editor includes a button that you can click to insert tables on advanced PDF/HTML templates.

Note:

For better performance, you shouldn't use nested tables, that is, tables within tables.

#### To insert a table on an advanced template: {#procedure_N2865756}

1.  Open the advanced template in the template editor.
    
2.  Place the cursor where you want to insert the table.
    
3.  Click the **Table** button:
    
    ![Advanced PDF/HTML Templates New Element toolbar with the Tables button outlined in red.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPDFHTMLAddTable.png)
4.  Complete the Table Properties window and click **OK**.
    
    ![Advanced PDF/HTML Templates Table Properties popup window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/TemplateCustomization/AdvPrintingTablePropertiesWindow.jpg)
    
    The table is added to the template in the template editor.
    

You can resize the rows, columns, and cells of a table by positioning the cursor over the cell border and dragging it to the required size.

Note:

You can also use HTML markup source editing to add a table to an advanced template, but it's more time-consuming and requires knowing HTML.

Important:

If you have text overlapping a footer or missing from a printout, ensure that any long content is enclosed in an HTML element that will split across pages.

The Report Generator has specific rules for where page breaks can occur. A `<table>` tag nested inside a `<td>` tag is cut off at the bottom if it spreads across multiple pages. Only the following tags split correctly if they're spread across multiple pages:

          `<table> <ul> <p> <pre> <ol> <h1> <h2> <h3> <h4> <blockquote>` 
        

### Related Topics

-   [WYSIWYG Editing in the Template Editor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454197641.html)
-   [Template Editor Toolbar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1506352236.html)
-   [Adding and Removing Fields in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2864695.html)
-   [Adding and Formatting Text in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2865176.html)
-   [Including Images in Advanced Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3957689146.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
