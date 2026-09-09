---
id: "section_N2592134"
type: "section"
title: "File Download with Online Forms"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Items, Forms, & Images > Publishing Forms > File Download with Online Forms"
parent: "section_N2590699"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592134.html"
anchors: ["procedure_N2592161"]
sha256: "a27601b49963d1c5e6de391b4534af3639081db9c87053e6e5f4b3e18034ca4c"
---

When you use the Sell Downloadable Files feature, you can offer your website visitors free file downloads when they submit contact information using an online customer form.

Before you set up this information item, create the online customer form customers will fill out to receive the download. For more information, see [Online Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N976289.html).

Upload the file that will be available for download. To do so, go to Documents > Files > File Cabinet. Choose the folder where you store items to download, and click Add File.

#### To set up an online form with a free download: {#procedure_N2592161}

1.  Go to _Commerce > Site Builder > Content Management > Publish Forms > New_.
    
2.  Click **File Download with Online Form**.
    
3.  In the **Name** field, enter a title for this form.
    
    This is the name of the link customers click to fill in and submit their information before downloading. For example, if this is a free music download when customers sign up for your newsletter, you might name it 'Free Download!'
    
4.  In the **Customer Form** field, select the online customer form that customers must fill out before downloading the file.
    
5.  In the **Downloadable File** field, select the file from the File Cabinet that customers can download for free after filling out the online customer form.
    
    Note:
    
    This file must be marked **Available Without Login** in the File Cabinet for customers to download the items.
    
6.  Select the **Display in Web Site** box.
    
7.  On the **Basic** subtab, enter any descriptions you want to appear with this item.
    
8.  At the bottom of the page, in the **Site Category** column, choose the category where you want to link to the form and download.
    
9.  Click **Add**.
    
10.  Repeat this process for each category where you want to display the link.
     
11.  On the **Media** subtab, choose a thumbnail image to appear with this customer form.
     
     For more information, see [Using Images in your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2592719.html).
     
12.  If you use the Multi-Language feature, see Multi-Language Names and Descriptions for more information about using the **Translations** subtab.
     
13.  Click **Save**.
     

The download automatically begins after site visitors submit their information. They may need to disable popups in their browser to continue downloading. A lead record is created or updated for the site visitor based on the settings in your online form.

Note:

If you host your website through NetSuite and want to publish a form, use the following tag within an href attribute: <%=getOnlineFormUrl(itemID)%>. The item ID can be found in the form record's URL.

### Related Topics

-   [Email Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591004.html)
-   [Search Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591207.html)
-   [Case and Customer Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2591690.html)
-   [Publishing Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2590699.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
