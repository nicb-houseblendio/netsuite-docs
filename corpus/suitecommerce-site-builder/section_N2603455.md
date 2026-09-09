---
id: "section_N2603455"
type: "section"
title: "Adding a 'Tell A Friend' Link"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Basic Customization > Adding a 'Tell A Friend' Link"
parent: "section_N2602412"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603455.html"
anchors: []
sha256: "a861471cce4b3894e08d5a4289877d2538c181c46fa8bd642e26cb94555e211c"
---

You can allow your customers to quickly send email messages to others containing links to items in your website using the 'tell a friend' preference. When you enable this preference, a site visitor can click a Tell A Friend link while viewing an item. Clicking this link opens a new message using the customer's email editor that contains a link to the item's page.

To enable this preference, go to _Commerce > Websites > Website List_. On the Appearance subtab, in the Tell a Friend section, check the Show 'Tell a Friend' Link box.

The Tell a Friend email message has a subject of 'Hi There,' contains the following text: 'I thought you would like to have a look at this product,' and includes the URL that points to the item in the Web store.

You can customize the text of this email at _Commerce > Site Builder > Content > Customize Text_. For more information, see [Customizing Website Text](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609254.html).

When you use a hosted site or a site with custom themes, you can also add the Tell a Friend link to hosted pages using an attribute tag in the following format:

          `<%=getCurrentAttribute('item','tellafriendlinkhtml')%>.` 
        

### Related Topics

-   [Creating and Editing Website Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602488.html)
-   [Changing Website Color Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603251.html)
-   [Basic Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602412.html)
-   [Using Web Site Text Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2609031.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
