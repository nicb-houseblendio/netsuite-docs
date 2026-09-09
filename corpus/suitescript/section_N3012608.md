---
id: "section_N3012608"
type: "section"
title: "Understanding NetSuite Assistants"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Developer Guide > Working with UI Objects > Understanding NetSuite Assistants"
parent: "chapter_1543503740"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3012608.html"
anchors: ["bridgehead_N3012721", "bridgehead_N3012768"]
sha256: "5a22877f6baac04b7ede9a8a5ceae227ab1b2b19baf57d30e8cfa149a5cd1e7d"
---

In NetSuite, assistants are made of steps that users follow to complete a bigger task. Some assistants require steps to be done in order, while others let users complete steps in any order or skip some. In those assistants, the steps are provided only as guidelines for what users can do to finish the task.

The UI objects you use to build your assistant give it the same look and feel as built-in NetSuite assistants. For examples of these assistants, see these topics:

-   [SuiteBundler Assistant](#bridgehead_N3012721)
    
-   [Import Assistant](#bridgehead_N3012768)
    

## SuiteBundler Assistant {#bridgehead_N3012721}

The SuiteBundler Assistant is a built-in NetSuite assistant tool that guides users through the steps to bundle custom NetSuite solutions for deployment to other accounts.

Note:

To access the SuiteBundler Assistant, go to _Customization > SuiteBundler > Create Bundle_.

This figure shows Step 1 (page 1) of the SuiteBundler Assistant. Steps are in order and appear horizontally below the title.

You can build all the components shown here in your own custom assistant.

![The Bundle Builder page at the Bundle Basics step.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/assistantBundler.png)

| 1 | Assistant title |
| --- | --- |
| 2 | Steps positioned vertically |
| 3 | Fields in a field group |
| 4 | Splash screen |

## Import Assistant {#bridgehead_N3012768}

The Import Assistant guides users through steps to import data into NetSuite.

Note:

To access the Import Assistant, go to _Setup > Import/Export > Import CSV Records_.

The following figure shows how an error message appears in an assistant. Users can't move to the next step until the error is resolved. When you build custom assistants, you can throw errors that prevent users from moving to the next step.

![The Import Assistant page with an Import Type of Accounting selected.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteScript/SuiteScriptDeveloper/SuiteScriptDeveloperGuide/assistantCSV.png)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
