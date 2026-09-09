---
id: "bridgehead_N2997678"
type: "bridgehead"
title: "Setting Your Script to Run With Administrative Privileges"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Executing Scripts Using a Specific Role > Setting Your Script to Run With Administrative Privileges"
parent: "chapter_N2997500"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2997678.html"
anchors: []
sha256: "d42d4898fbb2fe5bd44dafad09b0326822d44cbe3f35550dbe7f6b3724cfd442"
---

Sometimes a script needs to do something the initiating user's role can't. In these cases, you can execute the script as Administrator so it can read or change restricted records-or perform other high-privilege tasks-without failing.

Choose **Administrator** in the deployment's **Execute as Role** field only when the script needs full privileges, regardless of who's logged in.

For example:

-   A script that creates follow-up tasks after a sales order is saved and needs to read employee records-data many sales roles can't access.
    
-   Bundle installation scripts always need Administrator rights.
    
-   Scripts that run without a NetSuite session-like web store scripts or Suitelets marked Available Without Login-when they need NetSuite data. For more information, see [Setting Available Without Login](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997713.html).
    

#### To run a script as Administrator:

1.  Go to _Customization > Scripting > Script Deployments_
    
2.  Edit the deployment you want to change.
    
3.  In **Execute as Role**, select **Administrator**.
    
4.  Click Save.
    

Important:

Because the Administrator role gives unrestricted access, use it sparingly and only when other roles can't meet the script's needs.

### Related Topics:

-   [Executing Scripts Using a Specific Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997500.html)
-   [Script Types That Support Execute as Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1212112429.html)
-   [Setting Available Without Login](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997713.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
