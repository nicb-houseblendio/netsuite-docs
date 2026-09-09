---
id: "section_N3364548"
type: "section"
title: "Types of Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Types of Bundles"
parent: "chapter_N3364150"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364548.html"
anchors: []
sha256: "807d2421cddad0f5eac1cd6db22a06849183895a9186bf9b53a287f255703bef"
---

There are two types of bundles that can be installed in NetSuite accounts:

-   A **customization bundle** is a collection of custom objects that customize the NetSuite application.
    
    -   Customization bundles allow installation of application packages.
        
    -   Customization bundles can include objects such as custom forms, SuiteScripts, and website layouts.
        
    -   Preferences can be set for some customization bundle objects to ensure desired setup.
        
    -   Some types of objects in customization bundles can be locked to prevent changes from being made to them in target accounts after bundles have been installed, to eliminate unintended changes.
        
    -   As part of the bundle installation and update process, conflicts between customization bundle objects and existing target account objects are detected and resolved.
        
    -   SuiteScripts that implement required bundle setup, called bundle installation scripts, can be associated with customization bundles to be run as part of bundle installation, update, or uninstall.
        
    -   For more information, see [Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364871.html).
        
-   A **configuration bundle** is a collection of NetSuite setup entries and preferences.
    
    -   Configuration bundles can simplify and standardize NetSuite account configuration.
        
    -   Configuration bundles can include settings such as auto-generated numbering settings, company preferences, and enabled features.
        
    -   You cannot do the following with a configuration bundle:
        
        -   Include locked objects in the bundle
            
        -   Share the bundle as public
            
        -   Uninstall the bundle from an account
            
        -   Include a bundle installation script to be run as part of bundle installation, update, or uninstall
            
    -   For more information, [Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html).
        

Important:

You cannot mix object types between customization and configuration bundles. For example, you cannot include custom fields in a configuration bundle. And, you cannot include a company preference in a customization bundle. If your solution requires both customization and configuration objects, then you must create two separate bundles.

### Related Topics

-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364871.html)
-   [Configuration Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3366315.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Managed Bundles Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382953.html)
-   [Saved Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3384420.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
