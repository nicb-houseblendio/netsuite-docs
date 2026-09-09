---
id: "bridgehead_N2857802"
type: "bridgehead"
title: "Working with Custom Buttons"
branch: "customization"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > Customization > Custom Forms > Creating Custom Entry and Transaction Forms > Configuring Buttons and Actions > Working with Custom Buttons"
parent: "section_N2857647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2857802.html"
anchors: ["procedure_N2857835"]
sha256: "1fb422d1a012408523fbbf79f04675b265197073f84e58158122752eab4c439a"
---

You can add custom buttons to forms to initiate client SuiteScript. For example, you could add Create Invoice button on a customer form that performs a specific function when the button is clicked. The Custom Actions subtab is visible when the Client SuiteScript feature is enabled in your account.

Important:

Custom buttons appear only when a record is in Edit mode. To make a button appear in View mode, use a User Event Script or Workflow.

#### To add a custom button to associate with client SuiteScript: {#procedure_N2857835}

1.  On the **Custom Code** subtab of the form, in the **Script File** field, add the client SuiteScript. For more information, see [Associating Custom Code (Client SuiteScript) Files With Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2860797.html).
    
    The primary object used to encapsulate custom buttons is `serverWidget.Button`. For more information, see [serverWidget.Button](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4325806317.html).
    
2.  On the **Custom Actions** subtab of the Custom Forms page, click the **Custom Actions** subtab.
    
3.  In the **Label** field, enter the UI label for the button. The label can be up to 99 characters long.
    
4.  In the **Function** field, enter the name of the function to perform when the button is clicked. The function can exist in your client SuiteScript file or any library file attached to the **Custom Code** subtab.
    
5.  In the **Display As** column, select **Button** to display the button as an inline button. Select **Menu** to have the button to appear as an action in the **More Actions** menu. For more information, see [About Button and Action Layout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2857884.html).
    
6.  Click **Save**.
    

### Related Topics

-   [Configuring Buttons and Actions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2857647.html)
-   [Working with Standard Buttons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2857736.html)
-   [About Button and Action Layout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2857884.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
