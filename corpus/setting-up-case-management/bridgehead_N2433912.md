---
id: "bridgehead_N2433912"
type: "bridgehead"
title: "Setting Up Online Case Forms for NetSuite OneWorld"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Setting Up Customer Support in NetSuite OneWorld > Setting Up Online Case Forms for NetSuite OneWorld"
parent: "section_N2433348"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433912.html"
anchors: ["procedure_N2433979"]
sha256: "73064523fb75b14f1fd773a367a9d7c3cf7d0c55f7e1d5e588a5e2e21568f0bb"
---

By default, the Subsidiary field is included on online case forms as a hidden search field. You can set the value of the subsidiary field on the form by adding the **subsidiary** parameter in the URL. You can also choose a default subsidiary on the Set Up Workflow subtab of the online case form.

If the field remains hidden on the form, customers won't see the subsidiary when they submit the form.

The Default Subsidiary preference sets which subsidiary to associate with a case when no subsidiary is explicitly set on the form. It determines:

-   **Which customers are considered when NetSuite searches for an existing record for the person submitting the form.**
    
    NetSuite only considers the customers associated with the subsidiary set on the form when determining if there's an existing record.
    
    For example, you set the Handle Duplicate Records preference to create a new customer record when there's no match. NetSuite creates the record and associates it with the subsidiary set on the form. If no subsidiary is set on the form and no default subsidiary is set, the new record is associated with your root parent subsidiary.
    
    Another example, there's no matching record and the Handle Duplicate Records preference isn't set to create a new record. NetSuite associates the new case with an anonymous customer record. If a subsidiary is set, the case is associated with that subsidiary's anonymous customer placeholder.
    
-   **The subsidiary set on the case record that is created.**
    

If a subsidiary isn't set through the form or through a URL parameter, the default subsidiary is applied. If there's no matching customer, the anonymous customer placeholder for that subsidiary is used. In case profiles, the value in the subsidiary filter overrides the default subsidiary set on the online case form.

#### To set up an online case form: {#procedure_N2433979}

1.  Go to _Setup > Support > Case Management > Online Case Forms > New_.
    
2.  On the **Select Fields** subtab, select either the **Company Name** field or the **First Name** and the **Last Name** fields, and mark them mandatory.
    
3.  Click the **Set Up Workflow** subtab.
    
4.  In the **Default Subsidiary** field, select the subsidiary you want to associate with cases submitted through this form.
    
5.  Set any other options you want. For example, add a logo on the form that's specific to a subsidiary.
    
6.  Click **Save**.
    

For more information about online case forms, see [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html).

### Related Topics

-   [Setting Company-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433546.html)
-   [Setting Subsidiary-Level Support Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433676.html)
-   [Setting Up Case Forms for NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2433829.html)
-   [Customizing Support Rep Roles for NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434051.html)
-   [Creating Case Rules and Territories Based on Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434106.html)
-   [Setting Up Your Mail Server for Email Case Capture in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2434142.html)
-   [Setting Up Customer Support in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2433348.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
