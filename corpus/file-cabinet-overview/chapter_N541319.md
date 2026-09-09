---
id: "chapter_N541319"
type: "chapter"
title: "File Cabinet Overview"
branch: "file-cabinet-overview"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > File Cabinet Overview"
parent: "book_N473219"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html"
anchors: ["subsect_68150854965", "subsect_67151215977", "subsect_163723895810"]
sha256: "518a5a2d518646480bace5da027eaf5336e3a11a3cbe614ac85e764d47ef6e84"
---

Only users with the Administrator role and users with the Documents and Files permission can use the File Cabinet.

You can use the NetSuite File Cabinet to store and organize your business documents in much the same way as you store any files on your computer. You can store files that you receive or plan to send by email and you can attach files from the File Cabinet to records in NetSuite, such as customer records, transactions, and issues. Most File Cabinet folders can be restricted by the folder owner or an administrator.

The File Cabinet in NetSuite includes some folders that are created by default, depending on the features enabled in your account. You can identify folders created by NetSuite because the Internal ID is a negative number. In some cases, these folders serve a specific purpose. For example, SuiteScript script files are stored in the SuiteScripts folder.

Some files in the File Cabinet contain links that use URLs. Ensure that the URLs linking to those files contain account-specific domains. For example, the File Cabinet link should be _<accountID>_.app.netsuite.com, where _<accountID>_ is a variable representing your account ID. Use the Traffic Health tool to identify any existing data center-specific domains in links that you should update to account-specific domain links. For more information, see the [File Cabinet Traffic Health](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159303255545.html) topic in [Traffic Health](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157437326499.html).

## Permissions in the File Cabinet {#subsect_68150854965}

Your NetSuite account configuration or configuration of other critical business systems may depend on data in files stored in your NetSuite File Cabinet. In the File Cabinet, you can't restrict edit access at the file level. You can restrict access only to the folder that contains the file. You should set strict access control for which classes of users can edit or, if applicable, view those files in specific folders. Otherwise, a user may be able to change the configuration data in the file. A configuration change can potentially break the system or cause it to work in a way in which it was not intended.

Consider a critical workflow system that relies on a configuration containing a value APPROVER=email@example.com, and this configuration is accessed from a File Cabinet file. If a user edits the configuration file, they could change the email address and bypass the approval process. Ensure that only authorized users can edit the file. For more information, see [Restricting Access to File Cabinet Folders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542073.html).

You can block unauthorized internet access to a File Cabinet file, or let everyone in your company view the file by checking the required preference box. For more information, see [Preferences on File Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0530052000.html).

## System Notes in the File Cabinet {#subsect_67151215977}

Every file you add to the File Cabinet has a system notes record to track changes made to the file, including the context and when the changes were made. For more information, see [System Notes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158644279544.html) and [Searching System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html).

System notes for JSON, XML, and JavaScript files also include a File Content Hash field. NetSuite calculates the File Content Hash field based on the file contents, so it changes every time the file changes.

For remote files that you add to the File Cabinet using a URL, the File Content Hash field changes when you download this file or its parent folder from the File Cabinet. The value of the File Content Hash field also changes when NetSuite accesses the file through an internal process, such as a SuiteScript method call, or a SuiteFlow workflow step. This change is reflected in the system notes for that file.

## The File Cabinet and Your Website {#subsect_163723895810}

If you use Site Builder or SuiteCommerce Advanced, all website assets, including SSP Applications, are stored in the Website Hosting Files folder. For more information, read the following topics:

-   For information about hosting HTML files for a Site Builder website, read [Website Hosting with Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2598224.html).
    
-   For more information about SSP Applications, read [SSP Application Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2490486.html).
    
-   For more information about SuiteCommerce Advanced, read [Commerce Website Developer Documentation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2655313.html).
    

You can also create a company intranet site and post links to files stored in the File Cabinet. The following features are required to publish files to an intranet site:

-   File Cabinet
    
-   Document Publishing
    
-   Intranet
    

### Related Topics

-   [NetSuite Basics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_N473219.html)
-   [NetSuite Basics Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N473387.html)
-   [Getting Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N336026.html)
-   [Navigating NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N474404.html)
-   [Logging in to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1492022011.html)
-   [Logging out of NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158801369869.html)
-   [Using SuiteAnalytics Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7112240791.html)
-   [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)
-   [Working with Your Calendar and Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N499702.html)
-   [Working with Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N512006.html)
-   [Exporting Reports, Searches, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
