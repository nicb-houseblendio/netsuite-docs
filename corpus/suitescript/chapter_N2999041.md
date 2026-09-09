---
id: "chapter_N2999041"
type: "chapter"
title: "Defining Script Audience"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Defining Script Audience"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2999041.html"
anchors: ["bridgehead_N2999160", "bridgehead_N2999195"]
sha256: "5108d2caeb423f36aab2180e39a24fc3ca89da423131a0ace35137367fb681a9"
---

On the Audience subtab on the Script Deployment page, define the audience access for the script. When the script is deployed, it will only run in the roles specified in the Audience subtab.

The Audience subtab is included on the Script Deployment page for these script types: Suitelet, portlet, user event, global client (deployed at the record-level), RESTlet, mass update, and workflow action. You cannot specify an audience for scheduled scripts, map/reduce scripts, or bundle installation scripts.

Note:

Mass update script deployments and mass updates can both be assigned an audience. It is the user's responsibility to make sure the two audiences are in sync. For information about working with the mass update script type, see [SuiteScript 2.1 Mass Update Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460452911.html).

![The Script Deployment page Audience tab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/deploymentAudiences2.png)

General guidelines for specifying an audience:

-   If you don't specify any values on the Audience subtab, the script will execute only for the script owner even if the script deployment status is set to Released. For information about the differences between the Released and Testing deployment statuses, see [Setting Script Deployment Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2998873.html).
    
-   If you choose both role and department options on the Audience subtab, a user must belong to one of the selected roles AND one of the selected departments to execute the script. If you choose options for any other combinations of types (groups, employees, and partners), a user need only belong to a selected option of one type OR of another.
    
-   If you want the script to run only for specific users, select the appropriate roles, departments, groups, employees, or partners. If you want the script to run for all NetSuite users, do the following:
    
    -   Check the Select All box beside the Internal Roles field
        
    -   Select all roles in the External Roles field
        
    
    Note:
    
    When giving access to multiple roles, particularly external roles, ensure that each selected role has a valid need to access the script.
    

Be sure to save the Script Deployment record after all audience members have been defined.

If you are working with Suitelet Script Deployment records, see [Errors Related to the Available Without Login URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1524084097.html), which discusses the relevance of the Select All box as it pertains to internally and externally available Suitelets.

## Using the Audience Subtab to Test Scripts {#bridgehead_N2999160}

When the Status field on the Script Deployment record is set to Testing, you can test scripts assigned to specific audiences if you are a member of that audience type. For information about the Testing deployment status, see [Setting Script Deployment Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2998873.html).

For example, if you have a script that you want to execute for everyone in the Support Management role, you can log into NetSuite and then switch to the Support Management role to test the script. If the deployment status for the script is set to Testing, the script will run only for the script owner. After you have determined that the script runs as expected for the Support Management role, you can change the script's deployment status to Released. After it is set to Released, it will execute in the account for all those assigned to the Support Management role.

This is a good approach for script owners to verify that their script will run in the accounts for specified roles, departments, groups, employees, or partners.

## Using the Audience Subtab in OneWorld Accounts {#bridgehead_N2999195}

Script authors and owners who are developing scripts for NetSuite OneWorld accounts can specify a script audience based on subsidiary. In OneWorld accounts, the Audience subtab includes a Subsidiaries multiselect field. Don't forget to save your changes after selecting subsidiaries.

If the currently logged user is a member of a subsidiary which is selected in the multiselect field on the Script Deployment page, then the script is executed.

Script owners working in a OneWorld account that has multiple subsidiaries can select the subsidiaries they want their script to run in, and then log into an account of one of the specified subsidiaries. When a script's deployment status is set to Testing, the script will execute for the script owner and specified audience. This is a good way for script owners to verify that the script will run in accounts for specified subsidiaries.

![The Script Deployment page using the Audience tab for OneWorld accounts with the Subsidiaries list highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/deploymentAudiencesOneWorld2.png)

### Related Topics

-   [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html)
-   [Reviewing Outbound HTTPS and SFTP Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1555607753.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
