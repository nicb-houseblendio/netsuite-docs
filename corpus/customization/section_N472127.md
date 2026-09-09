---
id: "section_N472127"
type: "section"
title: "Form Layout Enhancements"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Form Layout Enhancements"
parent: "chapter_N2894013"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html"
anchors: ["bridgehead_N472224"]
sha256: "940e919b91e521769f78fdbf50bd323c3e127518b1e4d9034b5896946adff714"
---

Version 2010.2 introduced a new user interface (UI), which included a set of changes categorized as **Form Layout Enhancements**. These form layout enhancements were not automatically applied to custom forms that were created prior to 2010.2. NetSuite administrators have the option of applying form layout enhancements to each custom form, as described in [Deploying Upgraded Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896089.html).

Form layout enhancements include the following:

-   The addition of [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html) to organize all fields on a record into logical groups.
    
-   The consistent naming and placement of [Sublists and Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html).
    
    NetSuite administrators can **upgrade** the transaction and entry forms in their account to include these enhancements. Administrators must then **deploy** the upgraded forms to their NetSuite users before the users can begin working with the enhanced forms.
    
    Administrators should use the **Upgrade Checklist** to manage the form upgrade and deployment processes. If you are an account administrator, see [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html) to learn more.
    
    Important:
    
    As of 2012.2, form layout enhancements have been applied to all standard forms.
    

## Form Layout Enhancements (The Big Picture) {#bridgehead_N472224}

AI Assisted Content, Date: February 19, 2026, Writer: Jennifer Zwaniga, Description: I used Chatbot with issue 853976 to describe the issue record contents, identify if a note was needed, where to add it, and what to say about it, Assisted by Oracle Chatbot openai.gpt-4.1,

The following screenshots show the difference between a form that has been upgraded to include the [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html) and one that has not.

The first screenshot is a view of a sales order with a custom sales order form applied. In this screenshot, the [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html) and the [Sublists and Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html) changes associated with the Form Layout Enhancements have not yet been applied to the custom form used for this record.

![Sample form without form layout enhancement applied.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/nonFormLayoutEnhancement.png)

The second screenshot shows the same record, but with an 'upgraded' standard sales order form. The upgraded form now includes:

-   [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html) - All fields in the main header area are organized into the Primary Information, Sales Information, and Classification field groups. Based on the data in the record, NetSuite automatically created these field groups when the account administrator upgraded the form.
    
    ![Sample form with form layout enhancement applied.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/formLayoutEnhancementsApplied.png)
    
    Note:
    
    The Main section at the top of an entry form is used for fields and summary information only. Sublists are only supported in the lower part of the form, under designated subtabs. For more information, see [Configuring Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2858591.html).
    
-   Updated [Sublists and Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html) - Subtab and sublist data have been reorganized into more meaningful categories. In this example, the Address, Payment, Messages, and History tabs have been removed. Content that was previously on these subtabs has been moved to the main header area or other subtabs/sublists. The Billing, Accounting, Relationships, Communication, Related Records, and System Information tabs have been added.
    
    ![Sample form Items sublist with form layout enhancements applied.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBuilderCustomization/formLayoutEnhancements2Applied.png)

See the following topics:

-   [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html)
    
-   [Sublists and Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html)
    

### Related Topics

-   [Deploying Upgraded Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2894013.html)
-   [Custom Form Deployment Process (Summary)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2894227.html)
-   [Deploying Upgraded Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896089.html)
-   [Understanding Form Deployment Statuses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897563.html)
-   [Understanding Form Layout Enhancement Upgrade Logic](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
