---
id: "section_N2689968"
type: "section"
title: "Creating a Content Record"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > SuiteCommerce Integrations > Content Delivery Integration > Using Content Delivery > Creating a Content Record"
parent: "section_N2689412"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689968.html"
anchors: ["bridgehead_N2689992", "bridgehead_N2690032"]
sha256: "b7f23e8ed20521eca14ac345856afaad780cc95f8bf8d9e2957a63de6dc83225"
---

Content records hold information about media and files you want to display. Then you set up delivery rules with the Content Delivery SuiteApp. You create a new Content Record when you're setting up main body content for Landing Pages, or when you're defining Content Rules for Landing Pages or Content Records as described in [Using Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689412.html).

When you create a new Content Record, you select either Merchandising Rule or HTML.

## Using a Merchandising Rule {#bridgehead_N2689992}

You can only pick Merchandising Rules you've already set up. Simply select the rule you want, and click Save. For details on defining Product Merchandising rules, see [Product Merchandising](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687121.html).

![Shows how to select and save a merchandising rule in the NetSuite interface.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/SystemManagement/Integration/refCDPM.PNG)

## Using HTML {#bridgehead_N2690032}

You can use your own custom HTML elements to define the content you want to show. You can add HTML content to your record in two ways:

-   **File**: Select this to use an existing HTML file. You must upload the file to the file cabinet first. You can store these files anywhere, but it's best to keep them with your other website files in Web Site Hosting Files > Live Hosting Files.
    
-   **Text Editor**: Use the WYSIWYG editor to add your content. Type your content in the Content field and use the editor to add any formatting you want.
    

Note:

When you set the Type field to image, enter the image URL. Use the absolute path from your Live Hosting Files/site folder-usually the top images folder, like /images/navbar.jpg.

You can also add client-side JavaScript to add custom logic to your Content Delivery pages.

Note:

If you use jQuery methods in your code, make sure to use the `jQuery` prefix instead of `$`. For example, use `jQuery(document).ready(function(){alert('Hello World');});` instead of `$(document).ready(function(){alert('Hello World');});`.

Important:

While you can add client-side JavaScript to Content Delivery records, you can't reference external JavaScript libraries here. You would have to reference those from SSP application files or use more advanced customization.

![Shows where you can include your own custom HTML elements in the NetSuite interface.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/SystemManagement/Integration/refCDHTML.PNG)

### Related Topics

-   [Understanding Content Delivery Caching](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3824867874.html)
-   [Using Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689412.html)
-   [Understanding Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2689274.html)
-   [SEO Considerations for Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1491317607.html)
-   [Preparing Pages for Content Delivery](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2690549.html)
-   [Permission Validation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1542647720.html)
-   [Product Merchandising](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2687121.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
