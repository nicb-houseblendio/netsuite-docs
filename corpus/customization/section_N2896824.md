---
id: "section_N2896824"
type: "section"
title: "Testing Undeployed Custom Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Deploying Upgraded Custom Forms > Testing Undeployed Custom Forms"
parent: "section_N2896089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896824.html"
anchors: ["procedure_N2896839"]
sha256: "5194799a864f8aa7d56dd8694d2a5ca461f3b6a8ee70af0fee59de11a527d77f"
---

When you test an undeployed custom form, you are viewing the form in the context of a record page. When in test mode, you have the opportunity of viewing the form as it appears in New mode and Edit mode.

When it comes to testing SuiteScripts on custom forms, you will be testing any client or user event scripts associated with the record type or the form.

#### To test undeployed custom forms: {#procedure_N2896839}

1.  Go to the Upgrade Checklist:
    
    1.  Go to _Customization > Forms > Transaction Forms \[or Entry Forms\]_ \[or Entry Forms\].
        
    2.  On the forms list page, in the message area at the top, click **Upgrade Checklist**. If you have already upgraded forms in your account, the link in the message area is called **Return to Upgrade Checklist**.
        
2.  Click the **Enable Test Mode** button on the bottom of the **Upgrade Checklist**.
    
3.  Use the navigation menus to go to the form you want to test.
    
    For example, if you want to test a custom sales order form, do one or all of the following:
    
    -   Go to _Transactions > Sales > Enter Sales Orders_ > New (to test a form in New mode)
        
    -   Go to _Transactions > Sales > Enter Sales Orders > List_ and click **Edit** next to an existing record (to test a form in Edit mode)
        
4.  In the page that appears, from the **Custom Form** list, select the custom form you want to test.
    
    Note:
    
    When in Test Mode, all custom forms that appear in the **Custom Form** list will appear with the upgraded layout. This includes both deployed and undeployed custom forms.
    
5.  Notice that the page layout changes to include field group and subtab [Form Layout Enhancements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N472127.html). Verify that the upgraded layout will suit your business needs.
    
6.  If you have any client or user event scripts associated with the form or the record type your are testing, verify that the scripts process as expected.
    
7.  After testing your custom form, return to the Upgrade Checklist by going to Customization > Forms > Transaction ( _or Entry_ ) Forms, and clicking Upgrade Checklist at the top of the page. If you have already upgraded forms in your account, the link in the message area is called Return to Upgrade Checklist.
    
8.  On the Upgrade Checklist, click the Disable Test Mode button to take the form out of test mode.
    
9.  After testing a custom form, you can now deploy the upgraded form to end users. See [Deploying Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897031.html) for details.
    

### Related Topics

-   [Deploying Upgraded Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896089.html)
-   [Previewing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896302.html)
-   [Editing the Layout of Custom Forms Prior to Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896507.html)
-   [Avoid Editing Custom Forms in Tandem](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896749.html)
-   [Deploying Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897031.html)
-   [Deploying Skipped Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897360.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
