---
id: "SDFxml"
type: "SDFxml"
title: "SuiteCloud Development Framework XML Reference"
branch: "suitecloud-development-framework"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteCloud Development Framework > SuiteCloud Development Framework XML Reference"
parent: "chapter_4702622163"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml.html"
anchors: []
sha256: "d61ef0e8f241aa0e407a53b3cfdc60c6c26fe137d2ad6f6396d580fa7fc614de"
---

This reference documentation outlines the XML definitions of SDF custom objects that are supported in SuiteCloud Development Framework (SDF). This information includes their attributes, fields, field structures, field properties, possible field values, default field values, feature requirements, and other details.

For information about all of the customizations supported by SDF, see [Customizations Supported by SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4706653920.html).

For information about formats supported by SDF, see [Syntax Guidelines and Reference Formats for SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_24076946.html) and [Date and Time Formats in SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499269203.html).

For a table listing the root XML tag and script ID prefix for each SDF custom object, see [SDF Custom Object File Structure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1537555588.html).

Each SDF custom object in your SuiteCloud project must be represented as its own XML file and stored in the Objects folder. The root element in each file must be the XML definition of the SDF custom object. The following XML definitions of SDF custom objects are supported in SDF:

-   [addressForm](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3569816061.html)
    
-   [advancedpdftemplate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2214069420.html)
    
-   [bankstatementparserplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_450911196.html)
    
-   [bundleinstallationscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1616109134.html)
    
-   [center](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4252709751.html)
    
-   [centercategory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3893581673.html)
    
-   [centerlink](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3920524417.html)
    
-   [centertab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_300019872.html)
    
-   [clientscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4053132713.html)
    
-   [cmscontenttype](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4218421858.html)
    
-   [crmcustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4275481335.html)
    
-   [customglplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_117624676.html)
    
-   [customlist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2476691670.html)
    
-   [customrecordtype](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_372451363.html)
    
-   [customsegment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_274840654.html)
    
-   [customtransactiontype](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1766516211.html)
    
-   [dataset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1166002758.html)
    
-   [datasetbuilderplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_891141796.html)
    
-   [emailcaptureplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2376499874.html)
    
-   [emailtemplate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2610359453.html)
    
-   [entitycustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1378498284.html)
    
-   [entryForm](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_287092742.html)
    
-   [eventsubscriber](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7110236124.html)
    
-   [ficonnectivityplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2266593975.html)
    
-   [financiallayout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1929495528.html)
    
-   [fiparserplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3333781252.html)
    
-   [integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3719392610.html)
    
-   [itemcustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1799261045.html)
    
-   [itemnumbercustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_245003810.html)
    
-   [itemoptioncustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3170899425.html)
    
-   [kpiscorecard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4283963108.html)
    
-   [mapreducescript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3519311208.html)
    
-   [massupdatescript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2302851737.html)
    
-   [othercustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1832377546.html)
    
-   [pluginimplementation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1080430455.html)
    
-   [plugintype](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2530420543.html)
    
-   [portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_320447915.html)
    
-   [publisheddashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2517460692.html)
    
-   [reportdefinition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3105327707.html)
    
-   [restlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_410893908.html)
    
-   [role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2121043136.html)
    
-   [savedcsvimport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2642962146.html)
    
-   [savedsearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1933831387.html)
    
-   [scheduledscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1722194996.html)
    
-   [sdfinstallationscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1043649243.html)
    
-   [secret](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3777573046.html)
    
-   [singlepageapp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1427049920.html)
    
-   [sspapplication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1958249331.html)
    
-   [sublist](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1872888069.html)
    
-   [subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2906705078.html)
    
-   [suitelet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3243071555.html)
    
-   [toolset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_84193207470.html)
    
-   [transactionForm](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4143403259.html)
    
-   [transactionbodycustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3330726969.html)
    
-   [transactioncolumncustomfield](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2979546877.html)
    
-   [translationcollection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_4129151512.html)
    
-   [usereventscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2716615335.html)
    
-   [workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_3850241197.html)
    
-   [workbookbuilderplugin](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2903384145.html)
    
-   [workflow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_2086367724.html)
    
-   [workflowactionscript](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/SDFxml_1411852606.html)
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
