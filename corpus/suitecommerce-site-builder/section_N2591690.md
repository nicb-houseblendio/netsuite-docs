---
id: "section_N2591690"
type: "section"
title: "Case and Customer Forms"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Items, Forms, & Images > Publishing Forms > Case and Customer Forms"
parent: "section_N2590699"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html"
anchors: ["procedure_N2591782", "bridgehead_N2592052"]
sha256: "d94fad1061cf045f3decb3fa64ee063f837b41c164ba5524adaa6093f55d7208"
---

When you publish an online form, customers can complete the form directly on your website. First create the case or customer form, and then follow the steps below to publish the form on your website.

See also, [Embedding an Online Form in your Website Page](#bridgehead_N2592052).

When you create an online form for publishing on your website, you must check the Enable Online box. Note that the Title on the online form record does not display on your site, but visitors on your site will see the text you enter in the Message field. You create the name for the form that is visible on the website, when you create the published form.

To create online case forms, go to Setup > Support > Online Case Forms > New. For more information about creating online case forms, see [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html).

To create online customer forms, go to _Setup > Marketing > Setup Tasks > Online Customer Forms > New_. For more information about creating online customer forms, see [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html).

#### To publish an online case or customer form: {#procedure_N2591782}

1.  Go to _Commerce > Site Builder > Content Management > Publish Forms_.
    
2.  Select the type of online form you want to publish:
    
    -   For case records, click **Case Form**.
        
    -   For online customer forms, click **Customer Form**.
        
3.  Enter a value in the **Name** field to create the link displayed on your site.
    
    When site visitors click this name, they are directed to the page where they can fill out your online form.
    
4.  In the **Case Form** field or the **Customer Form** field, select the online form you want to publish.
    
5.  Check the **Display in Web Site** box to make this form available to anyone who visits your site.
    
6.  At the bottom of the page, select the **Site Category** where you want the form to display.
    
    1.  If you use the Multiple Site feature, you must first select a **Site**, and then select the tab or category where you want this form published
        
    2.  Click **Add**.
        
7.  On the **Basic** subtab, the fields listed below are optional:
    
    -   You can enter a **Brief Description** and **Detailed Description** of this form. The brief description displays under the name of the published form in lists on your site. The detailed description displays on the page that displays the form.
        
    -   You can enter text in the **Featured Description** field which shows when a published form is featured on your home page.
        
        Note:
        
        Published forms can only be featured on your home page if you use a NetSuite presentation tab as your home page. Items are not automatically featured on custom HTML pages that you host through NetSuite.
        
        For more information, see [Featuring Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2585769.html).
        
    -   In the Search Keywords field, you can enter alternate words or misspellings that site visitors might use when searching your website to find this form.
        
8.  (Optional) On the **Media** subtab, select a thumbnail image to show next to the published form name in lists.
    
    For more information, see [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html).
    
9.  If you use the Multi-Language feature, see Multi-Language Names and Descriptions for more information about using the **Translations** subtab.
    
10.  Click **Save**.
     

## Embedding an Online Form in your Website Page {#bridgehead_N2592052}

When a visitor to your website clicks on a link to an online form, a redirect occurs to the page where the visitor completes the form. You might want to embed an online form on your website, to keep visitors on one page.

For example, the Professional Office Supply store has an external catalog website. The merchant wants site visitors to fill out an online customer form on the home page, but wants to keep them on that home page.

You can use an iFrame to embed an online form in your NetSuite web store page, or your own custom HTML page. This lets you display an online customer form in a scrollable box embedded in your web page. Use the sample code below, replacing the URL in the src attribute with the Publishable Form URL displayed on the External subtab of your online form record.

          `<iframe  src ="https://forms.netsuite.com/app/site/crm/externalleadpage.nl?compid=NCC133237&formid=6&h=2b495d8e81474994631c" width="100%"> </iframe>` 
        

To embed an online form in a NetSuite tab, edit the tab, and then add the iFrame in the Message field. For a category, add the iFrame in the Detailed Description field.

To embed an online form in a custom HTML page that is part of an external catalog site or an HTML page you host in the NetSuite File Cabinet, edit your file, and then add the iFrame to your custom HTML.

### Related Topics

-   [Email Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591004.html)
-   [Search Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591207.html)
-   [File Download with Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592134.html)
-   [Publishing Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2590699.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
