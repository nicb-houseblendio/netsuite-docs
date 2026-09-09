---
id: "chapter_N2997182"
type: "chapter"
title: "Setting Script Execution Event Type from the UI"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > SuiteScript Monitoring, Auditing, and Logging > Setting Runtime Options > Setting Script Execution Event Type from the UI"
parent: "chapter_N2996991"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2997182.html"
anchors: []
sha256: "489a570abb57564b4bf9ae26771fdab9d2fd36ddcf9033431013cccd34250e80"
---

On the Script Deployment page, use the Event Type field to choose the event that'll trigger your script (see following figure). If the Event Type field is left blank, the script will execute only on the events specified in the script file.

![The Script Deployment page setting the Event Type to Edit.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/eventTypeDropDown.png)

Note:

The Event Type field is available on Script Deployment pages for Suitelet, user event, and record-level client scripts only.

Use the Event Type field to specify a script execution context at the time of script deployment, without having to modify your .js script file. After you select an event type and click Save, the deployed script will execute only on that event, regardless of the event types specified in the .js script file.

Note that event types selected on the Script Deployment page take precedence over the event types specified in the .js script file. For example, if the **create** event type is specified in the script, selecting **Edit** from the Event Type field on the Script Deployment page will restrict the script from running on any event other than Edit.

The following snippet is from a user event script. Notice that the event type specified in the code is create (`context.UserEvent.CREATE`). If the Edit event type is specified on the Script Deployment page, the script will execute only when the specified record is edited, not created.

          `function followUpCallAfterSubmit(type) { // execute the logic in this script onlyif a new customer is created if (context.type !== context.UserEventType.CREATE) return; // obtain a handle to the newly created customer record var customerRecord = context.newRecord; // remainder of script...... } }` 
        

### Related Topics

-   [Script Deployment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4486246754.html)
-   [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html)
-   [Reviewing Outbound HTTPS and SFTP Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1555607753.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
