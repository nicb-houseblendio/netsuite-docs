---
id: "section_N3380831"
type: "section"
title: "Documenting a Bundle"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Documenting a Bundle"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html"
anchors: ["bridgehead_N3380939", "procedure_N3381030", "bridgehead_N3381129", "bridgehead_N3381185", "bridgehead_N3381233"]
sha256: "42ba99c77d08ebce11f66044e86a34cf4e9decaec697735c4094a3e34b845532"
---

For every bundle you create, you should attach a document that describes the purpose of the bundle, how to install and use it, and where bundle users can get support when needed. This document should be aimed at administrators. There is a separate mechanism you can use to publish user documentation to the NetSuite Help Center. See [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html).

You specify a bundle documentation file in the **Admin Documentation** field, on the [Step 2 Bundle Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373339.html) page of the Bundle Builder. Use the provided NetSuite template as the basis for your bundle documentation file. For details, see:

-   [Using the Template to Create a Bundle Documentation File](#bridgehead_N3380939)
    
-   [Selecting a Bundle Documentation File from the File Cabinet](#bridgehead_N3381129)
    
-   [Selecting a Bundle Documentation File from Your Computer](#bridgehead_N3381185)
    

You also can enter a URL in the **Admin Documentation** field, to link to an externally hosted site that provides documentation. For more information, see [Using a Website to Provide Bundle Documentation](#bridgehead_N3381233).

## Using the Template to Create a Bundle Documentation File {#bridgehead_N3380939}

To facilitate the creation of your bundle document, NetSuite provides a Microsoft Word template (.dot file) that you can upload and use to structure your document. The template has been designed specifically for bundle documents and can be filled in. Using the template ensures that your documentation is efficient, consistent, and meets customer needs.

The template includes the following elements or sections:

-   Cover page
    
-   Copyright page
    
-   Table of Contents
    
-   Overview
    
-   Installing the Bundle
    
-   Using the Bundle
    
-   Updating the Bundle
    
-   Uninstalling the Bundle
    
-   Support
    

Although you can adapt this template, you should use this structure to ensure correct installation by administrators and effective adoption by users of the SuiteBundler.

#### To create a document using the bundle document template: {#procedure_N3381030}

1.  Start the Bundle Builder, at _Setup > Customization > SuiteBundler > Create Bundle_.
    
2.  On the Bundle Properties page, click the inline text Template link, or click the label for the **Admin Documentation** field, and then click **Template** in the field level help.
    
3.  Choose whether to open the template using Microsoft Word or to save the template file.
    
4.  Before you begin entering your text, save the template as a Word .doc type file.
    
5.  In the Word .doc file, replace the text in the grey fields with your own text.
    
    Important:
    
    You must include the entire NetSuite Disclaimer provided in the Support section.
    
6.  When you have completed entering the text in your Word .doc file, generate a PDF file.
    
7.  Return to the Bundle Properties page of the Bundle Builder.
    
8.  In the **Admin Documentation** field, click **New** from the dropdown list for the field.
    
9.  In the **File** popup window, select **Computer** in the **Attach From** field, check the **Available for SuiteBundles** box, click the **Browse** button, browse to the file, and click **Save**.
    
    The selected file appears in the **Documentation** field.
    

## Selecting a Bundle Documentation File from the File Cabinet {#bridgehead_N3381129}

To use a previously created document that has already been uploaded to the NetSuite File Cabinet as your bundle documentation file:

1.  Go to the Bundler Properties page of the Bundle Builder , at _Setup > Customization > SuiteBundler > Create Bundle_.
    
2.  In the **Admin Documentation** field, click **List** from the dropdown list for the field.
    
3.  In the **Choose Documentation** popup, select the file.
    
    The selected file is listed in the **Documentation** field.
    

Note:

If you do not see the file in the list and you are sure it was uploaded to the File Cabinet, it is possible it was not marked Available for SuiteBundles. You can edit the File Cabinet record to check this box.

## Selecting a Bundle Documentation File from Your Computer {#bridgehead_N3381185}

To use a previously created document that has not been uploaded to the NetSuite File Cabinet as your bundle documentation file:

1.  Go to the Bundle Properties page of the Bundle Builder , at _Setup > Customization > SuiteBundler > Create Bundle_.
    
2.  In the **Admin Documentation** field, click **New** from the dropdown list for the field.
    
3.  In the **File** popup, select **Computer** in the **Attach From** field, check **Available for SuiteBundles**, click the **Browse** button, browse to the file, and click **Save**.
    
    The selected file is listed in the **Documentation** field.
    

## Using a Website to Provide Bundle Documentation {#bridgehead_N3381233}

To use an externally hosted website to provide bundle documentation:

1.  Go to the Bundle Properties page of the Bundle Builder , at _Setup > Customization > SuiteBundler > Create Bundle_.
    
2.  In the **Admin Documentation** field, click **New** from the dropdown list for the field.
    
3.  In the **File** popup, select **Web** in the **Attach From** field and enter the URL in the **URL** field, and click **Save**.
    
    The entered URL is listed in the **Documentation** field.
    

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Publishing SuiteApp Help Content to the NetSuite Help Center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499368555.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
