---
id: "section_N2853340"
type: "section"
title: "Creating Custom Entry and Transaction Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms"
parent: "chapter_N2852749"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2853340.html"
anchors: ["procedure_N2853363"]
sha256: "a8a7b754a84b03db38bc87e7020bc4e3723bb77d65e4fc93bcc2c1730108cbef"
---

You can create your own custom entry and transaction forms by starting with an existing standard form and customizing it.

#### To create a custom entry or transaction form: {#procedure_N2853363}

1.  Choose a form to customize by doing one of the following:
    
    -   To customize an entry form, go to _Customization > Forms > Entry Forms_. Click **Customize** or **Edit** next to a form in the Custom Entry Forms list.
        
    -   To customize a transaction form, go to _Customization > Forms > Transaction Forms_. Click **Customize** or **Edit** next to a form in the Custom Transaction Forms list.
        
    -   If available, in view mode of a custom form, click the **Customize** link in the upper right, and then click **Customize Form**.
        
    
    Note:
    
    Forms labeled as (External) are used in the Customer Center and My Account section of your website.
    
2.  In the **Name** field, enter a name for your custom form.
    
3.  In the **ID** field, enter a unique alphanumeric ID for the custom form. For information about best practices and naming conventions, see [Conventions for Naming Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162428958352.html). For information about changing an existing ID, see [Changing the ID of a Custom Object](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162428789058.html).
    
    Note:
    
    You can't specify an ID for a transaction form when you create it, but you can change the ID after the form has been created.
    
4.  Set the custom form properties. Options vary depending on the type of form being customized. See the following topics:
    
    -   [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html)
        
    -   [Custom Transaction Forms Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html)
        
5.  Click **Save**.
    

For information about how to see what a completed form looks like, see [Viewing Completed Custom Entry and Custom Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_164813510950.html).

You can use SuiteCloud Development Framework (SDF) to manage custom entry and transaction forms as part of file-based customization projects. For more information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html). You can use the Copy to Account feature to copy an individual custom entry or transaction form to another of your accounts. You can use the Copy to Account feature to copy an individual custom entry or transaction form to another of your accounts. Each custom entry or transaction form page has a Copy to Account option in the upper-right corner. For more information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

For more information about customizing Entry forms, see [Custom Entry Form Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853525.html).

For more information about customizing Transaction forms, see [Custom Transaction Forms Properties](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2853604.html).

For more information, see the following topics.

-   [Moving Fields and Lists Between Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860592.html)
    
-   [Configuring Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856559.html)
    
-   [Configuring Fields or Screens](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2856992.html)
    
-   [Configuring Buttons and Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857647.html)
    
-   [Configuring Printing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858172.html)
    
-   [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html)
    
-   [Configuring QuickViews](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2859666.html)
    
-   [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html)
    
-   [Defining Preferred Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2873968.html)
    
-   [Adding Disclaimers to Transaction Form Footers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874493.html)
    
-   [Specifying Check Layout by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1513338497.html)
    
-   [Customizing Multiple Page Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874772.html)
    
-   [Linking Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861289.html)
    

After you've created a custom form, you should configure the subtabs. For more information, see [Configuring Subtabs for Custom Entry and Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2855162.html).

Important:

As you configure your custom form, consider whether the transactions to use the form require tax data. Only a form that includes required tax-related fields can be used for a transaction with tax consequences. You can't set tax field names through form customization. You must go to _Setup > Accounting > Set Up Taxes_. For more information, see [Customizing Tax Fields on Transaction Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1805065.html).

Note:

If you create or edit custom project forms when the Project Management feature is enabled, be aware that these forms can be altered if you later disable this feature. Immediately after you disable Project Management, you should review custom project forms to see if they have been changed, and if necessary, edit them to fit your requirements. For more information, see [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html) and [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html).

### Related Topics

-   [Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2852749.html)
-   [Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163605126400.html)
-   [Transaction Form Printing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4453516555.html)
-   [Creating Custom Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2862348.html)
-   [Creating Custom Note Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3914780887.html)
-   [Customizing Address Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2874310.html)
-   [Custom Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2861522.html)
-   [Customizing a Transaction Sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N551202.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
