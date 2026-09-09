---
id: "section_N2897360"
type: "section"
title: "Deploying Skipped Custom Forms"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Deploying Upgraded Forms > Deploying Upgraded Custom Forms > Deploying Skipped Custom Forms"
parent: "section_N2896089"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897360.html"
anchors: ["procedure_N2897401"]
sha256: "df34e1abfaa8cca1cbf90163820f2423a454a2d2ea3ac3fd5abe02c6cb6b6f3f"
---

Use the following steps to deploy a custom form that you had previously 'skipped.'

Note that, as of 2012.2, the form upgrade process has been simplified to remove the Skip Upgrade option. The following procedure applies to any custom forms for which you skipped upgrade prior to that release.

Important:

Field groups created on existing custom forms that were skipped will not be carried over in the new upgraded form. You will notice this when you preview the upgraded custom form.

#### To deploy skipped custom forms: {#procedure_N2897401}

1.  Go to the Upgrade Checklist:
    
    1.  Go to _Customization > Forms > Transaction Forms \[or Entry Forms\]_ \[or Entry Forms\].
        
    2.  On the forms list page, in the message area at the top, click **Upgrade Checklist**. If you have already upgraded forms in your account, the link in the message area is called **Return to Upgrade Checklist**.
        
2.  Next to the custom form you want to deploy, in the **Deploy Options** column, click **Undo Skip and Upgrade Form**. After clicking this link, the **Edit** link reappears next to the form, and the form itself becomes a link.
    
3.  In the **Preview Name** column, click the custom form to preview.
    
    The form that appears will have the layout enhancements applied according to the NetSuite logic for applying these enhancements. See [Understanding Form Layout Enhancement Upgrade Logic](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897877.html) for details.
    
    Notice the following:
    
    -   The new [Field Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472396.html) that automatically render when you preview the form.
        
    -   The [Sublists and Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N472528.html) that have been added or removed.
        
    -   If you had previously added custom field groups to these forms, when you upgrade the layout and deploy the form, all standard fields you may have placed on a custom field group will automatically be placed into the fields groups NetSuite considers appropriate. All custom fields you had placed in a custom field group will appear at the bottom of the main area of the form and will not have a field group title. You will have to manually edit those fields and place them on new field groups.
        
4.  If you decide you approve of most of the changes to your form, but you need to make additional layout modifications before deploying the form to users, see [Editing the Layout of Custom Forms Prior to Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896507.html).
    
5.  Next, test the upgraded form. See [Testing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896824.html).
    
6.  After thoroughly previewing and testing the custom form, click the **Deploy Form** link.
    

### Related Topics

-   [Deploying Upgraded Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896089.html)
-   [Previewing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896302.html)
-   [Editing the Layout of Custom Forms Prior to Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896507.html)
-   [Avoid Editing Custom Forms in Tandem](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896749.html)
-   [Testing Undeployed Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2896824.html)
-   [Deploying Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2897031.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
