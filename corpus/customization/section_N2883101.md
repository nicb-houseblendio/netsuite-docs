---
id: "section_N2883101"
type: "section"
title: "Linking Online Custom Record Forms to My Website"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Records Overview > Creating Custom Record Types > Online Custom Record Forms > Linking Online Custom Record Forms to My Website"
parent: "section_N2882522"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2883101.html"
anchors: ["procedure_N2883122"]
sha256: "0c108bbd241f845b87bfc8a13eccfef362cede0d52a6b648d67831a16324bd76"
---

You can link to an online custom record form from your website.

If you have a NetSuite website, you can create a link to an online form in one of your information items, category descriptions, and from any other HTML description field.

#### To link to an online custom form from your NetSuite website: {#procedure_N2883122}

1.  Click the **Setup** tab.
    
2.  On the Setup page, under the Customization heading, click **Record Types**.
    
    The Custom Record Types list opens.
    
3.  In the **Edit** column, click the name of the record type you want to edit.
    
4.  Click the **Online Forms** subtab.
    
5.  Click the name of the form you want to link to.
    
6.  On the Online Custom Record Form page, click the **External** subtab.
    
7.  Copy the URL from the **Publishable Form URL** field.
    
    You can highlight the URL with your mouse, right-click, and then click **Copy**.
    
8.  Go to _Commerce > Site Builder > Content > Information Items_.
    
9.  Click **Edit** next to the information item you want to link to your online custom record form.
    
10.  Select the **Basic** subtab.
     
11.  Enter or paste the link in the description field you want the link to appear in.
     
     For example, the account administrator of Wolfe Electronics wants to include a line in a **Detailed Description** field that says, "Click here to register for your warranty." The word "here" links to the custom record form.
     
     You'd enter the following HTML code:
     
                     `<p>Click <a href='the Online Custom Record Form's URL'>here</a> to register for your warranty.</p>` 
                   
     
12.  Click **Save**.
     

Now your customers can follow the link to your online custom record form on your website. After this form is submitted, a record is created with the customer's information.

You can also link to your online custom record form from an external website or from an email message. To do this, copy and paste the form's URL into a link in your HTML document.

For more information about entering HTML in your website, see [Using HTML in Description Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2589998.html).

For more information about online custom record forms, see [Creating Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882662.html).

### Related Topics

-   [Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882522.html)
-   [Adding Custom Online Forms for a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879167.html)
-   [Creating Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2882662.html)
-   [Creating HTML Templates for Online Custom Record Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2885246.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
