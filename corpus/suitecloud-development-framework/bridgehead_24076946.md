---
id: "bridgehead_24076946"
type: "bridgehead"
title: "Syntax Guidelines and Reference Formats for SDF Custom Objects"
branch: "suitecloud-development-framework"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteCloud Development Framework > Developing SDF Custom Objects > Syntax Guidelines and Reference Formats for SDF Custom Objects"
parent: "section_4738081469"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_24076946.html"
anchors: ["subsect_1523296932", "subsect_1523297036", "subsect_1523297147", "subsect_1523297336", "subsect_1523297346", "subsect_1556720821", "subsect_1555435822", "subsect_1556720777", "subsect_1523297354"]
sha256: "4d01ca086a426e36a68a74367ab381b14c90df32585f5b5fef59891f4b17dbe1"
---

Depending on the type of reference or value you want to define in your SDF custom object for SuiteCloud Development Framework (SDF), see the following topics for syntax guidelines and examples:

-   [Specifying a Boolean Value](#subsect_1523296932)
    
-   [Specifying a System Enum](#subsect_1523297036)
    
-   [Working with Password Fields](#subsect_1523297147)
    
-   [Specifying a Standard Object Reference to NetSuite Components](#subsect_1523297336)
    
-   [Specifying an SDF Custom Object Reference](#subsect_1523297346)
    
-   [Specifying a Custom File or Script Reference](#subsect_1523297354)
    
-   [Specifying a Custom Segment Reference](#subsect_1556720777)
    

To reference an object that is external to your SuiteCloud project, see the following topics:

-   [Specifying a Reference to an SDF Custom Object in Another SuiteApp](#subsect_1556720821)
    
-   [Specifying a Bundle Object Reference](#subsect_1555435822)
    

## Specifying a Boolean Value {#subsect_1523296932}

To specify a Boolean value, set the content to either **T** or **F**. For example:

            `<isinactive>F</isinactive>` 
          

## Specifying a System Enum {#subsect_1523297036}

To specify a system enum, ensure that the content is in upper case. For example:

            `<permkey>ADMI_CUSTRECORD</permkey>` 
          

## Working with Password Fields {#subsect_1523297147}

When working with password fields, note that any content that you specify is ignored when you deploy the SuiteCloud project. When you import a custom object from a NetSuite account, the password fields are masked as **(Encrypted)**. For example:

            `<custrecord_password>(Encrypted)</custrecord_password>` 
          

## Specifying a Standard Object Reference to NetSuite Components {#subsect_1523297336}

To specify a standard object reference to NetSuite components, ensure that the content is in upper case. For example:

            `<recordtype>CUSTOMER</recordtype>` 
          

## Specifying an SDF Custom Object Reference {#subsect_1523297346}

To specify an SDF custom object reference, ensure that you use a `scriptid` attribute=value pair encased in square brackets. For example, the following is an SDF custom object reference to an object with a script ID of `custobject_tutorial`:

            `<recordtype>[scriptid=customrecord_sample]</recordtype>` 
          

Script ID descriptors can be set up according to a parent/child relationship, such as a custom field on a record. To specify an object in a hierarchical context, from the object's XML file, include the reference within square brackets using the following format: \[parentscriptid=<scriptid>`.` childscriptid=<scriptid>\]. In the following example, the script ID of the object is prefixed with the script ID of the parent, where parent script ID is `customrecordscriptid` and child script ID is `customrecordcustomfieldscriptid` delimited by a period(.):

            `[scriptid=customrecordscriptid.customrecordcustomfieldscriptid]` 
          

### Specifying a Reference to an SDF Custom Object in Another SuiteApp {#subsect_1556720821}

In addition to the `scriptid` descriptor, SDF custom object references support an `appid` descriptor.

To specify an external SDF custom object reference, include the reference within square brackets in the object's XML file , using the following format: \[`appid=<appid>, scriptid=<scriptid>`\]. For example, the following is an SDF custom object reference to an object with an application ID of `com.samples.mysuiteapp` and a script ID of `custobject_tutorial`:

              `[appid=com.example.mysuiteapp, scriptid=customrecord_example_mysuiteapp_objectname]` 
            

When creating script IDs for SDF custom objects in your SuiteApp using SDF or NetSuite, you should always include your company and application names to mitigate Script ID collisions.

Note:

In an account customization project, any custom fields or objects that you deploy to a target account cannot be deleted from that account using SuiteCloud Development Framework (SDF). You can only create or modify objects. To delete an SDF custom object, you must remove all object references, and manually delete it from the account.

### Specifying a Bundle Object Reference {#subsect_1555435822}

To specify an external bundle object reference , you must include a bundle id descriptor.

In the object's XML file where you want to add the reference, use the following format: \[`bundleid= <number>, scriptid=<scriptid>`\]. For example, the following is a reference to an SDF custom object with a bundle ID of 351 and a script ID of `custobject_tutorial`:

              `[bundleid=351, scriptid=customrecord]` 
            

Note:

You can only reference one bundle ID at the object level.

### Specifying a Custom Segment Reference {#subsect_1556720777}

When working with custom segment references, a type descriptor can be used to reference unified IDs. For example, the following is an SDF custom object reference to a `customrecordcustomfield` object with a script ID of `customrecordscriptid.customrecordcustomfieldscriptid` that exists in an SDF SuiteApp with the application ID of `com.samples.mysuiteapp`:

              `[appid=com.samples.mysuiteapp, type=customrecordcustomfield, scriptid=customrecordscriptid.customrecordcustomfieldscriptid]` 
            

Important:

The type descriptor is only supported in custom field references that are generated by the application of a custom segment to a record. These references are typically custom segment unified field IDs. You should always enable unified IDs on custom segments when using them with SDF. By using unified IDs, the script IDs in your custom segment objects do not contain account-specific values, making them more portable and accessible to other NetSuite accounts. For more information about creating a custom segment in NetSuite with unified IDs, see [Creating a Custom Segment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4313465979.html).

## Specifying a Custom File or Script Reference {#subsect_1523297354}

To specify a custom file or script reference, ensure that the content is the file path encased in square brackets. For example:

            `<scriptfile>[/SuiteScripts/UserEventScript.js]</scriptfile>` 
          

### Related Topics

-   [Developing SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738081469.html)
-   [Translatable Fields on SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156951732735.html)
-   [Downloading the XML Definition of an Object from a NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4738151284.html)
-   [SDF Custom Object File Structure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1537555588.html)
-   [Account-Specific Values Validation in SuiteCloud Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1528397245.html)
-   [Date and Time Formats in SDF Custom Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499269203.html)
-   [Lists, Records, and Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492224846.html)
-   [Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162860732056.html)
-   [Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158473189934.html)
-   [Import and Export](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492228461.html)
-   [Published Dashboards and Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492212651.html)
-   [Scripting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492241142.html)
-   [Plug-ins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492214715.html)
-   [Centers and Tabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492238718.html)
-   [Users and Roles in SDF](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492206995.html)
-   [Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492209268.html)
-   [SuiteCommerce Web Site Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492210847.html)
-   [SuiteAnalytics Workbooks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158492203868.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
