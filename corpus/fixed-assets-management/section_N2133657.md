---
id: "section_N2133657"
type: "section"
title: "Viewing Script Error Notification Settings for Fixed Assets Management"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Managing Fixed Assets Scripts > Viewing Script Error Notification Settings for Fixed Assets Management"
parent: "chapter_164857349671"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2133657.html"
anchors: ["procedure_N2134952"]
sha256: "b4c2be72dfc2f21fef262c7a807dc8757c66359413df44e72ba539820eba0116"
---

The following table lists the default notification setting for each type of FAM script:

| FAM Script Type | Notification Setting |
| --- | --- |
| Client | Notify Current User |
| Suitelet | Notify Current User |
| User Event (UE) | Notify Current User |
| Scheduled | Notify All Admins |
| Bundle Installation | Notify All Admins |

Note:

All FAM scripts are locked. The notification settings cannot be changed.

#### To view the notification setting for a FAM script: {#procedure_N2134952}

1.  Go to Customization > Scripting > Scripts.
    
2.  On the Scripts page, click **View** next to the script whose settings you want to view.
    
    Note:
    
    You can use the filters at the top of the page to refine the list on the Scripts page.
    
3.  On the Script page, click the **Unhandled Errors** subtab. The selected option shows which notification is used for script errors:
    
    -   **Notify Current User** - NetSuite sends an email to the currently logged-in user.
        
    -   **Notify All Admins** - NetSuite sends an email to all users with the Administrator role.
        
    
    Note:
    
    The **Notify Script Owner**, **Notify Group**, and **Notify Emails** settings are currently not in use.
    

### Related Topics

-   [Managing Fixed Assets Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_164857349671.html)
-   [Fixed Assets Management Script Priority](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164857361903.html)
-   [Changing the Scheduled Script Runtime](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508315379.html)
-   [Updating Script Deployment Settings for Suitelets Available Without Login](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0714041106.html)
-   [Running the Migration Script to Update the Fixed Assets Management SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164857381791.html)
-   [Fixed Asset Error Recovery Script](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1016064026.html)
-   [Background Processing of Fixed Assets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_164861655712.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
