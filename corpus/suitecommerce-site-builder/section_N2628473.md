---
id: "section_N2628473"
type: "section"
title: "Defining Custom Web Site Tags"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Web Site Tags > Defining Custom Web Site Tags"
parent: "chapter_N2615371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628473.html"
anchors: ["bridgehead_N2628511", "bridgehead_N2628535", "procedure_N2628585"]
sha256: "6d5d498331c9d75263ac6fb003193d411f8b80440b06c2cbaf9d215e42cb1e64"
---

You can make your own custom tags to use in item or category templates and site themes. Use custom tags to repeat lines of custom HTML that you've created. You can also use custom tags to combine HTML with NetSuite item attribute tags to show information from a NetSuite record on your website.

By using custom tags, you don't have to enter a code snippet more than once. This gives you one place for your custom HTML, and it shows up everywhere you use the tag on your site.

## Tag Substitution {#bridgehead_N2628511}

You can also use custom tags in Tag Substitution. Tag Substitution on Tabs and Categories lets you change what your custom tag shows on certain pages of your site.

For example, if a site manager wants to hide search and navigation portlets on some tabs but not others, they can do it with tag substitution. First, create custom tags for each portlet by pasting the HTML code from the site theme into the portlets into custom tag records. Next, replace the HTML code in the theme for those portlets with custom tags. Finally, on each tab record that should be hidden, enter a tag substitution. For more information, see [Using Tag Substitution on Tabs and Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_71112650489.html).

## Creating Custom Tags {#bridgehead_N2628535}

Create custom tags to display information on your site. You can use custom tags to repeat lines of custom HTML, to combine HTML with attribute tags to display information from a NetSuite record on your website, or with tag substitution.

When you create a custom tag, you can use it in the following places:

-   Item records, in the store description field
    
-   Category records, in the brief and detailed description fields
    
-   Item/Category templates
    
-   Site themes
    

Important:

Web Site tags are not supported in SuiteCommerce Advanced websites.

#### To create a custom tag: {#procedure_N2628585}

1.  Go to _Commerce > Site Builder > Content > Tags > New_.
    
2.  In the **Tag** field, enter a name for your tag using all capital letters with no spaces.
    
    When you use this tag elsewhere in NetSuite, you will surround the tag with angle brackets. Do not enter the tag name with brackets here.
    
3.  In the **Description** field, enter an internal description about the purpose of the tag.
    
4.  In the **Default Value** field, enter what should appear when you do not define a substitution value on a tab or category record for this tag.
    
    Here, you can enter HTML, a combination of HTML and attribute tags, or a standard block of text.
    
5.  Click **Save**.
    

Important:

Do not use custom tag names that have the same names as HTML elements. Also, do not create custom tag names starting with 'NL' as this naming may conflict with default NetSuite tags.

### Related Topics

-   [Creating Attribute Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615537.html)
-   [Declare Attribute Tags for Tags Within Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2628302.html)
-   [Using the Server-Side Include Tag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2629027.html)
-   [Tags for Use in HTML Pages and Site Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2630406.html)
-   [Web Site Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2615371.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
